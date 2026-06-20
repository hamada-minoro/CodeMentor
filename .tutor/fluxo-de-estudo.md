# Fluxo de Estudo por Aula

Este é o ciclo obrigatório que qualquer IA tutora deve seguir ao conduzir uma aula do roadmap. Os prompts e skills do repositório implementam este fluxo — eles não substituem este documento, apenas o automatizam.

## O ciclo completo

1. O aluno escolhe uma aula do roadmap (veja `.tutor/curriculo/mapa-geral.md`).
2. O aluno pede: "Iniciar aula X do módulo Y".
3. A IA lê `.tutor/tutor-manifest.md`, o módulo correspondente em `.tutor/curriculo/` e as rubricas em `.tutor/rubricas/`.
4. A IA cria uma pasta em `estudos/modulo-XX-nome/aula-YY-nome-da-aula/`.
5. Dentro da pasta, a IA cria:
   - `README.md` com a explicação do conteúdo (veja `.tutor/templates/template-readme-aula.md`);
   - `exercicios.md` com exercícios progressivos (veja `.tutor/templates/template-exercicios.md`);
   - `minhas-respostas/python/` e `minhas-respostas/typescript/` para o aluno colocar os códigos;
   - `revisao.md` vazio ou com instruções de preenchimento;
   - `nota.md` vazio ou com a rubrica pronta para ser usada;
   - `consolidacao.md` vazio;
   - `diario.md` vazio, para anotações pessoais do aluno sobre essa aula específica.
6. O aluno estuda o `README.md`.
7. O aluno resolve os exercícios manualmente — em Python (Módulos 00 a 06), e em Python e/ou TypeScript a partir do Módulo 07.
8. O aluno coloca as respostas em `minhas-respostas/`.
9. O aluno pede: "Revise meus exercícios desta aula".
10. A IA analisa os arquivos reais do aluno, sem inventar conteúdo que não está lá.
11. A IA escreve `revisao.md` com: acertos, erros, explicações dos conceitos por trás dos erros, riscos de raciocínio, melhorias e sugestões.
12. A IA escreve `nota.md` com nota de 0 a 10 usando a rubrica em `.tutor/rubricas/rubrica-codigo.md`.
13. A IA cria `consolidacao.md` com um exercício novo, focado nos erros observados, para reforço.
14. O aluno tenta o exercício de consolidação.
15. A IA revisa novamente, atualizando `revisao.md` e `nota.md`.
16. A IA atualiza `progresso/mapa-de-progresso.md` com o status mais recente.
17. A IA sugere a próxima aula, mas **nunca avança automaticamente** sem o aluno pedir.

## Regra de ouro do ciclo

Nenhuma etapa deste ciclo deve pular a tentativa do aluno. Se o aluno pedir para "pular direto para a revisão" sem ter resolvido nada, a IA deve recusar educadamente e reforçar por que a tentativa importa — veja `.tutor/principios-pedagogicos.md`.

## Quando o ciclo é mais flexível

A partir do Módulo 08 (projetos maiores) e principalmente no Módulo 12 (Spec-Driven Development), o ciclo se adapta: em vez de `exercicios.md`, o aluno trabalha com `spec.md`, `plan.md`, `tasks.md`, `tests.md` e `review.md` (veja `docs/GUIA_SPEC_DRIVEN_DEVELOPER.md` e a skill `spec-driven-feature`). O espírito é o mesmo: pensar antes de implementar, e revisar depois.
