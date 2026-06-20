---
name: nivelar-aluno
description: Aplica um questionário curto de nivelamento para alunos que já têm alguma experiência em programação, descobre em qual módulo do roadmap eles devem começar, registra o ponto de partida no diário de aprendizado e no mapa de progresso, e inicia o módulo indicado. Use quando o aluno pedir nivelamento, perguntar "em qual módulo eu começo", dizer que já sabe programar, ou pedir um teste de nível inicial.
---

# Skill: Nivelar Aluno

Esta skill existe para alunos que **não estão começando do zero**. Quem nunca programou deve seguir o prompt padrão de início (Módulo 00, Aula 1) — não precisa de nivelamento.

## Processo obrigatório

1. Ler `CLAUDE.md`, `.tutor/tutor-manifest.md` e `.tutor/curriculo/mapa-geral.md`.
2. Aplicar o questionário abaixo, uma pergunta por vez ou em bloco (à escolha do aluno), sem julgar respostas erradas — o objetivo é mapear o nível real, não testar para reprovar.

### Questionário de nivelamento

1. Você já escreveu algum código antes? Em qual(is) linguagem(ns)?
2. Você sabe explicar, com suas palavras, o que são variáveis, condicionais (`if`/`else`) e laços (`for`/`while`)?
3. Você já escreveu funções com parâmetros e retorno?
4. Você sabe a diferença entre lista, dicionário/objeto e tupla, e quando usar cada um?
5. Você já usou Git e GitHub para versionar um projeto (commit, push, branch)?
6. Você sabe o que é uma classe, um objeto, e já organizou um programa em orientação a objetos?
7. Você sabe o que é Big O / complexidade de algoritmo, mesmo que de forma simples?
8. Você já criou ou configurou um projeto Node.js com TypeScript (`package.json`, `tsconfig.json`)?
9. Você já construiu uma API HTTP (rotas, request/response, autenticação)?
10. Você já modelou um banco de dados relacional ou escreveu migrations?
11. Você já escreveu testes automatizados (unitários ou de integração)?
12. Você já escreveu uma `spec.md` ou documento equivalente antes de implementar uma feature com IA?

## Como mapear respostas para o módulo de início

Use o `mapa-geral.md` como referência e a regra abaixo:

- Respostas "não" a partir da pergunta 1 ou 2 → começar no **Módulo 00**.
- Domina 2-4 (lógica básica em alguma linguagem), mas nunca usou Git → **Módulo 00 ou 01** (priorize o Módulo 00 se Git for novidade).
- Domina 1-5 mas não tem fluência em estruturas de dados nativas de Python → **Módulo 02**.
- Domina até 6 (OO) mas nunca parou para pensar em tipagem/contratos de dados → **Módulo 03**.
- Domina até 7 (Big O) mas nunca tocou em TypeScript/Node → **Módulo 07**.
- Domina até 8 (Node+TS configurado) mas nunca construiu API → **Módulo 08**.
- Domina até 9-10 (API com banco) mas não tem hábito de testes → **Módulo 10**.
- Domina até 11 (testes) mas nunca pensou em arquitetura em camadas → **Módulo 11**.
- Domina até 12 (specs/tasks com IA) → **Módulo 13** (Portfólio), revisando lacunas pontuais nos módulos anteriores se aparecerem no código do aluno.

**Regra explícita:** em caso de dúvida entre dois módulos, recomende sempre o mais cedo dos dois. Nunca recomende pular para o módulo mais avançado possível só porque o aluno afirma ter experiência — o módulo recomendado deve refletir o que o aluno demonstrou saber explicar, não apenas o que ele diz que já usou.

## Depois de decidir o módulo

1. Explicar ao aluno, em texto, qual módulo foi recomendado e por quê (citando as respostas que levaram à decisão).
2. Acrescentar uma entrada em `progresso/diario-de-aprendizado.md` (usar `.tutor/templates/template-diario.md` como modelo), registrando: data, resultado do nivelamento, módulo de início recomendado e principais lacunas identificadas.
3. Acrescentar uma linha em `progresso/mapa-de-progresso.md` com o módulo de início, aula inicial, status "em andamento" e a observação "início via nivelamento".
4. Perguntar ao aluno se ele concorda com o módulo recomendado ou quer começar em outro (a decisão final é do aluno).
5. Depois da confirmação, iniciar o módulo/aula combinado reaproveitando o processo da skill `iniciar-aula` (não duplique a lógica de criação de pastas — invoque o mesmo fluxo).

## Regra explícita

- Não pule o questionário para "economizar tempo do aluno" — sem as respostas, a recomendação de módulo não tem base.
- Não decida o módulo sozinho sem perguntar a confirmação final do aluno.
- Não crie a pasta do módulo antes de o aluno confirmar onde quer começar.

## Saída esperada

- Módulo e aula recomendados, com justificativa baseada nas respostas do questionário.
- Confirmação de que `progresso/diario-de-aprendizado.md` e `progresso/mapa-de-progresso.md` foram atualizados.
- Aula inicial já criada (via fluxo de `iniciar-aula`), após confirmação do aluno.
