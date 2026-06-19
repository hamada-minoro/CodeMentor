# Fase 03 — Tipagem e modelagem de dados

**Duração sugerida:** 3 a 4 semanas

## Objetivo da fase

Entender contratos, tipos e estruturas de dados — uma das bases mais importantes para trabalhar bem com IA depois, já que descrever bem os tipos reduz ambiguidade.

## Pré-requisitos

Fase 02 concluída.

## Tópicos e ordem sugerida

Tipagem dinâmica, tipagem estática, inferência de tipos, contratos, DTOs, entidades, validação, serialização, tipos opcionais, tipos nulos, imutabilidade, schema de dados.

## Atividades / exercícios esperados

Modelar os mesmos domínios em TypeScript e Python: usuário, produto, pedido, pagamento, tarefa, funcionário, equipamento, agendamento. Para cada domínio, definir campos obrigatórios, campos opcionais, regras de validação, estados possíveis, exemplos válidos e exemplos inválidos.

Projeto da fase: pequena biblioteca de validação de dados (e-mail válido, CPF com tamanho correto, senha forte, data futura, número positivo, string obrigatória). Não precisa ser perfeita — o objetivo é pensar em contrato e validação.

## Critérios para avançar

- [ ] Consegue modelar um domínio simples definindo campos, tipos e validações antes de escrever qualquer código.
- [ ] Entende a diferença entre validação em tempo de compilação (TypeScript) e em tempo de execução (Python).
- [ ] A biblioteca de validação cobre pelo menos 4 regras.

## Como a IA deve ajudar nesta fase

- Apresentar este é o primeiro momento em que vale começar a citar, informalmente, a ideia de "pensar antes de codar" — sem ainda introduzir os artefatos formais de Spec-Driven Development.
- Revisar os modelos de dados do aluno antes de qualquer implementação.

## Como a IA NÃO deve ajudar nesta fase

- Não modele o domínio inteiro pelo aluno — proponha perguntas sobre os campos antes de aceitar o modelo como pronto.
- Ainda não introduza os artefatos formais `spec.md`/`plan.md` — isso é reservado para fases mais avançadas.
