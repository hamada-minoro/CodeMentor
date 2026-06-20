# Guia do Spec-Driven Developer

## O problema: vibe coding

Vibe coding é pedir algo vago à IA, aceitar o que ela gera, testar superficialmente e seguir corrigindo no improviso:

```text
Crie um sistema de login completo aí usando Node.
```

Esse pedido não define regras, segurança, banco, erros, testes, arquitetura, escopo ou critérios de aceite — a IA decide tudo por você, inclusive decisões que deveriam ser suas. Um iniciante que aceita esse código sem entender constrói uma base frágil: sabe que "funcionou", mas não sabe por quê.

## A alternativa: Spec-Driven Development

Trabalhar com especificação antes da implementação. Em vez de começar pelo código, você começa pelos artefatos:

```text
spec.md      -> o que será feito e por quê
plan.md      -> como será feito
tasks.md     -> tarefas pequenas e verificáveis
tests.md     -> cenários de validação
review.md    -> revisão final
```

A IA deixa de "chutar código" e passa a ser executora supervisionada de um plano claro. Quanto mais ambíguo o pedido, mais a IA precisa adivinhar — e adivinhar errado custa retrabalho.

## Prompt solto vs. contexto estruturado

**Prompt solto:** `Crie login com JWT.`

**Contexto estruturado:**

```text
Vamos criar a feature de login usando o fluxo spec-driven.

Antes de implementar, leia CLAUDE.md e docs/specs/001-auth-login/{spec,plan,tasks}.md.

Regras: não altere escopo sem avisar; implemente uma task por vez; após cada etapa,
explique arquivos alterados; crie testes para regras de negócio; atualize review.md
com riscos e pendências.

Comece apenas validando se a spec tem ambiguidades.
```

## Como criar cada artefato

Use os templates em `.tutor/templates/`: `template-spec.md`, `template-plan.md`, `template-tasks.md`, `template-tests.md`, `template-review.md`. Exemplo completo em `exemplos-projetos/projeto-spec-driven/docs/specs/001-exemplo-feature/`.

## Quando começar a usar IA para implementar

A partir do Módulo 08 deste roadmap (quando você já souber construir uma API básica sozinho), você pode delegar implementação para a IA — dentro de um fluxo de spec, plan e tasks. Antes disso, construa com as próprias mãos.

## Como revisar código gerado por IA

Classifique cada problema encontrado:

- **bloqueante** — impede a feature de funcionar corretamente ou com segurança;
- **importante** — deveria ser corrigido antes de aceitar;
- **melhoria** — sugestão de qualidade, sem urgência;
- **dúvida** — algo que você não entendeu e precisa esclarecer.

Pergunte sempre: resolve o problema real? Cobre casos de erro? Tem teste? É seguro e simples o bastante? Respeita a arquitetura?

## Fluxo de uma nova feature

```text
1. Entender o problema       5. Mapear riscos          9. Testar cada task
2. Escrever spec             6. Criar plano técnico    10. Revisar código
3. Definir critérios         7. Quebrar em tasks        11. Atualizar docs
4. Mapear regras de negócio  8. Implementar task a task 12. Registrar decisões
```

O **Spec-Driven Developer** não é alguém que só pede código — é alguém que entende o problema, especifica a solução, planeja, conduz a IA e valida o resultado.
