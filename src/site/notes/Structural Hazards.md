---
{"dg-publish":true,"permalink":"/structural-hazards/","tags":["datorteknik"]}
---


Om två instruktioner vill läsa i minnet samtidigt blir det en strukturell hazard, då det inte går att både läsa in data från primärminnet och samtidigt läsa in en instruktion från primärminnet. Problemet kan lösas genom att fördröja en instruktion.

För att undvika strukturella hazards behöver man undvika minnesaccesser genom att använda register. Genom att öka antalet resurser, genom att exempelvis ha två cache minnen; ett för data och ett för instruktioner. Då kan båda läsas in samtidigt.
![Pasted image 20230131153104.png](/img/user/images/Pasted%20image%2020230131153104.png)

Man kan även ändra ordning på instruktioner för att undvika att använda resultat afrån load i direkt följande instruktion. Kompilatorn kan alltså användas för att minska antal stalls.
![Pasted image 20230131161704.png](/img/user/images/Pasted%20image%2020230131161704.png)
