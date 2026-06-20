# Módulo 05 — Orientação a objetos sem exagero (Python)

**Duração sugerida:** 4 semanas (6 aulas)

## Objetivo do módulo

Aprender a organizar responsabilidades — orientação a objetos não é criar uma classe para tudo.

## Pré-requisitos

Módulo 04 concluído.

## Aulas

### Aula 1 — Classe, objeto, estado e comportamento

O vocabulário básico de OO em Python: `class`, `__init__`, atributos, métodos.

### Aula 2 — Encapsulamento e abstração

Convenções de Python para "privado" (`_nome`, `__nome`), e o que esconder vs. o que expor.

### Aula 3 — Herança e composição

Quando herdar e quando compor — e por que compor costuma ser a escolha mais segura.

### Aula 4 — Interfaces e polimorfismo

Duck typing em Python, classes abstratas (`abc`), protocolos.

### Aula 5 — Coesão e acoplamento

Como perceber uma classe que "sabe demais" ou está fortemente amarrada a outra.

### Aula 6 — Princípios práticos

- Prefira composição a herança quando fizer sentido.
- Uma classe deve ter uma responsabilidade clara.
- Métodos devem ter nomes que expressem intenção.
- Evite objetos que sabem demais e funções gigantes.
- Modele regras de negócio perto do domínio.

## Atividades / exercícios esperados

Projeto do módulo: sistema simples de biblioteca, em Python, com entidades `Livro`, `Usuario`, `Emprestimo` e `Biblioteca`. Regras: um livro pode estar disponível ou emprestado; um usuário pode pegar até 3 livros; um empréstimo tem data de início e data prevista de devolução; não pode emprestar livro indisponível; atraso deve gerar aviso.

Perguntas de revisão: onde está a regra de negócio? Qual classe tem responsabilidade demais? O que pode virar função pura? O que precisa ser testado? O que aconteceria se adicionássemos multa por atraso?

## Critérios para avançar

- [ ] O sistema de biblioteca funciona e respeita as 4 regras descritas.
- [ ] Consegue identificar, no próprio código, uma classe com responsabilidade demais.
- [ ] Respondeu às perguntas de revisão por escrito.

## Como a IA deve ajudar neste módulo

- Fazer as perguntas de revisão acima depois que o aluno implementar o sistema.
- Apontar quando uma classe estiver acumulando responsabilidades demais, explicando o porquê.

## Como a IA NÃO deve ajudar neste módulo

- Não desenhe a arquitetura de classes completa antes do aluno tentar modelar sozinho.
