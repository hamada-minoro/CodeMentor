# Módulo 09 — Banco de dados e persistência

**Duração sugerida:** 4 a 6 semanas (6 aulas)

## Objetivo do módulo

Completar o backend com persistência real — backend sem banco de dados é incompleto.

## Pré-requisitos

Módulo 08 concluído (ou em andamento em paralelo, já que os dois temas se complementam).

## Aulas

### Aula 1 — Modelagem relacional

Tabelas, colunas, tipos, chave primária, chave estrangeira, índices, constraints.

### Aula 2 — Relacionamentos

Relacionamentos 1:1, 1:N e N:N, normalização.

### Aula 3 — SQL essencial

`SELECT`, `INSERT`, `UPDATE`, `DELETE`, `WHERE`, `JOIN`, `GROUP BY`, `ORDER BY`, `LIMIT`, `COUNT`, `SUM`, `AVG`.

### Aula 4 — Migrations e seeds

Versionar o esquema do banco, popular dados iniciais.

### Aula 5 — Transações e concorrência

Transações, integridade referencial, o que pode dar errado com acesso concorrente.

### Aula 6 — Backup e integridade

Backup básico, e por que integridade referencial importa mais do que parece no começo.

## Atividades / exercícios esperados

Evoluir a API financeira do Módulo 08 para suportar cartão de crédito, parcelas, contas bancárias, anexos de comprovantes, relatórios por categoria e metas mensais. Antes de implementar, escrever o modelo de dados em Markdown.

## Critérios para avançar

- [ ] O modelo de dados foi escrito antes da implementação (não depois).
- [ ] As migrations rodam sem erro e o relacionamento entre as tabelas está correto.
- [ ] Consegue escrever consultas SQL básicas sem copiar de exemplo.

## Como a IA deve ajudar neste módulo

- Revisar o modelo de dados escrito pelo aluno antes de gerar qualquer migration.
- Explicar por que um relacionamento deveria ser 1:N em vez de N:N (ou vice-versa) quando o aluno tiver dúvida.

## Como a IA NÃO deve ajudar neste módulo

- Não desenhe o modelo de dados inteiro pelo aluno — revise o que ele propôs e questione decisões antes de aceitar.
- Não gere migrations sem o modelo de dados estar documentado primeiro.
