---
{"dg-publish":true,"permalink":"/internet-control-message-protocol/","tags":["kommunikationssystem"]}
---

ICMP är ett hjälpprotokoll till IP på [[Network Layer\|Network Layer]]. [[Internet Protocol\|IP]] saknar både feldetektering, felkorrigering och hjälpfunktioner. ICMP kompenserar i viss mån för dessa svagheter i IP. ICMP-meddelanden kapslas in i IP-datagram som sedan ansvarar för att ICMP-meddelanden når önskad destination.

# ICMP
Består av en header på 8 byte och en datadel som är variabel. 

## Typer av meddelanden

### Felmeddelanden (error reporting messages)
Skickas av routrar eller värddatorer när ett problem uppstr med ett IP-datagram. Felmeddelandet skickas alltid till den ursprungliga sändaren. ICMP har inga funktioner för felhantering, utan rapporterar endast när ett fel uppstår. Det finns fyra typer av felmedelanden

- Destination Unreachable (Typ = 3)
	Routern kan inte hitta mottagaren
- Source Quench (Typ = 4)
	Vid överbelastning. Talar om för sändaren att datagrammet har kastats och att det är överbelastning, dvs att den borde skicka data långsammare.
- Time Exceeded (Typ = 11)
- Parameter Problem (Typ = 12)

### Förfrågningar (query messages)
Skickas från en användare, värddator eller [[Router\|router]] tll en mottagande [[Router\|router]] eller värddator. 

- Echo request (Typ = 8)
	Kontrollera m två enheter kan kommunicera med varandra.
- Timestamp request (Typ = 13)
	Hitta round-trip-time (RTT). KAn också användas för att synkronisera två klockor.
- Address-mask request (Typ = 17)
	Används för att hitta ens IP-adressmask.
- Router solicitation (Typ = 10)
	Används av en värddator för att se om dess routrar fungerar.

# ICMPv6
Skiljer sig till viss del i funktionalitet. ICMPv6 inkluderar funktionerna som finns i [[Address Resolution Protocol\|ARP]] och IGMP för [[IPv4\|IPv4]]. 

Felmeddelandet *Source Quench* är borttaget då det finns andra ufnktioner i IPv6 som tar hand om det. *Packet too big* är ett nytt felmeddelande, då endast sändaren får utföra [[Fragmentering\|Fragmentering]] i IPv6.

Förfrågningarna *Timestamp request* och *Adress-mask request* är också borttagna då andra funktioner i IPv6 sköter det. Två nya förfrågningar har lagts till. [[Address Resolution Protocol\|ARP]] ersätts av ICMPV6 *neighbor solicitation* och *neighbor advertisement*.

