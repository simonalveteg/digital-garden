---
{"dg-publish":true,"permalink":"/reduced-instruction-set-computers/","tags":["datorteknik"]}
---

Det finns ett semantiskt gap mellan högnivåspråk och maskinspråk. Det kan täckas antingen av Reduced Instruction Set Computers eller [[Complex Instruction Set Computers\|Complex Instruction Set Computers]].

Med RISC förenklar man instruktionsuppsättningen och anpassar den till de verkliga kraven ett applikationsprogram har.

## Karaktärsdrag
1. Enkla och få instruktioner
2. Enkla och få adresseringsmöjligheter
3. Fixt instruktionsformat
4. Stort antal register
5. Load-and-store architecture: dela upp instruktioner så att visas gör Load/Store och andra gör ALU-uperation, dvs igna instruktioner finns som lläser från minnet OCH gör ALU operation.

RISC är generellt snabbare än CISC om det framförallt är enkla instruktioner som ska exekveras.

[[RISC vs CISC\|RISC vs CISC]]