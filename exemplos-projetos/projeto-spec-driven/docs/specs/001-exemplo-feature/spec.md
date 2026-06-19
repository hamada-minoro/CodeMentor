# Spec: Lista de Favoritos

## 1. Contexto

Usuários da API financeira querem marcar categorias de despesa como "favoritas" para acessá-las mais rápido ao registrar uma nova transação. Hoje, todas as categorias aparecem em uma lista única e sem ordenação por uso.

## 2. Objetivo

Permitir que o usuário marque e desmarque categorias como favoritas, e que a listagem de categorias mostre os favoritos primeiro.

## 3. Não objetivos

- Não inclui reordenação manual dos favoritos (apenas favoritar/desfavoritar).
- Não inclui favoritos compartilhados entre usuários — é uma preferência individual.

## 4. Usuários envolvidos

Qualquer usuário autenticado da API financeira que cadastra transações.

## 5. Regras de negócio

- Uma categoria só pode ser favoritada pelo usuário que a está visualizando (favorito é por usuário, não global).
- Um usuário pode favoritar quantas categorias quiser.
- Desfavoritar uma categoria não a remove do sistema, apenas tira da lista de favoritos do usuário.

## 6. Fluxo principal

1. Usuário autenticado envia requisição para favoritar uma categoria.
2. Sistema valida que a categoria existe e pertence ao escopo do usuário (ou é uma categoria global).
3. Sistema registra a preferência e retorna sucesso.

## 7. Fluxos alternativos

- Usuário desfavorita uma categoria já favoritada.
- Usuário lista categorias e vê favoritos no topo, ordenados por nome.

## 8. Casos de erro

- Categoria inexistente: retornar 404.
- Usuário não autenticado: retornar 401.
- Categoria já favoritada e usuário tenta favoritar de novo: operação deve ser idempotente (não deve gerar erro nem duplicar).

## 9. Critérios de aceitação

- [ ] Dado um usuário autenticado, quando ele favorita uma categoria existente, então a categoria passa a aparecer na lista de favoritos.
- [ ] Dado um usuário autenticado, quando ele desfavorita uma categoria, então ela some da lista de favoritos mas continua existindo no sistema.
- [ ] Dado um usuário sem autenticação, quando ele tenta favoritar uma categoria, então o sistema retorna 401.
- [ ] Dado um usuário autenticado, quando ele lista categorias, então os favoritos aparecem primeiro, ordenados por nome.

## 10. Dados necessários

Nova entidade `FavoriteCategory`: `id`, `userId`, `categoryId`, `createdAt`. Relacionamento N:N entre `User` e `Category`, mediado por essa entidade.

## 11. Requisitos não funcionais

- Segurança: usuário só pode favoritar/desfavoritar para si mesmo, nunca para outro usuário.
- Performance: a listagem de categorias com favoritos não deve degradar significativamente com o volume esperado (poucas centenas de categorias por usuário).

## 12. Dúvidas em aberto

- Categorias globais (compartilhadas entre todos os usuários) podem ser favoritadas individualmente? (Assumido que sim, neste exemplo — mas isso deveria ser confirmado com o "dono do produto" antes de implementar em um projeto real.)
