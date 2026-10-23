# Project
## Section 1 - Pedro
## Section 2 - Antonio
## Section 3 - Tiago
## Section 4 - Santiago
## Estratégia / Walktrough: *Noody vai à piscina*

### Fluxo geral do jogo

```mermaid
flowchart LR
    A(["Início: o Noddy chega à piscina"]) --> B{"Apanhar itens na borda?"}
    B -- "Sim" --> C["Andar pela borda e apanhar óculos e/ou barbatanas"]
    B -- "Não" --> D["Mergulhar na piscina"]
    C --> D
    D --> E{"Ainda há argolas no fundo?"}
    E -- "Sim" --> F{"Ainda tem tempo debaixo de água?"}
    F -- "Sim" --> G["Nadar até à  próxima argola e apanhá-la"]
    E -- "Não" --> I(["Todas as argolas apanhadas: o Noddy ganha um gelado!"])
```

### Que itens apanhar primeiro?

```mermaid
flowchart LR
    A(["Antes de mergulhar"]) --> B{"As argolas no fundo são fáceis de ver?"}
    B -- "Não" --> C["Apanhar os óculos de nadar"]
    B -- "Sim" --> D{"As argolas estão longe umas das outras?"}
    C --> D
    D -- "Sim" --> E["Apanhar as barbatanas"]
    D -- "Não" --> F["Mergulhar já"]
    E --> F
    F --> G(["Começar a recolha"])
```

**Recomendação:** apanha **sempre os dois itens** antes de mergulhar. Como estão fora de água, não custam tempo de ar, e tornam a parte díficil do jogo muito mais fácil.

## Estratégia debaixo de água

```mermaid
flowchart LR
    A(["Debaixo de água"]) --> B["Olhar à volta e localizar as argolas"]
    B --> C["Escolher a argola mais próxima"]
    C --> D["Nadar até ela e apanhá-la"]
    D --> E{"Falta alguma argola?"}
    E -- "Sim" --> F{"O tempo está a acabar?"}
    F -- "Não" --> C
    F -- "Sim" --> G["Ir direto à argola mais próximas, sem desvios"]
    G --> E
    E -- "Não" --> H(["Vitória: gelado para o Noddy!"])

```