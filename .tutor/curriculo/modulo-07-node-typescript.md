# Módulo 07 — Node.js e TypeScript profissional

**Duração sugerida:** 4 a 6 semanas (8 aulas)

## Objetivo do módulo

Este é o primeiro módulo em que o aluno toca em uma segunda linguagem de propósito geral. Até aqui, tudo foi em Python — lógica, fundamentos, tipagem, paradigmas, OO, estruturas de dados. Agora o aluno já sabe pensar como programador; este módulo ensina a sintaxe e o ecossistema de Node.js + TypeScript, **e como usar IA para automatizar a criação de um projeto base de API, descrevendo bem o que se quer em um `spec.md`** — em vez de copiar comandos de tutorial sem entender.

## Pré-requisitos

Módulo 06 concluído. O aluno já entende variáveis, funções, condicionais, laços, OO, paradigmas e estruturas de dados — em Python. Este módulo assume essa base e foca no que é específico de Node/TypeScript.

## Aulas

### Aula 1 — Por que TypeScript, e o que muda vindo do Python

Tipagem estática vs. dinâmica na prática, compilação vs. interpretação, o papel do Node.js como runtime de JavaScript fora do navegador.

### Aula 2 — Criar um projeto Node do zero

`npm init`, entender o `package.json`, instalar o `typescript` como dependência de desenvolvimento, configurar o `tsconfig.json` (manualmente, lendo cada opção — sem copiar um arquivo pronto sem entender).

### Aula 3 — Sintaxe básica de TypeScript

`let`/`const`, tipos primitivos, arrays, objetos, funções, parâmetros opcionais, retorno de função.

### Aula 4 — Tipos mais avançados

Interfaces, type aliases, enums, union types, generics básicos.

### Aula 5 — Módulos (import/export) e assincronia

`import`/`export`, `async`/`await`, `try`/`catch`, comparando com `asyncio` do Python. (Aqui "módulo" é o termo da linguagem para um arquivo importável — não confundir com este Módulo 07 do roadmap.)

### Aula 6 — Scripts npm e ferramentas de qualidade

Scripts no `package.json` (`build`, `dev`, `start`), ESLint, Prettier — e por que isso importa para qualquer projeto, não só para IA.

### Aula 7 — Comparando com o que o aluno já sabe

Reimplementar em TypeScript um exercício pequeno que o aluno já fez em Python (ex.: o gerenciador de tarefas do Módulo 02), comparando explicitamente as diferenças de sintaxe e de filosofia entre as duas linguagens.

### Aula 8 — Automatizando o scaffold de um projeto com IA via `spec.md`

O foco prático deste módulo: em vez de pedir à IA "cria um projeto Node com TypeScript", o aluno escreve um `spec.md` descrevendo exatamente o que quer (estrutura de pastas, dependências, scripts, padrão de código), pede para a IA revisar a spec antes de qualquer comando, e só então deixa a IA gerar o scaffold inicial de uma API base (sem rotas de negócio ainda — isso é assunto do Módulo 08).

## Exemplo de `spec.md` para a Aula 8

```markdown
# Spec — Scaffold de API Node + TypeScript

## Objetivo
Criar a base de um projeto de API HTTP em Node.js com TypeScript, sem nenhuma rota de negócio ainda.

## Dependências
- typescript, @types/node (dev)
- framework HTTP: a definir (ex.: Express ou Fastify) — justificar a escolha antes de instalar
- eslint, prettier (dev)

## Estrutura de pastas esperada
src/
  index.ts
  config/
  routes/
  shared/
package.json
tsconfig.json
.eslintrc / eslint.config.js
README.md

## Scripts npm esperados
- dev: roda em modo desenvolvimento com reload
- build: compila TypeScript para JavaScript
- start: roda a versão compilada

## Critérios de aceitação
- Dado que o projeto foi gerado, quando eu rodo `npm run dev`, então o servidor sobe e responde em uma rota de health-check (`GET /health`).
- O `tsconfig.json` tem `strict: true`.
- Nenhuma rota de negócio foi criada além do health-check.
```

## Atividades / exercícios esperados

1. Criar manualmente (sem IA) um projeto Node + TypeScript mínimo, só para sentir o processo: `npm init`, instalar TypeScript, configurar `tsconfig.json`, escrever um `index.ts` que compila e roda.
2. Escrever o `spec.md` do scaffold da API (modelo acima), revisar com a IA antes de gerar qualquer código, e então pedir para a IA aplicar o scaffold a partir da spec.
3. Comparar: o que demorou mais, fazer manualmente ou descrever bem a spec? O que a spec evitou que desse errado?

## Critérios para avançar

- [ ] Criou um projeto Node + TypeScript manualmente, sem IA, pelo menos uma vez.
- [ ] Escreveu um `spec.md` com critérios de aceitação verificáveis antes de pedir o scaffold para a IA.
- [ ] O scaffold gerado a partir da spec atende exatamente aos critérios de aceitação descritos — nem mais, nem menos.
- [ ] Consegue explicar a diferença entre tipagem dinâmica (Python) e estática (TypeScript) com suas próprias palavras.

## Como a IA deve ajudar neste módulo

- Explicar sintaxe e conceitos de TypeScript/Node sob demanda, comparando sempre com o que o aluno já sabe em Python.
- Revisar o `spec.md` do aluno antes de gerar qualquer scaffold, apontando ambiguidades (ex.: "qual framework HTTP? por quê?").
- Gerar o scaffold automatizado **somente** depois que a spec estiver clara e revisada — e só o que a spec descreve, nada além disso.

## Como a IA NÃO deve ajudar neste módulo

- Não gere um projeto Node + TypeScript completo a partir de um pedido vago ("cria um projeto Node aí") sem uma spec por escrito.
- Não pule o exercício manual da Aula 2 — o aluno precisa sentir o processo de configurar um projeto do zero antes de automatizá-lo.
- Não adicione rotas de negócio, banco de dados ou autenticação no scaffold deste módulo — isso é assunto do Módulo 08 (Backend).
