# Review: Lista de Favoritos

> Exemplo de como `review.md` ficaria preenchido ao final da implementação desta feature de exemplo.

## Aderência à spec
- [x] Implementação cumpre os 4 critérios de aceitação listados em `spec.md`
- [x] Não objetivos foram respeitados (sem reordenação manual, sem favoritos compartilhados)
- [x] Casos de erro foram tratados (404, 401, idempotência)

## Qualidade
- [x] Código simples — sem abstração extra para um caso de uso ainda não pedido
- [x] Nomes claros (`addFavorite`, `removeFavorite`, `isFavorite`)
- [x] Baixo acoplamento — lógica de favoritos isolada no repository de categorias
- [x] Testável — testes unitários e de integração cobrem os cenários de `tests.md`
- [x] Sem dependências desnecessárias

## Segurança
- [x] Entrada validada (categoria existe antes de favoritar)
- [x] Permissões verificadas (favorito é sempre por usuário autenticado, nunca por outro usuário)
- [x] Dados sensíveis protegidos (não aplicável diretamente nesta feature, mas verificado que nenhum dado de outro usuário é exposto na listagem)

## Pendências

- Confirmar com o "dono do produto" se categorias globais devem mesmo ser favoritáveis individualmente (dúvida registrada em `spec.md`, seção 12).
- Avaliar, em uma iteração futura, se vale a pena cachear a lista de favoritos por usuário caso o volume de categorias cresça muito.
