---
{"dg-publish":true,"permalink":"/classless-addressing/","tags":["kommunikationssystem"]}
---

För att man ska veta vilka adress-bitar i en [[IPv4 Address\|IPv4 Address]] som utgör network-id och vilka som är host-id hör det en så kallad *mask* till varje IP-adress. Masken består av 32 bitar och en etta indikerar att adressbiten på motsvarande plats ingår i network-id och en nolla innebär host-id.

Ett annat sätt är att ange hur mnga ettor som masken består av efter ett "/". Exempelvis anger 128.11.3.31/18 att de första 18 bitarna är network-id.

Om ett nät ska allokera 750 adresser behöver nätmasken ha tillräckligt många nollor för att adresserna ska få plats. 750 är inte en tvåpotens, den minsta som rymmer 750 är 1024, dvs $2^{10}$. Det lämnar 32-10=22 bitar som måste vara ettor i masken. Det ger 255.255.252.0. 252 motsvarar 11111100, och från det kan man få 252 genom att ta $2^8-2^2$.