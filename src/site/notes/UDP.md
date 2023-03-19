---
{"dg-publish":true,"permalink":"/udp/","tags":["kommunikationssystem"]}
---

User Datagram Protocol är ett [[Transportprotokoll\|Transportprotokoll]] som erbuder en *best-effort*-dataöverföring. Dvs det finns inga felhanterinsfunktioner, utan felkontroll och eventuell omsändning får skötas av applikationen - precis som för [[Internet Protocol\|Internet Protocol]]. 

Applikationerna måste dela upp sin adata i lämpliga [[Packet\|paket]] själv. Det är inte garanterat att paketen kommer fram i rätt ordning.

När man kan leva med att tappa lite data (exempelvis när man ser på en video) kan UDP fungera bättre än [[TCP\|TCP]].

# Datagramformat
UDP är ett message-oriented protocol, dvs data skickas i form av meddelanden. När en applikation lämnar över data till UDP adderas endast en kort header på 8 byte. UDP-paketet (eller UDP-datagrammet) lämnas sedan över till IP. UDP-headern består av:
1. Sändarens portadress
2. Mottagarens portadress
3. Längd: den totala längden på datagrammet (header+data)
4. Kontrollsumma: En 16-bitars kontrollsumma beräknas på UDP-headern, UDP-data samt vissa fält i den IP-header som adderas när datagrammet lämnas över till [[Network Layer\|Network Layer]].