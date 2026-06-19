# Plan: Lista de Favoritos

## 1. Resumo técnico

Adicionar uma tabela de junção `favorite_categories` ligando usuários a categorias. Expor dois novos endpoints (favoritar/desfavoritar) e ajustar o endpoint de listagem de categorias para ordenar favoritos primeiro.

## 2. Arquivos impactados

- `src/modules/categories/categories.repository.ts`
- `src/modules/categories/categories.service.ts`
- `src/modules/categories/categories.controller.ts`
- `src/modules/categories/categories.schema.ts`
- Nova migration para `favorite_categories`

## 3. Modelo de dados

```text
favorite_categories
  id          uuid (pk)
  user_id     uuid (fk -> users.id)
  category_id uuid (fk -> categories.id)
  created_at  timestamp

  unique(user_id, category_id)
```

## 4. Contratos de API

- `POST /categories/:id/favorite` → 204 No Content (idempotente)
- `DELETE /categories/:id/favorite` → 204 No Content (idempotente)
- `GET /categories` → lista existente, agora com campo `isFavorite: boolean` em cada item, ordenada com favoritos primeiro

## 5. Estratégia de validação

- Validar que `:id` existe na tabela `categories` antes de inserir o favorito (404 se não existir).
- Exigir autenticação em ambos os novos endpoints (401 se ausente).
- Tratar inserção duplicada como no-op, não como erro (usar `ON CONFLICT DO NOTHING` ou equivalente).

## 6. Estratégia de testes

- Unitário: lógica de ordenação (favoritos primeiro, depois por nome).
- Integração: favoritar, desfavoritar, favoritar categoria inexistente, favoritar sem autenticação, favoritar a mesma categoria duas vezes.
- Manual: listar categorias antes e depois de favoritar uma, visualmente confirmando a ordenação.

## 7. Riscos

- Esquecer o índice único `(user_id, category_id)` pode gerar duplicatas silenciosas.
- Se categorias globais existirem, garantir que o favorito é sempre por usuário, nunca global.

## 8. Plano incremental

1. Criar migration de `favorite_categories`.
2. Implementar repository com métodos `addFavorite`, `removeFavorite`, `isFavorite`.
3. Implementar os dois novos endpoints no controller/service.
4. Ajustar o endpoint de listagem para incluir `isFavorite` e a ordenação.
5. Escrever testes de integração para os cenários do `tests.md`.
