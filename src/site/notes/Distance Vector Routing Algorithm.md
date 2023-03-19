---
{"dg-publish":true,"permalink":"/distance-vector-routing-algorithm/","tags":["kommunikationssystem"]}
---

Använder sig av [[Bellman-Fords algorithm\|Bellman-Fords algorithm]].

In this routing algorithm the best path info is shared locally. To begin with each [[Router\|router]] has a table with the cost of its paths. Nearby routers then tell each other what their tables look like, so that each [[Router\|router]] can get an overview of the network. Varje nät berättar för sina närmaste grannar hur dess eget träd/tabell/vektor ser ut enom att skika ett updpateringsmedelande, även kallat annonsering. The table gets updated for new entries and for cost changes. 

Om en nod plötsligt försvinner kommer dess grannar upptäcka det vid nästa annonseringstillfälle och ta bort den från sin tabell/vektor, de tar även bort rader där den noden hade varit nästa nod. Vid nästa tillfälle kan de skicka sina uppdaterade tabeller till sina grannar.

Kan sammanfattas med det engelska uttrycket "good news travel fast, bad news travel slow" efterom att det tar längre tid att vidarebefordra information om fel i nätverket. I extrema fall kan det ta flera annonseringsperioder att upptäcka fel. Det kan dessutom uppstå ghost-vägar pga detta. T.ex om A försvinner och C tar bort den, men innan C hinner skicka en uppdatering skickar F sin periodiska vektor som innehåller A. Till slut tror C att den kan nå A via F, vilket är helt fel.

# Initial routing tables example
![Pasted image 20230214155145.png](/img/user/images/Pasted%20image%2020230214155145.png)
when the [[Router\|router]] gets info about new destinations, it also saves the [[Router\|router]] that gave it the lowest cost for that destination in the "next" column. 
![Pasted image 20230214155356.png](/img/user/images/Pasted%20image%2020230214155356.png)
Noden kommer bara bearbeta tabellen från en annan nod i taget.

See also -> [[Routing Algorithms\|Routing Algorithms]]