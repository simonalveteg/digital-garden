---
{"dg-publish":true,"permalink":"/delayed-branching/","tags":["datorteknik"]}
---

Delayed branching är en kompilatorteknik som används för att minska penalties i [[Pipelining\|pipelinen]].

Delayed branching innebär att kompilatorn ändrar ordningen på instruktionerna så att en instruktion läggs efter det villkorliga hoppet. Om man använder delayed branching kommer instruktionen efter hoppet alltid att exekveras, även om hoppet tas. Om ingen instruktion kan flyttas till efter hoppet kommer NOP (no operation) att läggas där och prestandan blir likadan som om man inte använde delayed branching.