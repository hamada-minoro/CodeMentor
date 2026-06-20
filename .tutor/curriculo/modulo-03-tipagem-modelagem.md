# Módulo 03 — Tipagem e modelagem de dados (Python)

**Duração sugerida:** 3 a 4 semanas (6 aulas)

## Objetivo do módulo

Entender contratos, tipos e estruturas de dados — uma das bases mais importantes para trabalhar bem com IA depois, já que descrever bem os tipos reduz ambiguidade.

## Pré-requisitos

Módulo 02 concluído.

## Aulas

### Aula 1 — Tipagem dinâmica e inferência

Como o Python decide o tipo de uma variável em tempo de execução, e os limites disso.

### Aula 2 — Contratos e DTOs

O que é um contrato de dados, e como representar um com `dataclass` ou `TypedDict`.

### Aula 3 — Validação

Validar dados de entrada manualmente, e uma introdução a `pydantic` para contratos mais robustos.

### Aula 4 — Tipos opcionais e nulos

`Optional`, `None`, e os bugs comuns de não tratar ausência de valor.

### Aula 5 — Imutabilidade

Quando preferir estruturas imutáveis (tuplas, `frozen=True`), e por quê.

### Aula 6 — Schema de dados

Descrever a "forma" de um dado antes de implementar qualquer função que o manipule.

## Atividades / exercícios esperados

Modelar os mesmos domínios em Python: usuário, produto, pedido, pagamento, tarefa, funcionário, equipamento, agendamento. Para cada domínio, definir campos obrigatórios, campos opcionais, regras de validação, estados possíveis, exemplos válidos e exemplos inválidos.

Projeto do módulo: pequena biblioteca de validação de dados (e-mail válido, CPF com tamanho correto, senha forte, data futura, número positivo, string obrigatória). Não precisa ser perfeita — o objetivo é pensar em contrato e validação.

## Critérios para avançar

- [ ] Consegue modelar um domínio simples definindo campos, tipos e validações antes de escrever qualquer código.
- [ ] Entende a diferença entre validar em tempo de execução (o que o Python faz) e o que seria validar em tempo de compilação (conceito que vai reaparecer no Módulo 07, com TypeScript).
- [ ] A biblioteca de validação cobre pelo menos 4 regras.

## Como a IA deve ajudar neste módulo

- Este é o primeiro momento em que vale começar a citar, informalmente, a ideia de "pensar antes de codar" — sem ainda introduzir os artefatos formais de Spec-Driven Development.
- Revisar os modelos de dados do aluno antes de qualquer implementação.

## Como a IA NÃO deve ajudar neste módulo

- Não modele o domínio inteiro pelo aluno — proponha perguntas sobre os campos antes de aceitar o modelo como pronto.
- Ainda não introduza os artefatos formais `spec.md`/`plan.md` — isso é reservado para módulos mais avançados.
