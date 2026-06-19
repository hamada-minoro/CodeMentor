# `estudos/`

É aqui que a IA cria a estrutura de cada tópico do roadmap, quando você pede para iniciar um tópico.

## Estrutura

```text
estudos/
└── fase-XX-nome/
    └── topico-YY-nome-do-topico/
        ├── README.md           ← teoria do tópico
        ├── exercicios.md        ← exercícios progressivos, sem gabarito
        ├── minhas-respostas/    ← onde você coloca suas tentativas
        │   ├── python/
        │   └── typescript/
        ├── revisao.md           ← preenchido pela IA depois da sua tentativa
        ├── nota.md              ← nota com justificativa baseada em rubrica
        ├── consolidacao.md      ← exercício de reforço, se necessário
        └── diario.md            ← suas anotações sobre o tópico
```

## Como começar

Peça à sua IA:

```text
Iniciar tópico "[nome do tópico]" da Fase [número].
```

Veja o ciclo completo em `.tutor/fluxo-de-estudo.md` e um exemplo já preenchido em `.tutor/exemplos/exemplo-ciclo-topico-logica/`.

Esta pasta começa vazia — ela se preenche conforme você avança no roadmap.
