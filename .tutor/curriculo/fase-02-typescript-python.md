# Fase 02 — Fundamentos de TypeScript e Python

**Duração sugerida:** 4 a 6 semanas

## Objetivo da fase

Escrever código básico com mais organização nas duas linguagens da trilha.

## Pré-requisitos

Fase 01 concluída.

## Tópicos e ordem sugerida

### TypeScript

`let`/`const`, tipos primitivos, arrays, objetos, funções, parâmetros opcionais, retorno de função, interfaces, type aliases, enums, union types, generics básicos, módulos, async/await, `try/catch`.

### Python

Variáveis, listas, dicionários, tuplas, funções, argumentos nomeados, módulos, pacotes, list comprehension, tratamento de exceções, arquivos, type hints, dataclasses, ambientes virtuais.

## Exemplo de foco

```ts
type User = { id: string; name: string; email: string };
function formatUser(user: User): string {
  return `${user.name} <${user.email}>`;
}
```

```python
from dataclasses import dataclass

@dataclass
class User:
    id: str
    name: str
    email: str

def format_user(user: User) -> str:
    return f"{user.name} <{user.email}>"
```

## Atividades / exercícios esperados

Projeto da fase: gerenciador de tarefas via terminal, nas duas linguagens, com: criar tarefa, listar tarefas, marcar como concluída, remover tarefa, salvar em arquivo JSON, carregar do arquivo ao iniciar.

Documentar no `README.md` do projeto: como rodar, quais estruturas de dados foram usadas, quais erros foram encontrados e como foram resolvidos.

## Critérios para avançar

- [ ] O gerenciador de tarefas funciona nas duas linguagens.
- [ ] O aluno consegue explicar a diferença entre tipagem dinâmica (Python) e estática (TypeScript) com suas próprias palavras.
- [ ] O `README.md` do projeto está completo.

## Como a IA deve ajudar nesta fase

- Explicar diferenças de sintaxe e de filosofia entre as duas linguagens quando o aluno perguntar.
- Revisar o código do projeto da fase, mas só depois de uma tentativa real do aluno.

## Como a IA NÃO deve ajudar nesta fase

- Não gere o projeto completo do gerenciador de tarefas. O aluno deve construir peça por peça.
- Não pule a comparação entre Python e TypeScript — esse contraste é o ponto pedagógico da fase.
