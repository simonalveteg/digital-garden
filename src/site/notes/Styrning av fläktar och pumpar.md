---
{"dg-publish":true,"permalink":"/styrning-av-flaektar-och-pumpar/","tags":["elenergiteknik"]}
---

Asynkronmotorer används för att driva fläktar och pumpar, ex i ventilationssystem och cirkulationspumpar. Det är den vanligaste tillämpningen av motordrifter. Andelen av vår energiförbrukning som går till motordrifter är stor, därför är det viktigt att [[Energi\|energin]] utnyttjas på bästa möjliga sätt. Ofta vill man kunna variera flödet för att inte förflytta för mycket vätska eller ventilera onödigt mycket. Det kan ske på två sätt

1. Konstant hastighet: Motorn körs på konstant varvtal och flödesvariation åstadkoms genom att flödet stryps med någon form av ventil eller spjäll.
2. Variabel hastighet: Man varierar motorns varvtal vilket varierar flödet genom pumpen eller fläkten.

Sambandet mellan flödet genom en pump och trycket som den kan åstadkomma kan beskrivas med en *pumpkurva*. Maximalt flöde fås när mottrycket är noll och det maximala trycket fås när flödet är noll. För pumpens belastning gäller det omvända, dvs mottrycket ökar med ökat flöde. Oftast kan belastningen beskrivas av en kvadratisk funktion. [[Arbetspunkt\|Arbetspunkten]] bestäms av skärningen mellan de två kurvorna. Effekten som behövs beräknas som

$$
P=H\cdot Q
$$
där $H$ är tryckskillnaden mellan före och efter pumpen som uppkommer vid flödet $Q$.

![Pasted image 20230223141905.png](/img/user/images/Pasted%20image%2020230223141905.png)

Om man väljer att minska flödet genom att minska pumpens varvtal byter man från en pumpkurva till en annan. Det motsvarar en förflyttning från arbetspukt A till B i bilden nedan. Effekten till pumpen blir mycket lägre med denna metod jämfört med strypning, och är mycket effektiv.

![Pasted image 20230223142233.png](/img/user/images/Pasted%20image%2020230223142233.png)