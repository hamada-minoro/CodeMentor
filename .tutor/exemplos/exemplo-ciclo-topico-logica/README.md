# Variáveis, Entrada, Processamento e Saída

**Fase:** 1 — Lógica e pensamento computacional
**Tópico:** 01

## Objetivo de aprendizado

Entender como um programa recebe dados, guarda esses dados em variáveis, processa essas informações e devolve um resultado.

## Explicação

Todo programa, no fundo, faz três coisas: **recebe** algo, **transforma** esse algo e **devolve** um resultado. Uma variável é só uma "caixa com nome" onde você guarda um valor para usar depois.

## Pseudocódigo

```text
ler nome
ler idade
idade_em_dez_anos = idade + 10
escrever "Em 10 anos, " + nome + " terá " + idade_em_dez_anos + " anos"
```

## Exemplo em Python

```python
nome = input("Qual seu nome? ")
idade = int(input("Qual sua idade? "))
idade_em_dez_anos = idade + 10
print(f"Em 10 anos, {nome} terá {idade_em_dez_anos} anos")
```

## Exemplo em TypeScript

```ts
const nome = "Maria";
const idade = 28;
const idadeEmDezAnos = idade + 10;
console.log(`Em 10 anos, ${nome} terá ${idadeEmDezAnos} anos`);
```

(Em TypeScript puro fora do navegador, ler entrada do terminal exige bibliotecas extras — por isso este exemplo usa valores fixos. Não se preocupe com isso agora.)

## Erros comuns

- Esquecer de converter texto para número antes de somar (em Python, `input()` sempre retorna string).
- Confundir `=` (atribuição) com `==` (comparação).
- Dar nomes de variável que não dizem nada (`x`, `a`, `tmp`) quando um nome claro ajudaria a entender o código depois.

## Perguntas de reflexão

1. O que aconteceria se você somasse `idade + 10` sem converter `idade` para número?
2. Por que nomear bem uma variável ajuda até você mesmo, no futuro?
3. Qual a diferença entre "processar" e apenas "mostrar" um valor?

## Checklist para avançar

- [ ] Entendo o que é uma variável.
- [ ] Consigo ler uma entrada e usá-la em um cálculo.
- [ ] Consigo explicar a diferença entre entrada, processamento e saída com minhas próprias palavras.
