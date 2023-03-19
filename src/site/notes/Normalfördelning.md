---
{"dg-publish":true,"permalink":"/normalfoerdelning/","tags":["matematiskstatistik"]}
---

![Pasted image 20221123103622.png](/img/user/images/Pasted%20image%2020221123103622.png)
Normalfördelningen användes ofta för beskrivning av variatinoen hos olika företeelser, och stora delar av statistikteorin bygger på denna fördelning. [[Centrala Gränsvärdessatsen\|Centrala Gränsvärdessatsen]] säger att summan av många (mer än 30) ungefär oberoende felkällor som är av samma storleksordning blir approximativt normalfördelad. Normalfördelningen är även enkel att hantera matematiskt. 

Dess [[Täthetsfunktion\|Täthetsfunktion]] är 
$$
f_X(x)=\frac{1}{\sigma\sqrt{ 2\pi }}e^{-(x-\mu)^{2}/2\sigma^{2}}
$$
och har [[Fördelningsfunktion\|fördelningsfunktionen]]
$$
F_X(x)=\frac{1}{\sigma\sqrt{ 2\pi }}\int\limits_{-\infty}^{x} e^{-(t-\mu)^{2}/2\sigma^{2}} \, dt 
$$
och brukar betecknas $X\in N(\mu,\sigma)$, där $\mu$ är [[Väntevärde\|väntevärdet]] och [[Standardavvikelse\|standardavvikelsen]].

# Allmän Normalfördelning

När man arbetar med en allmän normalfördelning är det ofta bekvämt att använda
$$
f_X(x)=\frac{1}{\sigma}\varphi \left( \frac{x-\mu}{\sigma} \right)
$$
och
$$
F_X(x)=\Phi \left( \frac{x-\mu}{\sigma} \right) 
$$
där $\varphi$ och $\Phi$ ges av [[Standardiserad Normalfördelning\|Standardiserad Normalfördelning]].

Om $X\in N(\mu,\sigma)$ så gäller att
1. $E(X)=\mu$
2. $V(X)=\sigma^{2}$
3. $D(X)=\sigma$
(se [[Väntevärde\|Väntevärde]], [[Varians\|Varians]], [[Standardavvikelse\|Standardavvikelse]])

[[Linjärkombinationer av oberoende normalfördelade stokastiska variabler\|Linjärkombinationer av oberoende normalfördelade stokastiska variabler]]
