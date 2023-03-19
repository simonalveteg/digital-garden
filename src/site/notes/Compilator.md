---
{"dg-publish":true,"permalink":"/compilator/","tags":["datorteknik"]}
---

Varje processor har en egen kompilator. Kompilatorn tar indata (högnivåspråk) och genererar assembly instruktioner för processorn. Kompilatorn kan bara generera dem instruktioner som processorn har, och om processorn inte stödjer en instruktion (ex multiplikation) så får man lösa det på något annat sätt (ex generera ett program som utför multiplikation genom addition). Ju bättre kompilatorn är, desto färre assembly-instruktioner.

[Compiler Explorer (godbolt.org)](https://godbolt.org/)
