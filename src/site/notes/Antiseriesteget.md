---
{"dg-publish":true,"permalink":"/antiseriesteget/","tags":["analogelektronik"]}
---


![Pasted image 20220207142610.png](/img/user/images/Pasted%20image%2020220207142610.png)

om vi har V-V eller I-I så måste vi ha ett [[Förstärkande Steg\|förstärkande steg]] utan sammankoppling mellan in- och utgång. De andra stegen har en terminal gemensam mellan in och utgången, vilket är varför man måste använda ett Antiserie-steg

Två [[Transistor\|transistorer]] kopplas [[Serie- och paralell-kopplingar\|i serie]], men den ena kopplas “upp och ned” - i *antiserie*. [[Transistor\|Transistorerna]] ska vara lika [[Biasering\|biaserade]].

Består av två antiseriekopplade [[GE-steget\|GE-steg]]. Beroende på hur man kopplar kan man välja om det är positiv eller negativ överföring, dvs om den är inverterande eller inte. Det är negativ överföring om man inte korskopplar utgången.

## Småsignalmodell
Har tydliga likheter med hybrid-$\pi$ modellen för [[GE-steget\|GE-steget]], men ingen anslutning mellan in- och utgång. 
![småsignalmodell AS-steg.png|400](/img/user/images/sm%C3%A5signalmodell%20AS-steg.png)
$r_{0}'=r_{\pi 1}+r_{\pi 2}=2r_{\pi}$
$g_{m}'= \frac{g_{m}}{2}$
$r_{0}'=r_{o1}+r_{o2}=2r_{o}$
$g_{m}'r_{\pi}'=\frac{g_{m}}{2}2r_{\pi}=\beta_{f}$ 
$c_{\pi}'=\frac{c_{\pi}}{2}$
$c_{\mu}'=c_\mu$ 
I denna kurs försummas $c_\mu$ och $r_{0}$ om inget annat anges