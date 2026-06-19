# Tasks: Lista de Favoritos

## Preparação
- [ ] Ler `CLAUDE.md`
- [ ] Ler `spec.md` e `plan.md`
- [ ] Confirmar escopo (sem reordenação manual, sem favoritos compartilhados)

## Implementação
- [ ] Criar migration de `favorite_categories` com constraint única `(user_id, category_id)`
- [ ] Criar método `addFavorite(userId, categoryId)` no repository
- [ ] Criar método `removeFavorite(userId, categoryId)` no repository
- [ ] Criar método `listCategoriesWithFavorites(userId)` no repository, com ordenação de favoritos primeiro
- [ ] Criar endpoint `POST /categories/:id/favorite`
- [ ] Criar endpoint `DELETE /categories/:id/favorite`
- [ ] Ajustar endpoint `GET /categories` para usar o novo método do repository
- [ ] Criar testes unitários da lógica de ordenação
- [ ] Criar testes de integração dos cenários de erro e sucesso

## Validação
- [ ] Rodar testes
- [ ] Rodar lint
- [ ] Testar fluxo manual: favoritar, listar, desfavoritar, listar de novo
- [ ] Atualizar documentação de endpoints
- [ ] Revisar aderência à spec (critérios de aceitação)
