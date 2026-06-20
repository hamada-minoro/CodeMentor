---
name: spec-driven-feature
description: Conduz o fluxo de criação de uma feature usando spec.md, plan.md, tasks.md, tests.md e review.md. Use quando o aluno pedir para criar ou evoluir uma feature em um projeto maior (Módulo 08 em diante).
---

# Skill: Spec-Driven Feature

## Processo obrigatório

1. Ler `CLAUDE.md` e `docs/GUIA_SPEC_DRIVEN_DEVELOPER.md`.
2. Ler a pasta da feature em `docs/specs/` (ou `exemplos-projetos/.../docs/specs/`, conforme o contexto).
3. Se não existir `spec.md`, criar uma proposta usando `.tutor/templates/template-spec.md` — não implementar nada antes disso existir.
4. Se já existir `spec.md`, verificar ambiguidades antes de seguir.
5. Criar ou revisar `plan.md` usando `.tutor/templates/template-plan.md`.
6. Criar ou revisar `tasks.md` usando `.tutor/templates/template-tasks.md`.
7. Implementar uma task por vez.
8. Rodar testes após cada bloco relevante de implementação.
9. Atualizar `review.md` (usando `.tutor/templates/template-review.md`) com pendências e decisões.
10. Não alterar o escopo sem registrar a mudança explicitamente no próprio `spec.md`.

## Saída esperada

- Resumo do que foi feito.
- Arquivos alterados.
- Testes executados.
- Riscos restantes.
- Próximos passos.
