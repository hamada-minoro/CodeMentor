# `.claude/`

Esta pasta contém configuração específica do Claude Code: agents e skills. **Você, estudante, não precisa editar nada aqui.**

A lógica pedagógica em si vive em `.tutor/` (agnóstica de ferramenta). Esta pasta apenas conecta essa lógica às convenções do Claude Code — agents especializados e skills reutilizáveis.

## Estrutura

- `agents/` — agentes especializados (tutor, designer de currículo, gerador de exercícios, revisor, avaliador, coach de spec-driven, mantenedor de documentação).
- `skills/` — procedimentos reutilizáveis que implementam o ciclo de estudo descrito em `.tutor/fluxo-de-estudo.md`.
- `settings.example.json` — exemplo de configuração. Copie para `settings.json` e ajuste se necessário; `settings.json` não deve ser versionado se contiver dados pessoais.

## Para saber mais

- Claude Code Skills: https://docs.anthropic.com/en/docs/claude-code/skills
- Claude Code Subagents: https://docs.anthropic.com/en/docs/claude-code/sub-agents
