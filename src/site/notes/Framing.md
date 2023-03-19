---
{"dg-publish":true,"permalink":"/framing/","tags":["kommunikationssystem"]}
---

The [[Physical Layer\|physical layer]] kan inte skilja på bitar. När vi använder ett protokoll för att skicka en [[Signal\|signal]] använder vi framing (ramar) för att organisera datan. 

![framing.png](/img/user/images/framing.png)

Framing löser många problem, exempelvis
1. Om vi vill hantera fel vill vi begränsa mängden av data. En oändlig ström data är nästan omöjlig att detektera och korrigera fel i. 
2. Om flera användare delar samma medium måste systemet kunna byta mellan dem. 
3. Kan användas som synkroniseringspunkter

Flaggor används för att signifiera start och slut på en ram. [[Bit Stuffing\|Bit Stuffing]] kan användas för att undvika problem med det.

[[Cyclic Redundancy Check\|Cyclic Redundancy Check]]
