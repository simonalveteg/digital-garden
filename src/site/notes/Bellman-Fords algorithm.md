---
{"dg-publish":true,"permalink":"/bellman-fords-algorithm/","tags":["kommunikationssystem"]}
---


I Bellman-Fords algoritm itererar man fram den lägsta kostnaden från en nod till andra noder i grafen genom att upprepat räkna ut kostnaden för att ta sig från en nod via en båge till nästa nod. Man börjar med att skapa en lista över alla bågar och sätter kostnaden för utgångsnoden (roten) till 0 och kostnaden för alla andra noder i grafen till oändligheten. Sen gör man $n$ stycken iterationer, där $n$ är lika med antal noder i grafen minus 1. 