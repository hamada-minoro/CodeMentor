# Fase 09 — Testes e qualidade

**Duração sugerida:** 4 a 6 semanas

## Objetivo da fase

Entender que teste não é burocracia — é prova de comportamento.

## Pré-requisitos

Fase 08 concluída.

## Tópicos e ordem sugerida

Teste unitário, teste de integração, teste de contrato, teste end-to-end, teste manual guiado, teste de regressão.

### O que testar primeiro

Regras de negócio, validações, autenticação, permissões, cálculos, estados inválidos, integrações críticas.

## Checklist de qualidade

Antes de considerar uma feature pronta:

- [ ] Existe spec?
- [ ] Existem critérios de aceitação?
- [ ] A regra principal tem teste?
- [ ] Casos de erro foram tratados?
- [ ] Logs são suficientes?
- [ ] Nomes estão claros?
- [ ] A implementação respeita a arquitetura?
- [ ] O README foi atualizado?
- [ ] A IA não criou complexidade desnecessária?

## Atividades / exercícios esperados

Escrever testes unitários e de integração para a API financeira construída nas Fases 07 e 08, cobrindo pelo menos as regras de negócio principais e os casos de erro mais relevantes (entrada inválida, autenticação ausente, permissão insuficiente).

## Critérios para avançar

- [ ] As regras de negócio principais têm teste automatizado.
- [ ] O aluno consegue explicar a diferença entre teste unitário e teste de integração com um exemplo próprio.
- [ ] O checklist de qualidade acima foi aplicado a pelo menos uma feature real do projeto.

## Como a IA deve ajudar nesta fase

- Sugerir quais cenários testar antes de qualquer código de teste ser escrito.
- Revisar a cobertura de testes do aluno, apontando lacunas (especialmente em casos de erro).

## Como a IA NÃO deve ajudar nesta fase

- Não escreva a suíte de testes inteira de uma vez — ajude o aluno a pensar nos cenários primeiro, depois revise o que ele escrever.
