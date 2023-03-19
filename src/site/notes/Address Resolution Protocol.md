---
{"dg-publish":true,"permalink":"/address-resolution-protocol/","tags":["kommunikationssystem"]}
---

ARP är ett [[Network Layer\|nätverksprotokoll]] används för att hitta MAC-adressen för en värddator om man vet dess IP-adress. Det är ett hjälpprotokoll till [[Internet Protocol\|IP]] som lligger mellan [[OSI model\|OSI]] lager 2 och 3. Det finns ingen IP-header när ARP används.

I [[IPv4\|IPv4]] är ARP ett eget protokoll, men i [[IPv6\|IPv6]] ingår funktionen i ICMPv6.

An ARP request contains four addresses
1. Sender Hardware Address
2. Sender Protocol Address
3. Target Hardware Address 
4. Target Protocol Address - set to all zeros

An ARP reply contains the same four addresses, but with the last two no longer set to zero.

