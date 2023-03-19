---
{"dg-publish":true,"permalink":"/state-assignment/","tags":["digitalteknik"]}
---


State assignment = tillståndskodning
Tillståndskodning berör hur man väljer vad man ska kalla varje tillstånd. Det finns inga kända metoder för att ta fram en *optimal* tillståndskodning.

## Metoder
1. Hitta beroenden mellan tillstånden med [[Reduced Dependency Algorithm\|Reduced Dependency Algorithm]], och välj tillståndskodning efter det
2. Skriv upp alla tillstånd så att tillstånd med övergångar ligger efter varandra (så gott det går). Koda sedan med [[Graykod\|Graykod]]

Använder ett streck ovanför tillstånden i varje block, inte samma sak som [[State Minimization\|State Minimization]] där man använder {}.