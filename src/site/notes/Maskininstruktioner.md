---
{"dg-publish":true,"permalink":"/maskininstruktioner/","tags":["datorteknik"]}
---

Högnivåspråk omvandlas till assembly som omvandlas till maskininstruktioner.

Operationskod = Vad ska göras
Source Operander = Varifrån ska vi hämta information?
Destination Operand = Var ska resultatet hamna?
Hur fortsätter vi efter instruktionen?

Typer av instruktioner
- Aritmetiska och logiska ([[Arithmetic Logic Unit\|ALU]])
- [[Addressering\|Addressering]]
- [[Hoppinstruktioner\|Hoppinstruktioner]]
- In- och utmatning

# Antal adresser i en instruktion
För 4-adress instruktioner specifierar man i varje instruktion vilken nästa instruktion är. Det är mycket vanligare med 3-adress instruktioner där man helt enkelt antar att nästa instruktion är på nästa rad. 

4-adress instruktioner:
```
ADD X, A, B, i2
MUL X, X, C, i3
```

3-adress instruktioner:
```
ADD X, A, B
MUL X, X, C
```

2-adress instruktioner:
```
MOVE A, X
ADD X, B
MUL X, C
```

1-adress instruktioner:
```
LOAD A
ADD B
MUL C
STORE X
```
värden lagras i en ackumulator.

# Instruktionsformat

Med ett Fixed instruktionsformat är alla instruktioner lika långa. Då kan kontrollenheten göras lite lättare, då den vet exakt hur lång instruktionen kommer vara.

Med ett Flexibelt instruktionsformat kan instruktionerna ha olika längd. Det ger en större flexibilitet.