# Módulo 06 — Estruturas de dados, algoritmos e Big O (Python)

**Duração sugerida:** 6 a 8 semanas (8 aulas)

## Objetivo do módulo

Entender eficiência — não para decorar desafios de entrevista, mas para escolher a estrutura certa para cada problema.

## Pré-requisitos

Módulo 05 concluído.

## Aulas

### Aula 1 — Listas, pilhas e filas

`list` como pilha e fila, `collections.deque`.

### Aula 2 — Sets e dicionários como tabela hash

Por que busca em `set`/`dict` costuma ser O(1).

### Aula 3 — Linked lists, árvores e grafos

Implementações simples em Python, para entender a ideia — não para usar no dia a dia.

### Aula 4 — Heaps

`heapq`, fila de prioridade.

### Aula 5 — Busca

Busca linear e busca binária.

### Aula 6 — Ordenação e recursão

Ordenação simples (bubble/insertion) vs. `sorted()`/`.sort()` nativos, recursão básica.

### Aula 7 — BFS, DFS e backtracking

Percorrer grafos/árvores, backtracking básico.

### Aula 8 — Big O

Identificar O(1), O(log n), O(n), O(n log n), O(n²), O(2ⁿ) em código Python real.

## Como estudar sem virar decoreba

Para cada algoritmo: escrever a ideia em português, desenhar um exemplo, implementar em Python, testar com entradas pequenas e grandes, explicar a complexidade, e só então pedir para a IA revisar a explicação.

## Atividades / exercícios esperados

Projeto do módulo: comparador de performance — busca em lista com 100 itens, busca em lista com 10.000 itens, busca em dicionário, ordenação simples, ordenação nativa (`sorted()`). Documentar os resultados com tempos medidos (`time` ou `timeit`).

## Critérios para avançar

- [ ] Implementou e testou pelo menos 3 algoritmos de busca/ordenação em Python.
- [ ] Consegue identificar a complexidade Big O de um algoritmo simples sem ajuda.
- [ ] O comparador de performance documenta resultados reais, não estimativas.

## Como a IA deve ajudar neste módulo

- Revisar a explicação escrita do aluno sobre a complexidade de um algoritmo, apontando se está correta.
- Sugerir entradas de teste (pequenas e grandes) quando o aluno não souber por onde começar a medir performance.

## Como a IA NÃO deve ajudar neste módulo

- Não entregue a implementação do algoritmo antes do aluno tentar — incluindo algoritmos "clássicos" como busca binária ou bubble sort.
