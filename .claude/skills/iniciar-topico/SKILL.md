---
name: iniciar-topico
description: Inicia um novo tópico de estudo do roadmap, criando a estrutura de pastas, teoria e exercícios sem gabarito. Use quando o aluno pedir para começar, iniciar ou abrir um tópico/fase do roadmap.
---

# Skill: Iniciar Tópico

## Processo obrigatório

1. Ler `CLAUDE.md`.
2. Ler `.tutor/tutor-manifest.md`.
3. Ler `.tutor/fluxo-de-estudo.md`.
4. Identificar a fase e o tópico solicitados pelo aluno. Se o aluno não especificar a fase, consultar `.tutor/curriculo/mapa-geral.md` e perguntar.
5. Ler o arquivo da fase correspondente em `.tutor/curriculo/fase-XX-*.md`.
6. Verificar se a pasta `estudos/fase-XX-nome/topico-YY-nome/` já existe. Se já existir, avisar o aluno em vez de sobrescrever.
7. Criar a pasta `estudos/fase-XX-nome/topico-YY-nome-do-topico/`.
8. Criar `README.md` do tópico usando `.tutor/templates/template-readme-topico.md` como modelo, com:
   - nome do tópico e fase;
   - objetivo de aprendizado;
   - explicação em linguagem simples;
   - exemplo em pseudocódigo;
   - exemplo em Python;
   - exemplo em TypeScript;
   - erros comuns;
   - perguntas de reflexão;
   - checklist para avançar.
9. Criar `exercicios.md` usando `.tutor/templates/template-exercicios.md`, com exercícios de aquecimento, principais e um desafio extra.
10. Criar `minhas-respostas/python/.gitkeep` e `minhas-respostas/typescript/.gitkeep`.
11. Criar `revisao.md`, `nota.md` e `consolidacao.md` vazios (ou com instruções mínimas de preenchimento futuro).
12. Criar `diario.md` vazio para anotações do aluno.
13. Explicar ao aluno, em texto, o que fazer agora: estudar o README, resolver os exercícios sem IA, colocar as respostas em `minhas-respostas/` e pedir revisão depois.

## Regra explícita

Não crie gabarito no primeiro momento. O aluno deve tentar antes. Não inclua soluções completas em `exercicios.md` nem em nenhum outro arquivo criado por esta skill.

## Saída esperada

- Resumo do tópico criado e caminho da pasta.
- Lembrete de que o aluno deve tentar manualmente antes de pedir ajuda ou revisão.
