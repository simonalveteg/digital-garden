---
{"dg-publish":true,"permalink":"/reduced-dependency-algorithm/","tags":["digitalteknik"]}
---

En sorts [[State Assignment\|State Assignment]] där man för varje par av tillstånd:

1. Antar att de tillhör samma block
2. Iterativt, för varje insignalskombination, grupperar nästa tillstånd hos ett block till ett nytt block. Om ett tillstånd finns i flera block måste dessa slås ihop till ett block.

![Pasted image 20211026121248.png](/img/user/images/Pasted%20image%2020211026121248.png)

## Mål: 
Man vill typ få fram två olika "reduced dependencies". Om man har sex block kan man ha två med tre tillstånd i varje, och tre med två tillstånd i varje. Sen parar man ihop dessa i en 3x2 tabell och väljer q1q2q3 (valfritt sätt).