# Revisão — Variáveis, Entrada, Processamento e Saída

> Este é um exemplo de como a IA deve preencher este arquivo depois de revisar respostas reais do aluno. Em um módulo real, o conteúdo abaixo seria gerado a partir dos arquivos que estiverem em `minhas-respostas/`.

## Pontos fortes

- O exercício 1 e 2 (aquecimento) foram resolvidos corretamente nas duas linguagens, com nomes de variável claros.
- No exercício 3, a divisão entre os dois números foi implementada corretamente em Python.

## Erros encontrados

- No exercício 3 em TypeScript, a divisão não tratou o caso de divisão por zero.
- No exercício 5, a idade foi lida como string e somada diretamente a 10 sem conversão, gerando concatenação em vez de soma em Python.

## Conceito por trás dos erros

- Em Python, `input()` sempre devolve uma string. Para somar como número, é preciso converter com `int()` ou `float()` antes da operação.
- Dividir por zero é matematicamente indefinido — bons programas verificam esse caso antes de calcular, em vez de deixar o programa quebrar ou retornar um valor sem sentido.

## Riscos de raciocínio

- Notei uma tendência a assumir que "se rodou sem erro, está certo". Vale revisar a saída do programa com atenção, não só se ele rodou.

## Melhorias sugeridas

- Adicionar uma verificação antes de dividir: `se divisor for igual a 0, avisar o usuário`.
- Converter entradas numéricas explicitamente logo após a leitura, antes de qualquer cálculo.

## Conclusão

O aluno está pronto para avançar com uma consolidação focada em conversão de tipos e tratamento do caso de divisão por zero antes de seguir para o próximo módulo (condicionais).
