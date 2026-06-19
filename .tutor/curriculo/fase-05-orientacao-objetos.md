# Fase 05 — Orientação a objetos sem exagero

**Duração sugerida:** 4 semanas

## Objetivo da fase

Aprender a organizar responsabilidades — orientação a objetos não é criar uma classe para tudo.

## Pré-requisitos

Fase 04 concluída.

## Tópicos e ordem sugerida

Classe, objeto, estado, comportamento, encapsulamento, abstração, herança, composição, interface, polimorfismo, coesão, acoplamento.

### Princípios importantes

- Prefira composição a herança quando fizer sentido.
- Uma classe deve ter uma responsabilidade clara.
- Métodos devem ter nomes que expressem intenção.
- Evite objetos que sabem demais e funções gigantes.
- Modele regras de negócio perto do domínio.

## Atividades / exercícios esperados

Projeto da fase: sistema simples de biblioteca, com entidades Livro, Usuário, Empréstimo e Biblioteca. Regras: um livro pode estar disponível ou emprestado; um usuário pode pegar até 3 livros; um empréstimo tem data de início e data prevista de devolução; não pode emprestar livro indisponível; atraso deve gerar aviso. Implementar em TypeScript e depois em Python.

Perguntas de revisão: onde está a regra de negócio? Qual classe tem responsabilidade demais? O que pode virar função pura? O que precisa ser testado? O que aconteceria se adicionássemos multa por atraso?

## Critérios para avançar

- [ ] O sistema de biblioteca funciona nas duas linguagens e respeita as 4 regras descritas.
- [ ] Consegue identificar, no próprio código, uma classe com responsabilidade demais.
- [ ] Respondeu às perguntas de revisão por escrito.

## Como a IA deve ajudar nesta fase

- Fazer as perguntas de revisão acima depois que o aluno implementar o sistema.
- Apontar quando uma classe estiver acumulando responsabilidades demais, explicando o porquê.

## Como a IA NÃO deve ajudar nesta fase

- Não desenhe a arquitetura de classes completa antes do aluno tentar modelar sozinho.
