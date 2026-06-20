# Módulo 08 — Backend com Node.js/TypeScript e Python

**Duração sugerida:** 8 a 10 semanas (8 aulas)

## Objetivo do módulo

Construir software mais próximo do mercado: APIs reais, com autenticação e testes.

## Pré-requisitos

Módulo 07 concluído. O aluno já sabe criar e configurar um projeto Node + TypeScript; aqui o foco é usar isso para construir uma API de verdade.

## Aulas

### Aula 1 — Fundamentos web

Cliente e servidor, HTTP, request e response, headers, status codes, JSON, REST.

### Aula 2 — Autenticação, autorização e segurança básica

Autenticação, autorização, CORS, variáveis de ambiente, riscos comuns (senha em texto puro, token exposto).

### Aula 3 — Paginação, filtros e logs

Listar dados com paginação e filtros, e por que registrar logs estruturados.

### Aula 4 — Node.js com TypeScript: framework HTTP

Node.js puro, depois Express ou Fastify sobre o projeto criado no Módulo 07.

### Aula 5 — Validação e persistência em Node/TypeScript

Validação com Zod, Prisma ORM, PostgreSQL.

### Aula 6 — Testes e qualidade em Node/TypeScript

Jest ou Vitest, ESLint e Prettier. Opcional: avançar para NestJS (módulos, providers, dependency injection, pipes, guards, interceptors).

### Aula 7 — Python backend

FastAPI, Pydantic, SQLAlchemy, Alembic, Pytest, Uvicorn.

### Aula 8 — Comparando as duas implementações

Implementar o mesmo domínio nas duas stacks e comparar abordagens, não só sintaxe.

## Atividades / exercícios esperados

Projeto do módulo: API de controle financeiro pessoal, com cadastro de usuário, login, cadastro de categorias, receitas, despesas, listagem por período, resumo mensal, saldo, exportação CSV e testes básicos. Versão 1 em Node.js + TypeScript; versão 2 em Python + FastAPI, mesmo domínio, outra implementação.

Documentar: diagrama simples de entidades, endpoints, exemplos de request/response, regras de negócio, erros esperados, como rodar localmente e como rodar testes.

## Critérios para avançar

- [ ] As duas versões da API (Node.js e Python) implementam o mesmo domínio com sucesso.
- [ ] Existem testes básicos cobrindo ao menos as regras de negócio principais.
- [ ] A documentação dos endpoints está completa.

## Como a IA deve ajudar neste módulo

- A partir deste módulo, é apropriado começar a introduzir os artefatos formais de Spec-Driven Development (`spec.md`, `plan.md`, `tasks.md`) em projetos maiores como este — veja `.tutor/curriculo/modulo-12-ia-spec-driven.md` e `docs/GUIA_SPEC_DRIVEN_DEVELOPER.md`.
- Revisar contratos de API antes da implementação, apontando ambiguidades.

## Como a IA NÃO deve ajudar neste módulo

- Não gere a API completa de uma vez. Trabalhe endpoint por endpoint, revisando cada um.
- Não aceite código de autenticação sem revisar explicitamente questões de segurança básicas (senhas em texto puro, tokens expostos, etc.).
