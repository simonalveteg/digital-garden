---
{"dg-publish":true,"permalink":"/normalapproximationen/","tags":["matematiskstatistik"]}
---

Icke-normala fördelningar kan ofta hanteras med ungefär samma teknik som normala, förutsatt att stickproven är någorlunda stora.

Antag att man på grundval av ett eller flera slumpmässiga stickprov har beräknat en [[Punktskattning\|punktskattning]] $\theta^{*}$ av en okänd parameter $\theta$. Antag vidare att denna [[Punktskattning\|skattning]] är ungefär [[Normalfördelning\|normalfördelad]] med [[Väntevärde\|väntevärdet]] $\theta$ och [[Standardavvikelse\|standardavvikelsen]] $D$. Då är
$$
\begin{align}
I_\theta&=(\theta_{\text{obs}}^{*}-\lambda_{\alpha/2}D,\theta_{\text{obs}}^{*}+\lambda_{\alpha/2}D) & \text{om } D \text{ ej beror av }\theta \\
I_\theta&=(\theta_{\text{obs}}^{*}-\lambda_{\alpha/2}d,\theta_{\text{obs}}^{*}+\lambda_{\alpha/2}d) & \text{om } D \text{ beror av } \theta
\end{align}
$$
(och $d$ väljs lämpligt) ett [[Konfidensintervall\|konfidensintervall]] för $\theta$ med den approximativa [[Konfidensgrad\|konfidensgraden]] $1-\alpha$.

> I regel torde dock stickprov på ca 20 värden kunna analyseras med denna metodik.


Två specialfall är
$$
\begin{align}
I_\mu=(\overline x-\lambda_{\alpha/2}D,\overline x+\lambda_{\alpha/2}D) & \text{ om } \sigma \text{ känt } (D=\sigma/\sqrt{ n }) \\
I_\mu=(\overline x-\lambda_{\alpha/2}d,\overline x+\lambda_{\alpha/2}d) & \text{ om } \sigma \text{ okänt } (d=s/\sqrt{ n }) 
\end{align}
$$
där $s=\sqrt{ \frac{Q_{1}+Q_{2}}{(n_{1}-1)+(n_{2}-1)} }$ och $d=s\sqrt{ 1/n_{1}+1/n_{2} }$.