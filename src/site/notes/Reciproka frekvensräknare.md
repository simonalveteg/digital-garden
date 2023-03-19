---
{"dg-publish":true,"permalink":"/reciproka-frekvensraeknare/","tags":["mätteknik"]}
---

Reciproka [[Frekvensräknare\|frekvensräknare]] klarar av att mäta frekvensen enligt $f=N/T_{n}$. $T_n$ mäts genom att räkna antalet klockpulser från den inbyggda tidbasoscillatorn. $N$ måste vara ett heltal enligt definitionen, därför synkroniseras mätningen med insignalen ($T_{n}$ och $N$). Det finns ingen grindtid, bara synkroniseringslogik. När man börjar mäta inväntas nästa [[Triggning\|triggning]] innan mätningen stoppas. Eftersom att den är synkroniserad med insignalen är vi då säkra på att ett exakt antal ingångscykler mäts. 

Innehållet i räknekedjorna överförs till mikroprocessorn, som med hjälp av sitt program beräknar insignalens frekvens som kvoten $\frac{N}{T_{n}}$. 

Metoden kallas reciprok eftersom man mäter frekvensens reciproka värde (periodtiden). 

> Mätosäkerhet på $\pm1$ **klockcykel**. Start och stopp av räknekedjorna är synkroniserade med ingångssignalen, men mätningen är fortfarande totalt osynkroniserad med klockpulserna. Det leder till att delar av klockpulsperioder ibland räknas och ibland inte.

![reciprok räknare.png](/img/user/images/reciprok%20r%C3%A4knare.png)