---
{"dg-publish":true,"permalink":"/dijkstras-algorithm/","tags":["kommunikationssystem"]}
---

Utgå från en nod och skriv in dess närmsta grannar + kostnad i en temporär lista. Välj den billigaste och lägg till i den permanenta listan. Lägg till den nya nodens närmsta grannar i den temporära listan. Om det finns dubletter ska den med lägst kostnad sparas. Välj den billigaste igen och lägg till i den permanenta listan, fortsätt så. Exempel nedan.
![Pasted image 20230309141347.png](/img/user/Pasted%20image%2020230309141347.png)

![Pasted image 20230314091458.png](/img/user/images/Pasted%20image%2020230314091458.png)
