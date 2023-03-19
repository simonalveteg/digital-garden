---
{"dg-publish":true,"permalink":"/dynamic-host-configuration-protocol/","tags":["kommunikationssystem"]}
---

Dynamic Host Configuration Protocol är ett protokoll som används av en dator för att få en IP-adress, samt information om närmaste [[Router\|router]] som kopplar ut mot Internet (default gateway) och [[Domain Name System\|DNS-server]]. När en ator startar upp går den igenom en *bootstrap-process* där den skickar ut ett DHCP DISCOVER meddelande med broadcast. Ansvarig DHCP-server svarar med DHCP OFFER meddelande som innehåller en IP-adress samt annan information. Datorn skickar då ett DHCP REQUEST meddelande där den behär tillstånd att få använda den erbjudna adressen, varpå DHCP-servern svarar med ett DHCP ACKNOWLEDGEMENT. Adressen får användas under en begränsad tid (lease-time) och datorn måste begära en re-lease när halva tiden gått.

I IPv6-nät används istället [[DHCPv6\|DHCPv6]]