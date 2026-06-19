# Fase 08 — Banco de dados e persistência

**Duração sugerida:** 4 a 6 semanas

## Objetivo da fase

Completar o backend com persistência real — backend sem banco de dados é incompleto.

## Pré-requisitos

Fase 07 concluída (ou em andamento em paralelo, já que os dois temas se complementam).

## Tópicos e ordem sugerida

Tabelas, colunas, tipos, chave primária, chave estrangeira, índices, constraints, relacionamentos 1:1, 1:N e N:N, normalização, transações, migrations, seeds, backup, concorrência, integridade referencial.

### SQL essencial

`SELECT`, `INSERT`, `UPDATE`, `DELETE`, `WHERE`, `JOIN`, `GROUP BY`, `ORDER BY`, `LIMIT`, `COUNT`, `SUM`, `AVG`.

## Atividades / exercícios esperados

Evoluir a API financeira da Fase 07 para suportar cartão de crédito, parcelas, contas bancárias, anexos de comprovantes, relatórios por categoria e metas mensais. Antes de implementar, escrever o modelo de dados em Markdown.

## Critérios para avançar

- [ ] O modelo de dados foi escrito antes da implementação (não depois).
- [ ] As migrations rodam sem erro e o relacionamento entre as tabelas está correto.
- [ ] Consegue escrever consultas SQL básicas sem copiar de exemplo.

## Como a IA deve ajudar nesta fase

- Revisar o modelo de dados escrito pelo aluno antes de gerar qualquer migration.
- Explicar por que um relacionamento deveria ser 1:N em vez de N:N (ou vice-versa) quando o aluno tiver dúvida.

## Como a IA NÃO deve ajudar nesta fase

- Não desenhe o modelo de dados inteiro pelo aluno — revise o que ele propôs e questione decisões antes de aceitar.
- Não gere migrations sem o modelo de dados estar documentado primeiro.
