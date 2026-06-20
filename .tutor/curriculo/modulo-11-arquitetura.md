# Módulo 11 — Arquitetura de software

**Duração sugerida:** contínua (5 aulas, sem prazo fixo — este módulo acompanha o aluno por mais tempo)

## Objetivo do módulo

Entender que arquitetura é sobre decisões, limites e trade-offs — não sobre seguir um padrão por modismo.

## Pré-requisitos

Módulo 10 concluído.

## Aulas

### Aula 1 — Separação de responsabilidades

Camadas, domínio, aplicação, infraestrutura, controllers, services, repositories, DTOs, entidades, casos de uso.

### Aula 2 — Acoplamento, coesão e modularidade

Inversão de dependência, como perceber componentes fortemente amarrados entre si.

### Aula 3 — Uma arquitetura inicial simples

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

### Aula 4 — Design patterns e DDD introdutório

Visão geral de padrões comuns e dos conceitos básicos de Domain-Driven Design — sem exagerar no projeto de estudo.

### Aula 5 — Eventos, filas, cache e observabilidade

Visão geral, sem profundidade — esses temas se aprofundam depois do Módulo 13 (veja "Depois da base" em `docs/ROADMAP.md`).

## Perguntas de arquitetura

Antes de aceitar uma solução da IA, perguntar: onde essa regra deveria morar? Essa função está grande demais? Esse componente sabe coisas demais? Esse código será fácil de testar? Se o banco mudar, quanto código quebra? Se a regra mudar, onde altero? O erro está explícito? A solução está simples ou "inteligente demais"?

## Atividades / exercícios esperados

Reorganizar a API financeira dos módulos anteriores seguindo a estrutura de camadas acima, separando controllers, services e repositories. Documentar a decisão de onde cada regra de negócio mora.

## Critérios para avançar

- [ ] O projeto está organizado em camadas com responsabilidades claras.
- [ ] O aluno consegue responder às perguntas de arquitetura sobre o próprio código.
- [ ] Mudar uma regra de negócio não exige tocar em código de banco de dados diretamente.

## Como a IA deve ajudar neste módulo

- Fazer as perguntas de arquitetura listadas acima sempre que revisar uma proposta de solução, antes de aceitar.
- Explicar trade-offs entre abordagens, sem impor uma única "arquitetura certa".

## Como a IA NÃO deve ajudar neste módulo

- Não imponha um padrão arquitetural complexo (DDD completo, microsserviços) para um projeto de estudo pequeno — isso seria complexidade desnecessária.
