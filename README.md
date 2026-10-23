# *O Noddy Vai À Piscina*
## Introdução ao jogo
 Chegou o verão e o Noddy tem andado a implorar aos pais para ir à piscina municpal, porque nessa piscina costuma haver uma banca de gelados. Mas os pais só deixam o Noddy comer o gelado depois de Noddy concluir um desafio que os pais o propõem, já que os pais querem que Noddy aprenda a nadar. O Noddy pode encontrar itens na piscina que o vão beneficiar durante o desafio. O objetivo de Noddy é conseguir coletar todas as argolas que estão espalhadas pela piscina inteira e assim será recompensado com um gelado. Se Noddy não conseguir coletar todas as argolas, um Nadador Salvador salva o Noddy de se afogar e o jogo recomeça.

 ![Noddy no Verão](https://i.ytimg.com/vi/FeaClNpAIWo/maxresdefault.jpg) 

# Personagens ou itens

## Personagens
- Noddy
- Nadador Salvador
- Mae 


### Itens 

| Item | Efeito | Quando é mais útil |
|------|--------|--------------------|
|Óculos de nadar | Aumentam a visão debaixo de água | Quando as argolas são difíceis de ver ou estão espalhados |
| Barbatanas | Aumentam a velocidade a nadar | Quando os objetos estão longe uns dos outros |
| Argola | Objetivo do jogo | Quando o noddy apanha todas as argolas o hoje termina |
| Gelado | Recompensa | É Obtido quando todas as argolas sao apanhadas sendo esta a recompensa de conclusão |

## História/Enredo

O jogo passa-se na cidade dos brinquedos onde o noddy vive com os seus pais. o noddy gosta de ir a uma piscina especifica na cidade dos brinquedos porque nessa mesma piscina têm uma banca de gelados onde o noddy adora ir. Num dia quente de verão Noddy pede aos pais para ir à piscina. Os 3 vão à piscina, ao chegar,noddy pede à mãe um gelado, mas a mãe lança um desafio a noddy. Esse desafio consiste em apanhar todas as argolas que estão dentro da piscina e aí receberá o gelado. Noddy conseguiu completar o desafio e recebeu o seu gelado e foram os 3 felizes para casa.

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