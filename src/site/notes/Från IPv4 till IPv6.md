---
{"dg-publish":true,"permalink":"/fran-i-pv4-till-i-pv6/","tags":["kommunikationssystem"]}
---

Det kommer ta lång tid innan vi kan övergå helt till IPv6, då *alla* värddatorer och routrar måste uppdateras till att använda det istället för [[IPv4\|IPv4]]. IETF har definierat tre strategier för övergångsperioden.

# Dual stack
Innebär att en värddator implementerar både [[IPv4\|IPv4]] och IPv6 under övergångsperioden. Om mottagaren har en IPv6 används det annars används [[IPv4\|IPv4]]. Två [[Network Layer\|nätprotokoll]] körs alltså samtidigt på värddatorn. I ett nät där värddatorerna använder dual stack måste också alla routrar kunna hantera både [[IPv4\|IPv4]] och IPv6.

# Tunnelling
Ska användas när ett IPv6-datagram måste passera ett nät som bara har implementerar [[IPv4\|IPv4]]. Det kapslas in i ett [[IPv4\|IPv4]] datagram, med adresser som motsvarar tunnelns ändpunkter i det specifika nätet. För att man skall veta att det är ett IPv6-datagram som skickas med [[IPv4\|IPv4]] sätter man protokollfältet i IPv4-headern till 41.

# Header Translation
Ska användas när större delen av internet gått över till IPv6. Routern översätter IPv6-headern till en IPv4-header när det finns en enhet som inte stödjer IPv6.