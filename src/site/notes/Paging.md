---
{"dg-publish":true,"permalink":"/paging/","tags":["datorteknik"]}
---


Genom att dela in ett program i sidor (pages) och det fysiska [[Computer Data Storage\|minnet]] i ramar där sidor och ramar är lika stora, och använda en sid-tabell så blir man av med [[Fragmentering\|fragmentering]].

Man har dock fördubblat mängden tid som krävs vid läsning av adresser. Lösningen till detta är att använda [[Cacheminne\|Cacheminne]] - Translation Look-Aside Buffer (TLB) för sidtabeller.

![Pasted image 20230215170137.png](/img/user/images/Pasted%20image%2020230215170137.png)

# Demand Paging
Om man endast laddar de pages som behövs till primärminnet kan man ha flera program igång samtidigt.