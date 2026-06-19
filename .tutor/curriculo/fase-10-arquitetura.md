# Fase 10 — Arquitetura de software

**Duração sugerida:** contínua

## Objetivo da fase

Entender que arquitetura é sobre decisões, limites e trade-offs — não sobre seguir um padrão por modismo.

## Pré-requisitos

Fase 09 concluída.

## Tópicos e ordem sugerida

Separação de responsabilidades, camadas, domínio, aplicação, infraestrutura, controllers, services, repositories, DTOs, entidades, casos de uso, inversão de dependência, acoplamento, coesão, modularidade, design patterns, arquitetura limpa, DDD introdutório, eventos, filas, cache, observabilidade.

## Uma arquitetura inicial simples

```text
src/
  modules/
    users/
      users.controller.ts
      users.service.ts
      users.repository.ts
      users.types.ts
      users.schema.ts
      users.test.ts
    transactions/
      ...
  shared/
    database/
    errors/
    logger/
    config/
```

## Perguntas de arquitetura

Antes de aceitar uma solução da IA, perguntar: onde essa regra deveria morar? Essa função está grande demais? Esse módulo sabe coisas demais? Esse código será fácil de testar? Se o banco mudar, quanto código quebra? Se a regra mudar, onde altero? O erro está explícito? A solução está simples ou "inteligente demais"?

## Atividades / exercícios esperados

Reorganizar a API financeira das fases anteriores seguindo a estrutura de camadas acima, separando controllers, services e repositories. Documentar a decisão de onde cada regra de negócio mora.

## Critérios para avançar

- [ ] O projeto está organizado em camadas com responsabilidades claras.
- [ ] O aluno consegue responder às perguntas de arquitetura sobre o próprio código.
- [ ] Mudar uma regra de negócio não exige tocar em código de banco de dados diretamente.

## Como a IA deve ajudar nesta fase

- Fazer as perguntas de arquitetura listadas acima sempre que revisar uma proposta de solução, antes de aceitar.
- Explicar trade-offs entre abordagens, sem impor uma única "arquitetura certa".

## Como a IA NÃO deve ajudar nesta fase

- Não imponha um padrão arquitetural complexo (DDD completo, microsserviços) para um projeto de estudo pequeno — isso seria complexidade desnecessária.
