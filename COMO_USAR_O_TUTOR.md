# Como Usar o Tutor

Este guia explica, na prática, como interagir com a IA tutora deste repositório no dia a dia.

## O ciclo básico

```text
1. Iniciar tópico  →  2. Estudar  →  3. Resolver exercícios  →  4. Pedir revisão  →  5. Receber nota
   →  6. Fazer consolidação (se necessário)  →  7. Avançar
```

Esse ciclo está detalhado em `.tutor/fluxo-de-estudo.md`. Aqui vai a versão prática, com os comandos que você realmente vai digitar.

## 1. Iniciar um tópico

```text
Iniciar tópico "condicionais" da Fase 1.
```

Ou, se sua IA suportar skills do Claude Code:

```text
/iniciar-topico condicionais, Fase 1
```

A IA vai criar `estudos/fase-01-logica/topico-02-condicionais/` com tudo que você precisa.

## 2. Estudar

Leia o `README.md` daquele tópico. Não tenha pressa — releia se precisar, peça analogias diferentes se uma explicação não fizer sentido.

## 3. Resolver exercícios

Abra `exercicios.md` e resolva sem IA gerando a solução. Coloque os arquivos em `minhas-respostas/python/` e/ou `minhas-respostas/typescript/`.

Se travar, use prompts como:

```text
Estou estudando [CONCEITO]. Não resolva meus exercícios.
Me explique de outra forma e faça 3 perguntas para eu testar meu entendimento.
```

## 4. Pedir revisão

```text
Revise minhas respostas em estudos/fase-01-logica/topico-02-condicionais/minhas-respostas/.
```

Ou:

```text
/revisar-exercicios estudos/fase-01-logica/topico-02-condicionais/
```

## 5. Receber nota

A IA vai escrever `nota.md` usando a rubrica de `.tutor/rubricas/rubrica-codigo.md`. Leia a justificativa, não só o número.

## 6. Fazer consolidação (se necessário)

Se a nota indicar lacunas, a IA cria `consolidacao.md` com um exercício focado nos seus erros. Resolva antes de avançar.

## 7. Avançar

```text
Leia progresso/mapa-de-progresso.md. Estou pronto para avançar?
```

A decisão final de avançar é sua — a IA só recomenda.

## Dicas gerais

- Não tenha vergonha de errar. O erro é parte do método deste repositório.
- Sempre que puder, registre o que aprendeu em `progresso/diario-de-aprendizado.md`.
- Se sentir que a IA está te dando a resposta cedo demais, lembre ela das regras em `.tutor/regras-de-comportamento-da-ia.md` — cole o link do arquivo no chat.
