---
{"dg-publish":true,"permalink":"/flerstegsfoerstaerkare/","tags":["analogelektronik"]}
---

om vi inte får tillräckligt bra precision i vår överföring så måste vi lägga till fler [[Förstärkande Steg\|förstärkande steg]].

Varje steg kan teoretiskt maximalt bidraga med faktorn $\beta_f$ till [[Förstärkning\|slingförstärkningen]] ($A \beta$). Om vi har ett precisionskrav på att slutna [[Förstärkning\|förstärkningen]] $A_{t}$ ska avvika max x% från den [[Förstärkning\|asymptotiska förstärkningen]] ($A_{t\infty}$) ger detta krav på [[Slingförstärkning\|slingförstärkningen]]. Om då $|A \beta| > \beta_{f}$ måste flera [[Förstärkande Steg\|förstärkarsteg]] användas.

De förstärkande stegen får inte kortsluta [[feedback\|återkopplingsnätverket]], dvs man måste ha minst ett [[Antiseriesteget\|AS-steg]] om [[feedback\|återkopplingsnätet]] inte föreser [[Nullor\|nullorn]] med en gemensam in- och utgång. 

[[Förstärkande Steg\|Förstärkande steg]] kopplas efter varandra i [[Nullor\|nullorn]], så att föregående stegs utgångsport ansluts till efterföljande stegs ingångsport. 

Kombinationen av steg måste ge [[Negativ Återkoppling\|Negativ Återkoppling]]! 
- Sätt polariteten på ingången och gå sen steg för steg och sätt ut plus- och minustecken (stegen är inverterande eller inte) (se bild)
	- ![steg i strömförstärkare.png|300](/img/user/images/steg%20i%20str%C3%B6mf%C3%B6rst%C3%A4rkare.png)

Implementera [[Förstärkare\|förstärkaren]] med teoretiskt minimalt antal steg och beräkna $A \beta$. Kontroller att $|A \beta|$ är större än kravet. Om det inte är det får man lägga till ett steg till och göra om processen.

[[Ingångssteg\|Ingångssteg]]
[[Utgångssteg\|Utgångssteg]]
