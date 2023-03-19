---
{"dg-publish":true,"permalink":"/carrier-sense-multiple-access/","tags":["kommunikationssystem"]}
---

Man måste lyssna på kanalen innan man börjar skicka iväg [[Framing\|ramar]]. Så fort kanalen verkar vara ledig får man börja skicka. 

Vulnerable time = Propagation time. Det finns en viss tid mellan två punkter där även om två olika datorer inte känner att någon annan sänder kan någon redan ha börjat sända, bara att den dator som är längre bort inte har hunnit få [[Signal\|signalen]] än. Det leder till kollisioner.


### CSMA with Collision Detection
Each user monitors the medium after sending a [[Framing\|frame]], aborts transmission and sends a jamming [[Signal\|signal]] if collision is detected. 

Kollisioner detekteras genom att terminalen hela tiden observerar länken (carrier sense). Om amplituden plötsligt blir högre än den ska vara så vet den att det är två signaler som skickas samtidigt och slutar omedelbart sända, väntar en viss tid innan den börjar sända igen. Blir det kollision igen dubbleras tiden som den väntar (exponential back-off).

För att CSMA/CD ska fungera måste transmissionstiden vara mer än två gånger så lång som utbredningstiden $t_U$ (round trip time). 
$$
t_T > 2\cdot t_U
$$
Om den inte är det kommer man inte kunna detektera kollisionerna, då amplituden vid terminalen i worst case inte kommer vara högre än den ska vara. Worst case är alltså när mottagaren också börjar sända, fast först precis innan sändarens signal har kommit fram. Mottagaren kommer direkt inse att det är en kollision och sluta sända, men om sändaren redan har slutat sända kommer den aldrig att upptäcka att det blivit en kollision.

Transmissionstiden är tiden för att skicka iväg en ram med storlek $s$ med transmissionshastigheten (bit rate) $b$. 
$$
t_T=\frac{s}{b}
$$
