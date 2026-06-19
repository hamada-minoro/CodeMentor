# Fase 11 — IA profissional e Spec-Driven Development

**Duração sugerida:** começa em paralelo a partir da Fase 03 (informalmente) e vira prática central após a Fase 07; esta fase formaliza o fluxo completo.

## Objetivo da fase

Sair do "vibe coding" e aprender a trabalhar com especificação, plano, tarefas, testes e revisão antes de qualquer implementação — o modelo Spec-Driven Developer.

## Pré-requisitos

Fases 00 a 10 concluídas. Esta fase assume que o aluno já sabe construir uma API com banco, testes e arquitetura em camadas.

## Tópicos e ordem sugerida

1. O que é vibe coding e por que é perigoso para iniciantes (e até para experientes, em projetos sérios).
2. O que é Spec-Driven Development.
3. Os artefatos: `spec.md`, `plan.md`, `tasks.md`, `tests.md`, `review.md`.
4. Como escrever uma spec com critérios de aceitação claros.
5. Como quebrar uma feature em tarefas pequenas e verificáveis.
6. Como conduzir uma IA para implementar uma task por vez.
7. Como revisar código gerado por IA com critério (bloqueante, importante, melhoria, dúvida).
8. Subagents e skills no Claude Code, e como usar agentes especializados (arquiteto, revisor, etc.).

Veja o guia completo em `GUIA_SPEC_DRIVEN_DEVELOPER.md`.

## Atividades / exercícios esperados

Escolher uma feature nova para o projeto financeiro das fases anteriores (ex.: metas de economia, notificação de gastos). Antes de implementar:

1. Escrever `spec.md` com contexto, objetivo, regras de negócio, fluxos e critérios de aceitação.
2. Escrever `plan.md` com a abordagem técnica.
3. Escrever `tasks.md` quebrando a implementação em etapas pequenas.
4. Implementar uma task por vez, com a IA, revisando cada etapa.
5. Escrever `tests.md` e os testes correspondentes.
6. Fechar com `review.md`, registrando pendências e decisões.

## Critérios para avançar

- [ ] A spec da feature tem critérios de aceitação verificáveis (formato "dado X, quando Y, então Z").
- [ ] A implementação foi feita task por task, com revisão entre etapas — não tudo de uma vez.
- [ ] O aluno revisou o código gerado pela IA e conseguiu apontar pelo menos um problema ou melhoria antes de aceitar.

## Como a IA deve ajudar nesta fase

- Atuar como executora supervisionada de um plano claro — não como geradora de código a partir de um pedido vago.
- Validar se a spec tem ambiguidades antes de qualquer implementação.
- Implementar uma task por vez, explicando arquivos alterados após cada etapa.
- Usar a skill `spec-driven-feature` para conduzir esse fluxo.

## Como a IA NÃO deve ajudar nesta fase

- Não implemente a feature inteira de uma vez, mesmo que a spec esteja completa — task por task, sempre.
- Não altere o escopo da spec sem registrar a mudança explicitamente no próprio `spec.md`.
- Não aceite "crie um sistema de X completo" como pedido válido — sempre direcione o aluno a escrever a spec primeiro.
