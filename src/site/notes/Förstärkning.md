---
{"dg-publish":true,"permalink":"/foerstaerkning/","tags":["analogelektronik"]}
---


$$A_{t}=\frac{Q_L}{Q_{g}}$$
Q = quantity (eftersom det kan vara både spänning och ström), L = load, g = generator. 

Den verkliga förstärkningen $A_t$ skiljer sig från den [[Asymptotisk Förstärkning\|asymptotiska förstärkningen]] med en **[[Diskrepansfaktor\|diskrepansfaktor]]**. 

$$
A_{t}=A_{t\infty} \frac{-A\beta}{1-A\beta} + A_{t0}\frac{1}{1-A\beta} \approx A_{t\infty}\frac{-A\beta}{1-A\beta}
$$
men man kan försumma sista termen om [[Slingförstärkning\|slingförstärkningen]] är tillräckligt stor. 

Vi vet (eller kan enkelt lista ut) A. Om vi har *en* [[Transistor\|transistor]] och använder den som en [[Förstärkare\|förstärkare]] så är $A=g_{m}$. $\beta = Q_{i}/Q_{c}$ när $Q_{s}=0$.

![superpositionsmodellen.png](/img/user/images/superpositionsmodellen.png)

### Beräkningsflöde av $A_t$
1. Beräkna $A_{t\infty}$ med en nullorkoppling
2. Beräkna [[Slingförstärkning\|slingförstärkningen]] i $A\beta$ i den verkliga kopplingen
3. Beräkna den verkliga förstärkningen $A_{t}$

# Frekvensbeteende 
[[Slingförstärkning\|Slingförstärkningen]] är [[Frekvensberoende\|frekvensberoende]], alltså måste även $A_{t}$ vara det (enligt definitionen), om $\beta$ är [[Frekvensberoende\|frekvensberoende]]. Det beror på hur [[Frekvenskompensering\|frekvenskompenseringen]] implementarats i [[feedback\|återkopplingsnätet]]. 

Högfrekvensbeteendet undersöks genom att 
1. Beräkna högfrekvensbeteendet hos $A \beta$
2. Undersöka hur frekvensbeteendet hos [[Diskrepansfaktor\|diskrepansfaktorn]] påverkas av $A \beta$
3. Undersöka eventuellt [[Frekvensberoende\|frekvensberoende]] i $A_{t\infty}$.
