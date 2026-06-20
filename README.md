# CodeMentor BR

#### *Dica inicial, quando no vs code, abra esse arquivo apertando com o botão direito em cima dele e escolhendo a opção 'Abrir Visualização', sua leitura será mais prazerosa dessa forma.

**Aprenda programação com apoio de IA, sem virar dependente dela.**

Estudar programação com IA pode acelerar muito o aprendizado, mas também pode criar um problema: o aluno copia respostas, pula fundamentos e chega em projetos maiores sem saber explicar, corrigir ou avaliar o próprio código.

O **CodeMentor BR** transforma a IA do seu editor em um tutor: ela explica, gera exercícios, revisa suas respostas, dá nota com critério e só então sugere o próximo passo — mas nunca entrega a solução antes da sua tentativa.

> Este projeto não te ensina a pedir código pronto para a IA. Ele te ensina a aprender programação com IA e, depois, a usar IA como um desenvolvedor de verdade.

---

## Prompt inicial — como começar

Cole um dos dois prompts abaixo na sua IA (GitHub Copilot, Claude Code, etc.).

### Opção 1 — Nunca programei (ou quero começar do zero)

```txt
Estou começando a estudar programação. Leia com atenção este projeto, começando pelo
README.md. Vou começar pelo Módulo 00, Aula 1. Faça o necessário para eu começar e crie
um arquivo Markdown prático com um passo a passo resumido de como estudar.
```

### Opção 2 — Já tenho alguma base em programação

```txt
Já tenho experiência básica em programação. Antes de começar, aplique o questionário de
nivelamento deste projeto para descobrir em qual módulo do roadmap eu devo começar,
registre o resultado no meu progresso e inicie o módulo indicado.
```

---

## Documentação

Depois deste README, leia os guias em `docs/` nesta ordem:

| Ordem | Arquivo | O que explica |
|---|---|---|
| 1 | [docs/COMO_USAR_O_TUTOR.md](docs/COMO_USAR_O_TUTOR.md) | O ciclo prático do dia a dia: iniciar aula, estudar, resolver, pedir revisão, avançar. |
| 2 | [docs/ROADMAP.md](docs/ROADMAP.md) | Os 14 módulos do currículo, em ordem, e o que esperar de cada um. |
| 3 | [docs/SETUP_VSCODE_IA.md](docs/SETUP_VSCODE_IA.md) | Como configurar o VS Code e qual IA usar (gratuita ou paga). |
| 4 | [docs/GUIA_DO_ESTUDANTE.md](docs/GUIA_DO_ESTUDANTE.md) | Onde colocar arquivos, como interpretar notas, dicas gerais. |
| 5 | [docs/GUIA_SPEC_DRIVEN_DEVELOPER.md](docs/GUIA_SPEC_DRIVEN_DEVELOPER.md) | Como trabalhar com `spec.md`/`plan.md`/`tasks.md` (a partir do Módulo 07~08). |

Os arquivos internos que orientam a própria IA estão em `.tutor/` — você não precisa editá-los para estudar.

---

## Para quem é este projeto?

- Estudantes que estão começando em programação ou já têm alguma base.
- Pessoas que querem aprender com IA, mas sem pular fundamentos.
- Professores, mentores ou familiares que querem orientar alguém no estudo de programação.

## Como funciona o ciclo de estudo

Cada aula do roadmap segue o mesmo ciclo: **a IA explica → gera exercícios → você tenta sozinho → a IA revisa sem entregar tudo de imediato → você corrige → recebe nota e feedback → consolida → só então avança.** Esse ciclo evita o uso passivo da IA. Veja o passo a passo completo em [docs/COMO_USAR_O_TUTOR.md](docs/COMO_USAR_O_TUTOR.md).

---

## Roadmap de aprendizado (resumo)

**Python primeiro, sempre.** Dos Módulos 00 a 06, todo o conteúdo é só em Python. TypeScript e Node.js entram como módulo dedicado a partir do **Módulo 07** — incluindo como criar um projeto Node do zero e automatizar o scaffold de uma API com IA via `spec.md`.

| Módulo | Tema |
|---|---|
| 00 | Ambiente, terminal e Git |
| 01 | Lógica de programação (Python) |
| 02 | Fundamentos de Python |
| 03 | Tipagem e modelagem de dados (Python) |
| 04 | Paradigmas de programação (Python) |
| 05 | Orientação a objetos (Python) |
| 06 | Estruturas de dados, algoritmos e Big O (Python) |
| 07 | Node.js e TypeScript profissional |
| 08 | Backend (Node/TypeScript + Python) |
| 09 | Banco de dados |
| 10 | Testes e qualidade |
| 11 | Arquitetura de software |
| 12 | IA profissional e Spec-Driven Development |
| 13 | Portfólio |

Detalhe completo de cada módulo (aulas, exercícios, critérios para avançar) em [docs/ROADMAP.md](docs/ROADMAP.md) e [.tutor/curriculo/mapa-geral.md](.tutor/curriculo/mapa-geral.md).

---

## Estrutura do repositório

```txt
CodeMentor/
├── README.md            ← você está aqui
├── CLAUDE.md             ← instruções para a IA (Claude Code)
├── docs/                 ← guias práticos (leia na ordem da seção "Documentação")
├── .tutor/               ← regras, currículo, templates e rubricas que a IA usa
├── .claude/              ← skills e agents
├── estudos/              ← onde a IA cria cada módulo/aula conforme você avança
├── progresso/            ← diário de aprendizado e mapa de progresso
└── exemplos-projetos/    ← referências de projetos de portfólio
```

Cada aula segue o padrão `estudos/modulo-XX-nome/aula-YY-nome/`, com `README.md`, `exercicios.md`, `minhas-respostas/`, `revisao.md`, `nota.md`, `consolidacao.md` e `diario.md`.

---

## Como começar

1. Instale o [VS Code](https://code.visualstudio.com/) e o [Git](https://git-scm.com/), e clone este repositório.
2. Abra a pasta no VS Code (`code .`).
3. Configure sua IA seguindo [docs/SETUP_VSCODE_IA.md](docs/SETUP_VSCODE_IA.md) (GitHub Copilot Free para começar, ou Claude Pro + Claude Code se quiser investir).
4. Cole um dos prompts da seção "Prompt inicial" acima.

---

## Filosofia do projeto

Um estudante que aprende apenas copiando código gerado por IA terá dificuldade quando precisar corrigir bugs, entender erros, adaptar soluções ou explicar decisões técnicas. Por isso:

> Use IA para acelerar o aprendizado, mas não para fugir do raciocínio.

Isso não é um curso milagroso, nem um gerador de código pronto, nem uma promessa de emprego rápido — é um método para estudar programação com organização, registrar progresso e usar IA como ferramenta profissional, não como atalho.

---

## Contribuições

Contribuições são bem-vindas: novos exercícios, melhorias no roadmap, rubricas, exemplos de projetos, correções de texto, adaptações para diferentes níveis de aluno.

## Licença

```txt
MIT License
```
