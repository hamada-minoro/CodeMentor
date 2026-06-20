# Módulo 02 — Fundamentos de Python

**Duração sugerida:** 4 a 6 semanas (10 aulas)

## Objetivo do módulo

Escrever código Python com mais organização, indo além dos scripts simples do Módulo 01.

## Pré-requisitos

Módulo 01 concluído.

## Aulas

### Aula 1 — Listas e tuplas

Criar, percorrer, adicionar, remover, indexar, slicing.

### Aula 2 — Dicionários

Pares chave-valor, métodos comuns, quando usar dicionário em vez de lista.

### Aula 3 — Funções com argumentos nomeados

Argumentos posicionais, nomeados, valores padrão, `*args`/`**kwargs` (visão geral).

### Aula 4 — Módulos e pacotes da linguagem

Organizar código em múltiplos arquivos, `import`, estrutura de um pacote simples. (Aqui "módulo" é o termo da própria linguagem Python para um arquivo importável — não confundir com o Módulo 02 deste roadmap.)

### Aula 5 — List comprehension

Reescrever loops simples como comprehensions, sem abusar de comprehensions ilegíveis.

### Aula 6 — Tratamento de exceções

`try`/`except`/`finally`, criar exceções específicas, quando capturar e quando deixar propagar.

### Aula 7 — Arquivos

Ler e escrever arquivos de texto e JSON.

### Aula 8 — Type hints

Anotar tipos de parâmetros e retornos, e por que isso ajuda tanto humanos quanto IA a entender o código.

### Aula 9 — Dataclasses

Modelar entidades simples com `@dataclass` em vez de dicionários soltos.

### Aula 10 — Ambientes virtuais

`venv` (ou `uv`), `requirements.txt`, por que isolar dependências por projeto.

## Exemplo de foco

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

Projeto do módulo: gerenciador de tarefas via terminal, em Python, com: criar tarefa, listar tarefas, marcar como concluída, remover tarefa, salvar em arquivo JSON, carregar do arquivo ao iniciar.

Documentar no `README.md` do projeto: como rodar, quais estruturas de dados foram usadas, quais erros foram encontrados e como foram resolvidos.

## Critérios para avançar

- [ ] O gerenciador de tarefas funciona de ponta a ponta (criar, listar, concluir, remover, persistir).
- [ ] O aluno consegue explicar, com suas próprias palavras, por que usou lista, dicionário ou dataclass em cada parte do projeto.
- [ ] O `README.md` do projeto está completo.

## Como a IA deve ajudar neste módulo

- Explicar quando usar lista, dicionário, tupla ou dataclass, com exemplos pequenos.
- Revisar o código do projeto do módulo, mas só depois de uma tentativa real do aluno.

## Como a IA NÃO deve ajudar neste módulo

- Não gere o projeto completo do gerenciador de tarefas. O aluno deve construir peça por peça.
- Não introduza TypeScript ou Node.js neste módulo — isso é assunto do Módulo 07, depois que a base em Python estiver sólida.
