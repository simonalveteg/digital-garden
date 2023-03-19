---
{"dg-publish":true,"permalink":"/hoppinstruktioner/","tags":["datorteknik"]}
---

När instruktioner inte bara utförs i ordning behöver man ett sätt att hoppa mellan instruktionsrader. Det är där hoppinstruktioner kommer in.

För att göra hopp till annan del av kod laddar man [[Program Counter\|programräknaren]] med ett nytt värde. Det finns två typer av hopp; 
1. Ovillkorliga hopp
2. Villkorliga hopp

# Ovillkorliga hopp
Kommer ske oavsett vad.

# Villkorliga hopp
Villkor bestäms av flaggor i statusregister. De vanligaste flaggorna är 
- N: 1 om resultatet är negativt 
- Z: 1 om resultatet är noll
- V: 1 om aritmetskt overflow
- C: 1 om carry

Oavsett om hoppet görs eller inte minskar prestandan i en [[Pipelining\|pipeline]] vid villkorliga hopp.

# Återhopp och parameteröverföring
Det finns två alternativ. Det ena är att använda ett antal regiser för att spara återhoppsadress och för parameteröverföring, med fördelen att det är snabbt. Nackdelen är att man behöver [[Register\|register]]. Det andra alternativet är att reservera en del av minnet och skapa en kö som fungerar enligt Last-In First-Out. Fördelen är att minnet är stort, men det är mycket långsammare än [[Register\|register]].

Parameterna förs över genom att registerna överlappar. 