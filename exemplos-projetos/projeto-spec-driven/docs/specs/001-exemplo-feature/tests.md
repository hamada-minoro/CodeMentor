# Tests: Lista de Favoritos

## Cenários principais
- [ ] Deve favoritar uma categoria existente
- [ ] Deve desfavoritar uma categoria favoritada
- [ ] Deve listar categorias com favoritos primeiro, ordenados por nome

## Cenários de erro
- [ ] Deve retornar 404 ao favoritar categoria inexistente
- [ ] Deve retornar 401 ao favoritar sem autenticação
- [ ] Deve ser idempotente ao favoritar a mesma categoria duas vezes (sem erro, sem duplicata)
- [ ] Deve ser idempotente ao desfavoritar uma categoria que não estava favoritada

## Testes manuais

1. Criar um usuário e autenticar.
2. Listar categorias — nenhuma deve aparecer como favorita.
3. Favoritar uma categoria.
4. Listar categorias novamente — a categoria favoritada deve aparecer primeiro, com `isFavorite: true`.
5. Desfavoritar a mesma categoria.
6. Listar categorias novamente — a ordenação deve voltar ao padrão (por nome).
