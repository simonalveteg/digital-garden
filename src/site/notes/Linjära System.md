---
{"dg-publish":true,"permalink":"/linjaera-system/","tags":["systemochtransformer"]}
---


ett [[System (matematisk definition)\|System (matematisk definition)]] $S$ kallas linjärt om 
$$S(c_{1}w_{1}+c_{2}w_{2})=c_{1}S(w_{1})+c_{2}S(w_{2})$$
för alla tal $c_{1}, c_{2}$ och alla insignaler $w_{1}(t), w_{2}(t)$.

> $S$ är linjärt $\Rightarrow S(0)=0$ 

[[Ekvationssystem\|Ekvationssystem]] är [[System (matematisk definition)\|System (matematisk definition)]]. Linjära system innehåller endast addition och multiplikation med konstanter. Elektriska kretsar är en sorts system, då man kan skriva upp [[Ekvationssystem\|ekvationssystem]] som beskriver variablerna i kretsen (ström, spänning). 

En envariabelsfunktion $f(x)=sinx$ avbildar x på sinx. Samma sak gäller för flera variabler (ex med [[Vektorer\|vektorer]] och [[Avbildningsmatris\|avbildnignsmatriser]]). Ett system $S$ är en avbildning som avbildar en insignal på en utsignal, där både insignal och utsignal kan vara vad som helst ([[Vektorer\|vektorer]], funktioner, [[Serier\|serier]], [[Matris\|matriser]] etc). Man kan betrakta system med kontinuerlig tid eller med diskret tid.

Om man lånar pengar från banken (klassiskt exempel) med 2% ränta och $x_{0}$ pengar från början blir $x_{n}=1.02^{n}x_{0}$. Man får ett system som avbildar $x_{0} \rightarrow (x_{0},x_{1},x_{2}...x_{n},...)$ , dvs avbildar ett tal på en [[Serier\|serie]].

>S är linjärt $\Leftrightarrow$ det finns en [[Distributioner\|generaliserad funktion]] ([[Distributioner\|distribution]]) $k(t,\tau)$ så att $$S(w)=\int_{-\infty}^{\infty}k(t,\tau)w(\tau)d \tau$$
>$k(t,\tau)$ kallas [[Impulssvar\|impulssvaret]] av systemet $S$ 


## Test för linjära system
[[Insignal-Utsignalmodeller\|Insignal-Utsignalmodeller]]
testa om $S(0)=0$ och $S(cw)=cS(w)$



[[Tidsdiskreta System\|Tidsdiskreta System]]