---
{"dg-publish":true,"permalink":"/udp-vs-tcp/","tags":["kommunikationssystem"]}
---

Det finns tre huvudsakliga skillnader mellan [[TCP\|TCP]] och [[UDP\|UDP]].
1. UDP är förbindelsefritt och TCP är förbindelseorienterat. Dvs TCP sätter upp en [[Kanal\|kanal]] för utbyte mellan två datorer medan UDP skickar varje [[Packet\|paket]] individuellt.
2. TCP har feldetektering. TCP Använder [[Go-back-N ARQ\|Go-back-N ARQ]] för att kunna begära omsändning av tappade paket. För UDP är ett tappat paket borta. 
3. TCP ser till att paket levereras till högre lager i rätt följd, medan UDP skickar vidare ett paket oberoende av de övriga.

Både web-browsing och nedladdning av filer kräver att den begärda filen kommer fram felfritt, så där är TCP att föredra framför UDP. Det kan uppstå en fördröjning vid omsändningar, men den är oftast inte märkbar för de applikationerna.

Realtidsapplikationer som Voice over IP är ofta mer känsliga för fördröjningar, vilket gör att UDP kan vara att föredra. Det är svårt att koppla upp TCP-förbindelser i en broadcasting situation där samma material ska nå många mottagare, vilket kan underlättas med UDP.