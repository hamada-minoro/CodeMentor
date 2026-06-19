# CodeMentor BR — Roadmap de Programação dos Fundamentos até o Spec-Driven Development

Um repositório educacional open source para aprender programação do zero com apoio de IA — sem cair em "vibe coding".

## 1. O que é este projeto

Este repositório é um **tutor de programação guiado por IA**. Ele não ensina sozinho: ele organiza o caminho, gera exercícios, revisa suas respostas e te acompanha do primeiro "Olá, mundo" até você conseguir planejar e conduzir uma IA para construir software de verdade.

A trilha principal usa **Node.js com TypeScript** e **Python**, e termina te apresentando ao **Spec-Driven Development** — o jeito profissional de trabalhar com IA: especificar antes de codar.

## 2. Para quem é este repositório

- Para quem está começando em programação do zero ou quase do zero.
- Para quem já tentou estudar sozinho e se perdeu entre tutoriais soltos.
- Para quem usa (ou quer usar) IA para estudar, mas não sabe como evitar virar dependente dela.
- Para quem tem acesso a no mínimo uma IA dentro do VS Code: GitHub Copilot Free, Claude Code/Claude Pro, ou um modelo local via Ollama.

Não é para quem busca um curso de "programação em 3 meses" ou um gerador automático de projetos prontos.

## 3. O que você vai aprender

- Lógica de programação e pensamento computacional.
- Fundamentos de TypeScript e Python, em paralelo.
- Tipagem, modelagem de dados e paradigmas de programação.
- Orientação a objetos sem exagero.
- Estruturas de dados, algoritmos e noções de Big O.
- Backend com Node.js/TypeScript e Python (FastAPI).
- Banco de dados relacional, testes e arquitetura de software.
- Como usar IA como tutor, revisor e, por fim, executora supervisionada de um plano — o modelo **Spec-Driven Developer**.

Veja o detalhamento completo em [ROADMAP.md](ROADMAP.md).

## 4. As duas teses centrais

**Fundamentos antes de frameworks.** Frameworks mudam a cada poucos anos. Lógica, tipos, estrutura de dados, testes e arquitetura permanecem. Por isso este repositório força você a entender o "porquê" antes de te deixar usar atalhos.

**IA como tutor, não como muleta.** Em todas as fases iniciais, a IA aqui é instruída a te explicar, te questionar e te revisar — não a resolver exercícios por você. Só depois que você tiver base, o repositório te ensina a usar IA como acelerador profissional, dentro de um fluxo de especificação, planejamento e revisão.

## 5. Por onde começar (sem se perder na quantidade de pastas)

Você vai ver várias pastas neste repositório. A maioria delas é **infraestrutura para a IA funcionar como tutor** — você não precisa abrir nem entender essas pastas para estudar. São elas:

- `.tutor/` — instruções que qualquer IA lê para saber como te ensinar. Você não edita isso.
- `.claude/` — agents e skills específicos para quem usa Claude Code. Você não edita isso.

As pastas que você de fato vai usar no dia a dia são:

| Pasta | Para que serve |
|---|---|
| `estudos/` | Onde a IA cria cada tópico do roadmap, com teoria e exercícios |
| `workspace-aluno/` | Seu espaço livre para testar código em Python e TypeScript |
| `progresso/` | Seu diário de aprendizado e mapa de progresso |
| `exemplos-projetos/` | Projetos de referência, incluindo um exemplo de Spec-Driven Development |

Se a quantidade de arquivos parecer assustadora no começo, relaxe: você só precisa interagir com as quatro pastas acima. O resto existe para a IA, não para você decorar.

## 6. Como começar

### 6.1. Clonar o repositório

```bash
git clone <url-do-seu-fork-ou-repo>
cd codementor-br
```

### 6.2. Abrir no VS Code

```bash
code .
```

Veja o guia completo de configuração em [SETUP_VSCODE_IA.md](SETUP_VSCODE_IA.md), que cobre três caminhos:

- **Caminho A** — Gratuito: VS Code + GitHub Copilot Free.
- **Caminho B** — Pago: Claude Pro + Claude Code.
- **Caminho C** — IA local: Ollama + Continue (ou similar).

### 6.3. Iniciar seu primeiro tópico

Com a IA escolhida aberta no VS Code, peça:

```text
Leia `CLAUDE.md` e `.tutor/tutor-manifest.md`.
Quero iniciar o tópico "variáveis, entrada, processamento e saída" da Fase 1.
Crie a pasta de estudo, explique o conteúdo e gere exercícios sem gabarito.
```

A IA vai criar uma pasta em `estudos/fase-01-logica/...` com tudo que você precisa para estudar aquele tópico.

### 6.4. Resolver os exercícios

Resolva manualmente, em Python e/ou TypeScript, colocando seus arquivos dentro de `minhas-respostas/`. Tente sem IA primeiro. Se travar, use a IA para te explicar — não para resolver por você. Veja os prompts recomendados em [GUIA_DO_ESTUDANTE.md](GUIA_DO_ESTUDANTE.md).

### 6.5. Pedir revisão

```text
Revise minhas respostas em
estudos/fase-01-logica/topico-01-variaveis-entrada-processamento-saida/minhas-respostas/.
Use a rubrica, aponte erros, dê nota e crie um exercício de consolidação.
```

A IA vai escrever `revisao.md` e `nota.md` dentro da pasta do tópico, e vai te propor um exercício extra em `consolidacao.md` caso você precise reforçar algo.

### 6.6. Avançar

```text
Leia progresso/mapa-de-progresso.md e minhas últimas avaliações.
Diga se estou pronto para avançar e sugira o próximo tópico.
```

A IA nunca avança automaticamente por você — você decide quando seguir.

## 7. Estudando Python e TypeScript em paralelo

Sempre que um tópico permitir, resolva o mesmo exercício nas duas linguagens. Isso te ajuda a separar "conceito de programação" de "sintaxe de uma linguagem específica" — uma das habilidades mais valiosas para trabalhar bem com IA depois.

## 8. Registrando seu progresso

Depois de cada revisão, vale a pena anotar em `progresso/diario-de-aprendizado.md` o que você aprendeu, o que travou e o que te surpreendeu. Esse diário também ajuda a IA a te dar contexto melhor nas próximas sessões.

## 9. Exemplos de prompts prontos

Você encontra uma lista completa em [.tutor/prompts/](. tutor/prompts/README.md), mas os mais usados no dia a dia são:

```text
Estou estudando [CONCEITO]. Explique de forma simples, com analogia e exemplo pequeno.
Não resolva meus exercícios. Ao final, faça 3 perguntas para testar meu entendimento.
```

```text
Estou com este erro: [COLE_O_ERRO]
Não corrija diretamente. Explique o que significa, as causas prováveis e o que verificar, uma coisa por vez.
```

## 10. Aviso honesto sobre ferramentas

Este repositório não depende de uma ferramenta de IA específica. Ele foi desenhado para funcionar com qualquer IA capaz de ler os arquivos em `.tutor/`.

Preços, limites de uso e disponibilidade de planos gratuitos ou pagos (GitHub Copilot Free, Claude Pro, Ollama, etc.) mudam com frequência. Antes de decidir qual caminho seguir, consulte sempre a documentação oficial de cada ferramenta — não confie apenas no que está escrito aqui.

Links de referência:

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

## 11. Licença e contribuição

Este projeto é educacional e aberto a contribuições. Antes de abrir um PR, revise se sua mudança preserva a tese central: fundamentos primeiro, IA como tutor antes de IA como acelerador. Sugestões de novos tópicos, exercícios e correções de conteúdo são bem-vindas via issues ou pull requests.
