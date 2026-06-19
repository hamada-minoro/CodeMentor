---
name: revisar-exercicios
description: Revisa as respostas do aluno em minhas-respostas/, escreve revisao.md e nota.md usando rubrica, e propõe consolidação. Use quando o aluno pedir revisão dos exercícios de um tópico.
---

# Skill: Revisar Exercícios

## Processo obrigatório

1. Ler `CLAUDE.md` e `.tutor/tutor-manifest.md`.
2. Ler `.tutor/rubricas/rubrica-codigo.md` e `.tutor/rubricas/escala-de-notas.md`.
3. Ler os arquivos reais do aluno em `estudos/.../minhas-respostas/python/` e `.../typescript/`. Não invente conteúdo que não esteja lá — se a pasta estiver vazia, avise o aluno em vez de revisar algo inexistente.
4. Ler `exercicios.md` do mesmo tópico para comparar a resposta com o que foi pedido.
5. **Preservar o código original do aluno.** Nunca edite ou sobrescreva os arquivos em `minhas-respostas/`.
6. Escrever ou atualizar `revisao.md` usando `.tutor/templates/template-revisao.md`, contendo, nesta ordem:
   - pontos fortes (o que funcionou);
   - erros encontrados;
   - explicação do conceito por trás de cada erro;
   - riscos de raciocínio (não só bugs pontuais);
   - sugestões de melhoria;
   - indicação clara se o aluno pode avançar ou precisa de reforço.
7. Escrever `nota.md` usando `.tutor/rubricas/rubrica-codigo.md`, com nota de 0 a 10 e justificativa item a item.
8. Atualizar `progresso/mapa-de-progresso.md` com o status e a nota mais recentes.
9. Sugerir (sem decidir por ele) que o aluno gere uma consolidação se a nota for baixa ou houver erro conceitual recorrente — usar a skill `consolidar-conhecimento`.

## Regras explícitas

- Não dê nota sem justificativa.
- Não seja vago: "está errado" não é uma revisão válida — explique o porquê.
- Não humilhe o aluno. Comece sempre pelos pontos fortes.
- Não revise um exercício que o aluno não tentou — se notar que algo foi colado de uma IA sem entendimento, pergunte ao aluno antes de avaliar.

## Saída esperada

- Resumo direto: o que foi revisado, nota dada, e se o aluno está pronto para avançar ou precisa de reforço.
