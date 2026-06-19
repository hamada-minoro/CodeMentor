# Guia do Spec-Driven Developer

## O que é vibe coding

Vibe coding é quando você descreve algo de forma vaga para a IA, aceita o que ela gera, testa superficialmente e segue corrigindo no improviso.

Exemplo ruim:

```text
Crie um sistema de login completo aí usando Node.
```

Problemas com esse pedido: não define regras, não define segurança, não define banco, não define erros, não define testes, não define arquitetura, não define escopo, não define critérios de aceite.

## Por que vibe coding é perigoso para iniciantes

Quando você não especifica nada, a IA decide tudo por você — inclusive decisões que deveriam ser suas: como tratar erros, que dados validar, qual a regra de negócio real. Um iniciante que aceita esse código sem entender constrói uma base de conhecimento frágil: sabe que "funcionou", mas não sabe por quê, nem o que fazer quando parar de funcionar.

## O que é Spec-Driven Development

É trabalhar com especificação antes da implementação. Em vez de começar pelo código, você começa por artefatos:

```text
spec.md      -> o que será feito e por quê
plan.md      -> como será feito
tasks.md     -> tarefas pequenas e verificáveis
tests.md     -> cenários de validação
review.md    -> revisão final
```

A IA deixa de ser "alguém que chuta código" e passa a ser uma executora supervisionada de um plano claro.

## Por que especificar antes de codar melhora o uso da IA

Quanto mais ambíguo o pedido, mais a IA precisa "adivinhar" — e adivinhar errado custa retrabalho. Uma spec clara, com critérios de aceitação verificáveis, reduz a ambiguidade e te dá um jeito objetivo de checar se o resultado está certo.

## Diferença entre prompt solto e contexto estruturado

**Prompt solto:**

```text
Crie login com JWT.
```

**Contexto estruturado:**

```text
Vamos criar a feature de login usando o fluxo spec-driven.

Antes de implementar, leia:
- CLAUDE.md
- docs/specs/001-auth-login/spec.md
- docs/specs/001-auth-login/plan.md
- docs/specs/001-auth-login/tasks.md

Regras:
- não altere escopo sem avisar;
- implemente uma task por vez;
- após cada etapa, explique arquivos alterados;
- crie testes para regras de negócio;
- rode os testes relacionados;
- atualize review.md com riscos e pendências.

Comece apenas validando se a spec tem ambiguidades.
```

## Como criar spec, plan, tasks, tests e review

Use os templates em `.tutor/templates/`:

- `template-spec.md`
- `template-plan.md`
- `template-tasks.md`
- `template-tests.md`
- `template-review.md`

Veja um exemplo completo em `exemplos-projetos/projeto-spec-driven/docs/specs/001-exemplo-feature/`.

## Quando o aluno pode começar a usar IA para implementar

A partir da Fase 07 deste roadmap (quando você já souber construir uma API básica sozinho), você pode começar a delegar implementação para a IA — desde que dentro de um fluxo de spec, plan e tasks. Antes disso, o foco deve ser construir com as próprias mãos.

## Como revisar código gerado por IA

Classifique cada problema encontrado como:

- **bloqueante** — impede que a feature funcione corretamente ou com segurança;
- **importante** — deveria ser corrigido antes de aceitar, mas não impede o funcionamento básico;
- **melhoria** — sugestão de qualidade, sem urgência;
- **dúvida** — algo que você não entendeu e precisa esclarecer antes de aceitar.

Pergunte sempre: isso resolve o problema real? Cobre casos de erro? Tem teste? Segue os padrões do projeto? É seguro? É simples o bastante? Não criou dependências desnecessárias? Respeita a arquitetura?

## Fluxo profissional de uma nova feature

```text
1. Entender o problema
2. Escrever spec
3. Definir critérios de aceitação
4. Mapear regras de negócio
5. Mapear riscos e casos de erro
6. Criar plano técnico
7. Quebrar em tasks pequenas
8. Implementar uma task por vez
9. Testar cada task
10. Revisar código
11. Atualizar documentação
12. Registrar decisões
```

Esse é o caminho do **Spec-Driven Developer**: não seja apenas alguém que pede código — seja alguém que entende o problema, especifica a solução, planeja a execução, conduz a IA e valida o resultado.
