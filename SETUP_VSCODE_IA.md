# Setup do VS Code com IA

> Preços, limites e disponibilidade de planos mudam com frequência. As informações abaixo são um guia geral — consulte sempre a documentação oficial de cada ferramenta antes de decidir.

Existem três caminhos possíveis para usar este repositório. Escolha o que faz sentido para você agora; você pode trocar de caminho depois sem perder nada, porque o tutor (`.tutor/`) é o mesmo para qualquer IA.

## Caminho A — Gratuito: VS Code + GitHub Copilot Free

### Passo a passo

1. Instale o [VS Code](https://code.visualstudio.com/).
2. Instale o [Git](https://git-scm.com/).
3. Crie uma conta no [GitHub](https://github.com/).
4. Na aba de extensões do VS Code, procure por "GitHub Copilot" e instale.
5. Faça login com sua conta do GitHub.
6. Abra o chat do Copilot e use-o com moderação — como apoio para entender conceitos, não como executor automático de exercícios.
7. O plano gratuito do GitHub Copilot tem limites de uso que podem mudar. Consulte a [documentação oficial do GitHub Copilot](https://docs.github.com/en/copilot) antes de planejar sua rotina de estudo em torno dele.

### Prompts recomendados para Copilot Free

```text
Leia .tutor/tutor-manifest.md e me ajude a estudar o tópico X sem resolver por mim.
```

```text
Explique meu erro neste código, mas não reescreva a solução completa.
```

```text
Crie 3 perguntas para testar se eu entendi este conceito.
```

```text
Revise minha explicação antes de revisar meu código.
```

## Caminho B — Pago: Claude Pro + Claude Code no VS Code

### Passo a passo

1. O Claude Pro inclui acesso ao Claude Code, mas preços, limites e disponibilidade podem mudar — consulte [claude.com/pricing](https://claude.com/pricing).
2. Instale a extensão [Claude Code](https://docs.anthropic.com/en/docs/claude-code) no VS Code, ou via terminal conforme a [documentação de integração com IDEs](https://docs.anthropic.com/en/docs/claude-code/ide-integrations).
3. Abra o projeto pelo terminal com `code .` na raiz do repositório, para o VS Code herdar as variáveis de ambiente.
4. Faça login com sua conta.
5. Peça ao Claude para ler `CLAUDE.md` e `.tutor/tutor-manifest.md` antes de qualquer interação de estudo.
6. Use as skills do projeto (veja [docs/skills](https://docs.anthropic.com/en/docs/claude-code/skills)) como `/iniciar-topico`, `/revisar-exercicios` e `/avancar-roadmap` quando disponíveis no seu ambiente.

### Prompts recomendados para Claude Code

```text
Leia CLAUDE.md e .tutor/tutor-manifest.md. Quero iniciar o tópico "variáveis" da Fase 1.
Crie a estrutura de estudo seguindo o fluxo do tutor.
```

```text
Use a skill iniciar-topico para criar o tópico "condicionais" da Fase 1.
```

```text
Use a skill revisar-exercicios para revisar minhas respostas em
estudos/fase-01-logica/topico-02-condicionais/minhas-respostas/.
```

## Caminho C — IA local: Ollama + Continue (ou similar)

### Passo a passo

1. Instale o [Ollama](https://ollama.com/) e baixe um modelo compatível com seu hardware.
2. Instale a extensão [Continue](https://www.continue.dev/) no VS Code (ou outra extensão equivalente de IA local que você prefira).
3. Configure a extensão para usar o modelo local rodando no Ollama.
4. Modelos locais podem ter qualidade inferior a modelos pagos, principalmente em raciocínio mais longo. Ajuste suas expectativas e prefira prompts menores e objetivos.
5. Sempre dê contexto explícito apontando para `.tutor/tutor-manifest.md`, já que IAs locais geralmente não leem o repositório sozinhas como o Claude Code faz.
6. Mantenha os arquivos de estudo organizados — isso facilita colar o conteúdo certo no contexto de um modelo com janela de contexto menor.

### Prompt recomendado para IA local

```text
Você é meu tutor de programação. Leia o arquivo .tutor/tutor-manifest.md e o arquivo
da fase em .tutor/curriculo/. Não resolva exercícios por mim. Me explique o tópico X,
crie exercícios e depois revise minhas respostas.
```

## Qual caminho escolher?

Não existe caminho "certo". O importante é manter consistência. Se seu acesso a ferramentas pagas mudar no futuro, o repositório continua funcionando do mesmo jeito — porque a lógica de tutoria vive em `.tutor/`, não em uma ferramenta específica.

## Referências oficiais

- VS Code: https://code.visualstudio.com/
- Git: https://git-scm.com/
- Node.js: https://nodejs.org/
- Python: https://www.python.org/
- TypeScript: https://www.typescriptlang.org/docs/
- GitHub Copilot: https://docs.github.com/en/copilot
- Claude Code: https://docs.anthropic.com/en/docs/claude-code
- Claude Code no VS Code: https://docs.anthropic.com/en/docs/claude-code/ide-integrations
- Claude Code Skills: https://docs.anthropic.com/en/docs/claude-code/skills
- Claude Code Subagents: https://docs.anthropic.com/en/docs/claude-code/sub-agents
- Claude Pricing: https://claude.com/pricing
- Ollama: https://ollama.com/
- Continue: https://www.continue.dev/
