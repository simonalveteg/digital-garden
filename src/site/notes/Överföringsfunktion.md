---
{"dg-publish":true,"permalink":"/oeverfoeringsfunktion/","tags":["reglerteknik","analogelektronik"]}
---

The transfer function is a [[Process Models\|process model]]
$$Y(s)=G(s)U(s)$$
where $G(s)$ is the model (the transfer function), $Y(s)$ is the laplace transform of our output and $U(s)$ is the laplace transform of our input.

A transfer function is the laplace transform of the [[Impulssvar\|impulse response]] of a [[Linjära och Tidsinvarianta System\|LTI system]] when you set the initial conditions to zero.


För ett [[Linjära och Tidsinvarianta System\|linjärt tidsinvariant system]] $S$ gäller
$$e^{st}\xrightarrow{S}H(s)e^{st}$$
där överföringsfunktionen ges av$$H(s)=\int_{-\infty}^{\infty}e^{-st}h(t)dt=\mathcal{L}(h(t))(s)$$
där integralen kan tolkas som [[Laplacetransformationer\|laplacetransformen]] av $h(t)$.

Antag att $S$ är [[Linjära och Tidsinvarianta System\|LTI]] och reellt (dvs [[Impulssvar\|impulssvaret]] är reellt). Då är 
1. $S(sin(wt))=A(w)sin(wt+\varphi(w))$
2. $S(cos(wt))=A(w)cos(wt+\varphi(w))$


## [[Differentialekvationer\|Differentialekvationer]]
Om man har en funktion som 
$$y'''+3y'+y=2w''+w$$
blir överföringsfunktionen
$$H(s)=\frac{2s^{2}+1}{s^{3}+3s+1}$$
dvs insignal genom utsignal.


## [[Poler\|Poler]] och [[Nollställen\|nollställen]]
Generellt kan en överföringsfunktion skrivas på formen
![överföringsfunktion.png](/img/user/images/%C3%B6verf%C3%B6ringsfunktion.png)
$n_{1}$, $n_{2}$ osv kallas [[Nollställen\|nollställen]] och $p_1$, $p_2$ osv kallas [[Poler\|poler]].
[[Poler\|Polerna]] och nollställena kan markeras i [[Laplace-planet\|s-planet]]. [[Poler\|Poler]] markeras med x och [[Nollställen\|nollställen]] med o.
![polerochnollställenisplanet.png](/img/user/images/polerochnollst%C3%A4llenisplanet.png)
Förekommer endast i par, och är då konjugat till varandra.

Placeringen av [[Singularitet\|singulariteterna]] i överföringsfunktionen avgör exempelvis om ett [[System (matematisk definition)\|System (matematisk definition)]] är [[Stabila och Instabila System\|stabilt]] eller inte.

> Alla [[Poler\|poler]] till överföringsfunktionen är [[Egenvärden\|egenvärden]] till systemmatrisen och altså egensvängningsfrekvenser till [[System (matematisk definition)\|systemet]]. Om $s=p$ är en [[Poler\|pol]] till $H(s)$ så finns en fri svängning till [[System (matematisk definition)\|systemet]] med tidsberoende av formen $e^{pt}$.

Överföringsfunktionen för ett [[System (matematisk definition)\|System (matematisk definition)]] av andra ordningen med komplexa [[Poler\|poler]] kan skrivas på formen
$$G(s)=\frac{K \omega_{0}^{2}}{s^{2}+2\zeta\omega_{0}s+\omega_{0}^{2}}$$
$\omega_{0}$ är en naturlig parameter som beskriver hur långt avståndet är till origo (i det komplexa talplanet). Den är ett bra mått på hur snabb processen är.
$\zeta$ är den [[Relativ Dämpning\|relativa dämpningen]] (vinkeln i det komplexa talplanet). Den talar om hur mycket det svänger (då vinkeln avgör fördelningen mellan realdel och imaginärdel).

## Se också
[[Transfer Function vs Linear State-Space Model\|Transfer Function vs Linear State-Space Model]]
[[Samband mellan impulssvar och överföringsfunktion\|Samband mellan impulssvar och överföringsfunktion]]
[[Amplitudfunktionen\|amplitudfunktion]]
[[Frekvensfunktion\|Frekvensfunktion]]
[[Fasfunktionen\|fasfunktion]]



