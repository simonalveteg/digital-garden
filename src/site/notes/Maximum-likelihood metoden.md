---
{"dg-publish":true,"permalink":"/maximum-likelihood-metoden/","tags":["matematiskstatistik"]}
---

Idén bakom ML-metoden är att som [[Punktskattning\|skattning]] av $\theta$ ta det värde som gör våra mätdata så troliga som möjligt. 

Funktionen
$$
L(\theta)=\begin{cases}
P(X_{1}=x_{1},X_{2}=x_{2},\dots,X_n=x_n;\theta) & \text{(diskreta fallet)} \\ \\
f_{X_{1},X_{2},\dots,X_n}(x_{1},x_{2},\dots,x_n;\theta) & \text{(kont. fallet)}
\end{cases}
$$
kallas *likelihood-funktionen* (L-funktionen). I det diskreta fallet anger $L(\theta)$ [[Sannolikhet\|sannolikheten]] att just värdena $x_{1},\dots,x_n$ i stickprovet skall erhållas om $\theta$ vore det sanna parametervärdet. I det kontinuerliga fallet är $L(\theta)$ det värde som den $n$-dimensionella [[Täthetsfunktion\|täthetsfunktionen]] för den [[Stokastisk Variabel\|stokastiska variabeln]] $X=(X_{1},\dots,X_n)$ antar för $x_1,\dots,x_n$.

I L-funktionen låter man argumentet $\theta$ anta alla värden inom parameterrummet $\Omega_\Theta$ och ser efter för vilket väde på argumentet som funktionen blir så stor som möjligt. Det värdet kallas $\theta_{obs}^{*}$ och tas som [[Punktskattning\|skattning]].

> Det värde för $\theta_{obs}^{*}$ för vilket $L(\theta)$ antar sitt största värde inom $\Omega_\Theta$ kallas **ML-skattningen** av $\theta$.

ML_skattningen är under allmänna villkor [[Konsistent Punktskattning\|konsistent]]. Den är inte alltid [[Väntesvärdesriktig Punktskattning\|väntevärdesriktig]] men den är ungefär [[Väntesvärdesriktig Punktskattning\|väntevärdesriktig]] då antalet data är stort. 