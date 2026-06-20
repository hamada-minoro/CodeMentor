# `estudos/`

É aqui que a IA cria a estrutura de cada aula do roadmap, quando você pede para iniciar uma aula.

## Estrutura

```text
estudos/
└── modulo-XX-nome/
    └── aula-YY-nome-da-aula/
        ├── README.md           ← teoria da aula
        ├── exercicios.md        ← exercícios progressivos, sem gabarito
        ├── minhas-respostas/    ← onde você coloca suas tentativas
        │   ├── python/
        │   └── typescript/      ← usado só a partir do Módulo 07
        ├── revisao.md           ← preenchido pela IA depois da sua tentativa
        ├── nota.md              ← nota com justificativa baseada em rubrica
        ├── consolidacao.md      ← exercício de reforço, se necessário
        └── diario.md            ← suas anotações sobre a aula
```

## Como começar

Peça à sua IA:

```text
Iniciar aula "[nome da aula]" do Módulo [número].
```

Se você já tem alguma experiência e não sabe por onde começar, peça um nivelamento (skill `nivelar-aluno`) em vez de adivinhar o módulo.

Veja o ciclo completo em `.tutor/fluxo-de-estudo.md` e um exemplo já preenchido em `.tutor/exemplos/exemplo-ciclo-aula-logica/`.

Esta pasta começa vazia — ela se preenche conforme você avança no roadmap.
