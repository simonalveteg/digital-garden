---
{"dg-publish":true,"permalink":"/dhc-pv6/","tags":["kommunikationssystem"]}
---

DHCPv6 har delvis samma funktion som [[Dynamic Host Configuration Protocol\|DHCP]], men i IPv6 finns det två sätt för en dator att få en IP-adress:

# Stateless autoconfiguration
En dator kan själv konfigurera sig utan hjälp av en server, däremot måsåte den självgenererade lokala adressen, en link local-adress, kontrolleras så att den verkligen är unik på det lokala nätet. Datorn skickar en ICMPv6 Neighbor Solicitation förfrågan på nätet. Om en annan dator redan har adressen skickar den ICMPv6 Neighbor Advertisement. 

# Stateful Configuration
DHCPv6 används på ungefär samma sätt som [[Dynamic Host Configuration Protocol\|DHCP]] för [[IPv4\|IPv4]], fast med nya adresseringstyper och funktioner som är definierade för IPv6.