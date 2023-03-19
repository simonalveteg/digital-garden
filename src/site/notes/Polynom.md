---
{"dg-publish":true,"permalink":"/polynom/","tags":["funktionsteori"]}
---

Enklaste (i någon mening viktigaste) exemplen på [[Holomorf\|holomorfa]] funktioner.

Polynomdivision: Fungerar precis lika bra för komplexa polynom. Räkningarna blir besvärligare (men samma metod).
Faktorsatsen: Låt p(z) vara ett polynom. Då är p(a)=0 om och endast om $p(z)=(z-a)q(z)$ för något polynom q. ($deg (q) = deg (p -1)$). Beviset är identiskt som för reella polynom.

## Metoder för att lösa kompexa polynomekvationer
Alt 1:
1. Byt ut z mot x+iy 
2. Sätt upp ett [[Ekvationssystem\|ekvationssystem]]
	1. Realdelen
	2. Imaginärdelen
	3. Absolutbeloppet i kvadrat
Om $z^2=w$ måste $|z|^2=|w|$, vilket ger den tredje ekvationen i [[Ekvationssystem\|ekvationssystemet]] ovan
Alt 2:
1. Kvadratkomplettera
2. Använd PQ-formeln
Alt 3:
1. 



## Uppskattningar
Låt p(z) vara ett polynom av grad n (dvs $a_{n} \neq 0$). 
![Pasted image 20220119095431.png](/img/user/images/Pasted%20image%2020220119095431.png)
när z går mot oändligheten är det alltså oavsett i vilken riktning man går mot oändligheten. Samma sak som i flerdim.
![Pasted image 20220119095820.png](/img/user/images/Pasted%20image%2020220119095820.png)
sista steget utnyttjar [[Triangelolikheten\|Triangelolikheten]].
## Algebrans fundamentalsats
Låt $p(z)$ vara ett icke-konstant polynom. Då finns ett [[Komplexa Tal\|komplext tal]] a så att $p(a)=0$.

Som en konsekvens av algebrans fundamentalsats kan polynom faktoriseras.