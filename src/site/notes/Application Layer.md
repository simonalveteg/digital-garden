---
{"dg-publish":true,"permalink":"/application-layer/","tags":["kommunikationssystem"]}
---


![nätverksapplikationer.png](/img/user/images/n%C3%A4tverksapplikationer.png)

## Client-server paradigm
I en typisk internet-konfiguration har vi en server någonstans som väntar på användare.
![clientserverparadigm.png](/img/user/images/clientserverparadigm.png)
## Peer to Peer Paradigm
Peer to peer är ett alternativ till Client-Server Paradigm där användarna pratar med varandra istället. Fördelen är att hela systemet inte går ner om servern går ner. Torrents är en variant av P2P, där man laddar ned en fil från flera olika användare.
![peertopeerparadigm.png](/img/user/images/peertopeerparadigm.png)

## World Wide Web
World Wide Web (WWW) är en applikation som använder ett protokol (HTTP) för att prata med en server.
	Universal Resource Locator (URL)
	HyperText Transfer Protocol  (HTTP)

### Universal Resource Locator
protocol://host:port/path

### Hypertext Transfer Protocol
Ett text-baserat protokol som anger en sida och ger lite "kommandon" till servern. Startar och använder en [[TCP\|TCP]] anslutning. Har requests och responses.
