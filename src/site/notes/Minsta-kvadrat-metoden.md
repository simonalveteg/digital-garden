---
{"dg-publish":true,"permalink":"/minsta-kvadrat-metoden/","tags":["matematiskstatistik"]}
---

$$
Q(\theta)=\sum\limits_{i=1}^{n}(x_i-\mu_i(\theta))^{2}
$$
är summan av kvadraterna på observationernas avvikelser från väntevärdena. $x_i-\mu_i(\theta)$ är det erhållna försöksfelet för den $i$:te observationen om $\theta$ vore det korrekta parametervärdet. Idén är att som $\theta$-[[Punktskattning\|skattning]] ta det $\theta$-värde som gör summan av kvadraterna på avvikelserna så liten som möjligt.

Det värde $\theta_{obs}^{*}$ för vilket $Q(\theta)$ antar sitt minsta värde inom $\Omega_\Theta$ kallas MK-skattningen av $\theta$.

MK-metoden kan generaliseras
1. Fördelningen innehåller $k$ okända parametrar $\theta_{1},\theta_{2},\dots,\theta_k$. Uttrycket $Q$ blir då en funktion av dessa paramarar, och man mestämmer en [[Punktskattning\|skattning]] för var och en så att $Q$ blir så litet som möjligt.
2. Värdena $x_{1},\dots,x_n$ är obserationer av [[Stokastisk Variabel\|s.v.]] $X_{1},\dots,X_n$ med olika fördelningar som beror av samma okända parameter eller parametrar.

MK-metoden ger i regel inte samma resultat som [[Maximum-likelihood metoden\|ML-metoden]]. Eftersom [[Maximum-likelihood metoden\|ML-metoden]] ger skattningar med goda egenskaper, bör mestadels MK-metoden få stryka på foten, utom möjligen då ML-skattningen är svår att numeriskt bestämma. MK-metoden har dock den mycket stora fördelen att fördelningen inte behöver vara helt känd.