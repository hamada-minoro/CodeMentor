---
name: iniciar-aula
description: Inicia uma nova aula de estudo do roadmap, criando a estrutura de pastas, teoria e exercícios sem gabarito. Use quando o aluno pedir para começar, iniciar ou abrir uma aula/módulo do roadmap.
---

# Skill: Iniciar Aula

## Processo obrigatório

1. Ler `CLAUDE.md`.
2. Ler `.tutor/tutor-manifest.md`.
3. Ler `.tutor/fluxo-de-estudo.md`.
4. Identificar o módulo e a aula solicitados pelo aluno. Se o aluno não especificar o módulo, consultar `.tutor/curriculo/mapa-geral.md` e perguntar.
5. Ler o arquivo do módulo correspondente em `.tutor/curriculo/modulo-XX-*.md`.
6. Verificar se a pasta `estudos/modulo-XX-nome/aula-YY-nome/` já existe. Se já existir, avisar o aluno em vez de sobrescrever.
7. Criar a pasta `estudos/modulo-XX-nome/aula-YY-nome-da-aula/`.
8. Criar `README.md` da aula usando `.tutor/templates/template-readme-aula.md` como modelo, com:
   - nome da aula e módulo;
   - objetivo de aprendizado;
   - tópicos desta aula (lista curta de subseções de conteúdo);
   - explicação em linguagem simples;
   - exemplo em pseudocódigo;
   - exemplo em Python;
   - exemplo em TypeScript (somente a partir do Módulo 07 — nos Módulos 00 a 06, omita esta seção);
   - erros comuns;
   - perguntas de reflexão;
   - checklist para avançar.
9. Criar `exercicios.md` usando `.tutor/templates/template-exercicios.md`, com exercícios de aquecimento, principais e um desafio extra.
10. Criar `minhas-respostas/python/.gitkeep` (e `minhas-respostas/typescript/.gitkeep` somente a partir do Módulo 07).
11. Criar `revisao.md`, `nota.md` e `consolidacao.md` vazios (ou com instruções mínimas de preenchimento futuro).
12. Criar `diario.md` vazio para anotações do aluno.
13. Explicar ao aluno, em texto, o que fazer agora: estudar o README, resolver os exercícios sem IA, colocar as respostas em `minhas-respostas/` e pedir revisão depois.

## Regra explícita

Não crie gabarito no primeiro momento. O aluno deve tentar antes. Não inclua soluções completas em `exercicios.md` nem em nenhum outro arquivo criado por esta skill.

## Saída esperada

- Resumo da aula criada e caminho da pasta.
- Lembrete de que o aluno deve tentar manualmente antes de pedir ajuda ou revisão.
