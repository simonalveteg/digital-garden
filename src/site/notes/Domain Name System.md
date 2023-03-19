---
{"dg-publish":true,"permalink":"/domain-name-system/","tags":["kommunikationssystem"]}
---

När man skall nå en annan dator på Internet måsåte man veta dess IP-adress. Det är fett wack att behöva komma ihåg massa siffror, så man har skapat Domain Name System där en IP-adress kan få ett symboliskt namn. Man kan dock bara skicka ett IP-datagram till webbservern om man känner till IP-adressen, så applikationsprotokollet behöver kontakta DNS-servern - en globalt distribuerad databas - för att få reda på IPn.

Det ska finnas en DNS-server i varje domän. Om den lokala DNS-servern inte har den aktuella IP-adressen skickar den vidare förfrågan till andra servrar. 

DNS skickas över [[UDP\|UDP]].