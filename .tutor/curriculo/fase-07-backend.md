# Fase 07 — Backend com Node.js, TypeScript e Python

**Duração sugerida:** 8 a 10 semanas

## Objetivo da fase

Construir software mais próximo do mercado: APIs reais, com autenticação e testes.

## Pré-requisitos

Fase 06 concluída.

## Tópicos e ordem sugerida

### Fundamentos web

Cliente e servidor, HTTP, request e response, headers, status codes, JSON, REST, autenticação, autorização, CORS, paginação, filtros, logs, variáveis de ambiente.

### Node.js com TypeScript

Node.js puro, Express ou Fastify, validação com Zod, Prisma ORM, PostgreSQL, Jest ou Vitest, ESLint e Prettier. Depois, avançar para NestJS (módulos, providers, dependency injection, pipes, guards, interceptors, testes de integração).

### Python backend

FastAPI, Pydantic, SQLAlchemy, Alembic, Pytest, Uvicorn.

## Atividades / exercícios esperados

Projeto da fase: API de controle financeiro pessoal, com cadastro de usuário, login, cadastro de categorias, receitas, despesas, listagem por período, resumo mensal, saldo, exportação CSV e testes básicos. Versão 1 em Node.js + TypeScript; versão 2 em Python + FastAPI, mesmo domínio, outra implementação.

Documentar: diagrama simples de entidades, endpoints, exemplos de request/response, regras de negócio, erros esperados, como rodar localmente e como rodar testes.

## Critérios para avançar

- [ ] As duas versões da API (Node.js e Python) implementam o mesmo domínio com sucesso.
- [ ] Existem testes básicos cobrindo ao menos as regras de negócio principais.
- [ ] A documentação dos endpoints está completa.

## Como a IA deve ajudar nesta fase

- A partir desta fase, é apropriado começar a introduzir os artefatos formais de Spec-Driven Development (`spec.md`, `plan.md`, `tasks.md`) em projetos maiores como este — veja `.tutor/curriculo/fase-11-ia-spec-driven.md` e `GUIA_SPEC_DRIVEN_DEVELOPER.md`.
- Revisar contratos de API antes da implementação, apontando ambiguidades.

## Como a IA NÃO deve ajudar nesta fase

- Não gere a API completa de uma vez. Trabalhe endpoint por endpoint, revisando cada um.
- Não aceite código de autenticação sem revisar explicitamente questões de segurança básicas (senhas em texto puro, tokens expostos, etc.).
