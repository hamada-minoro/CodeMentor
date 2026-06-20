# Setup do VS Code com IA

> Preços, limites e disponibilidade de planos mudam com frequência. Consulte sempre a documentação oficial de cada ferramenta antes de decidir.

Existem dois caminhos para usar este repositório. Comece pelo gratuito; você pode migrar para o pago depois sem perder nada, porque o tutor (`.tutor/`) é o mesmo para qualquer IA.

## Extensões recomendadas do VS Code

Instale estas extensões antes de começar, independente do caminho escolhido:

- **GitHub Copilot** (ou **Claude Code**, se for pelo Caminho B) — a IA tutora.
- **Python** (Microsoft) — suporte e execução de código Python.
- **Pylance** — autocomplete e checagem de tipos para Python.
- **ESLint** — linting para TypeScript/JavaScript (a partir do Módulo 07).
- **Prettier** — formatação automática de código.
- **GitLens** — visualizar histórico e autoria do Git direto no editor.

## Caminho A — Gratuito: VS Code + GitHub Copilot Free

1. Instale o [VS Code](https://code.visualstudio.com/), o [Git](https://git-scm.com/) e crie uma conta no [GitHub](https://github.com/).
2. Na aba de extensões, instale "GitHub Copilot" e faça login com sua conta do GitHub.
3. Use o chat do Copilot com moderação — como apoio para entender conceitos, não como executor automático de exercícios.
4. O plano gratuito tem limites de uso que podem mudar — consulte a [documentação oficial](https://docs.github.com/en/copilot).

### Prompts recomendados

```text
Leia .tutor/tutor-manifest.md e me ajude a estudar a aula X sem resolver por mim.
```

```text
Explique meu erro neste código, mas não reescreva a solução completa.
```

## Caminho B — Pago: Claude Pro + extensão Claude Code no VS Code

Se quiser investir, este caminho dá acesso a skills e fluxo de tutoria mais automatizado.

1. O Claude Pro inclui acesso ao Claude Code — preços e limites podem mudar, consulte [claude.com/pricing](https://claude.com/pricing).
2. Instale a extensão **Claude Code** no VS Code (veja a [documentação de integração com IDEs](https://docs.anthropic.com/en/docs/claude-code/ide-integrations)).
3. Abra o projeto pelo terminal com `code .` na raiz do repositório, e faça login.
4. Peça para a IA ler `CLAUDE.md` e `.tutor/tutor-manifest.md` antes de qualquer interação de estudo.

### Prompts recomendados

```text
Leia CLAUDE.md e .tutor/tutor-manifest.md. Quero iniciar a aula "variáveis" do Módulo 1.
```

```text
Use a skill iniciar-aula para criar a aula "condicionais" do Módulo 1.
```

## Referências oficiais

- VS Code: https://code.visualstudio.com/
- Git: https://git-scm.com/
- Node.js: https://nodejs.org/
- Python: https://www.python.org/
- GitHub Copilot: https://docs.github.com/en/copilot
- Claude Code: https://docs.anthropic.com/en/docs/claude-code
- Claude Code no VS Code: https://docs.anthropic.com/en/docs/claude-code/ide-integrations
- Claude Pricing: https://claude.com/pricing
