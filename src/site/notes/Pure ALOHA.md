---
{"dg-publish":true,"permalink":"/pure-aloha/","tags":["kommunikationssystem"]}
---

Alla skickar när de vill. Om man inte får ett ACK väntar man en random tid innan man får skicka igen. Problemet med Pure [[ALOHA\|ALOHA]] är att om endast en bit överlappar mellan två [[Packet\|paket]] är båda förstörda och måste vänta, [[Slotted ALOHA\|Slotted ALOHA]] var en lösning på det.

Nodernas försök att skicka ramar är [[Poission-Fördelning\|poisson-fördelade]]. Om antalet dataramar genererade under den tiden det tar att skicka en ram är $G$ så är sannolikheten att en sändning lyckas i genomsnitt 
$$
S=Ge^{ -2G }.
$$
Maximal throughput när $G=0.5$, då effektiviteten blir $18.39\%$. Detta kan bevisas genom att ta den partiella derivatan av formeln med avseende på G och sätta den lika med noll.