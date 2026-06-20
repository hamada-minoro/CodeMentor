# Módulo 10 — Testes e qualidade

**Duração sugerida:** 4 a 6 semanas (4 aulas)

## Objetivo do módulo

Entender que teste não é burocracia — é prova de comportamento.

## Pré-requisitos

Módulo 09 concluído.

## Aulas

### Aula 1 — Tipos de teste

Teste unitário, teste de integração, teste de contrato, teste end-to-end, teste manual guiado, teste de regressão.

### Aula 2 — O que testar primeiro

Regras de negócio, validações, autenticação, permissões, cálculos, estados inválidos, integrações críticas.

### Aula 3 — Escrevendo a suíte de testes

Aplicar testes unitários e de integração na API financeira (Módulos 08 e 09).

### Aula 4 — Checklist de qualidade

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

Escrever testes unitários e de integração para a API financeira construída nos Módulos 08 e 09, cobrindo pelo menos as regras de negócio principais e os casos de erro mais relevantes (entrada inválida, autenticação ausente, permissão insuficiente).

## Critérios para avançar

- [ ] As regras de negócio principais têm teste automatizado.
- [ ] O aluno consegue explicar a diferença entre teste unitário e teste de integração com um exemplo próprio.
- [ ] O checklist de qualidade acima foi aplicado a pelo menos uma feature real do projeto.

## Como a IA deve ajudar neste módulo

- Sugerir quais cenários testar antes de qualquer código de teste ser escrito.
- Revisar a cobertura de testes do aluno, apontando lacunas (especialmente em casos de erro).

## Como a IA NÃO deve ajudar neste módulo

- Não escreva a suíte de testes inteira de uma vez — ajude o aluno a pensar nos cenários primeiro, depois revise o que ele escrever.
