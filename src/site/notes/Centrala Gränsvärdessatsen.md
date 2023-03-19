---
{"dg-publish":true,"permalink":"/centrala-graensvaerdessatsen/","tags":["matematiskstatistik"]}
---

Om $X_{1},X_{2},\dots$ är en oändlig följd av [[Oberoende Stokastiska Variabler\|oberoende]] likafördelade [[Stokastisk Variabel\|s.v]]. med [[Väntevärde\|väntevärdet]] $\mu$ och [[Standardavvikelse\|standardavvikelsen]] $\sigma>0$, så gäller för $Y_n=X_{2}+\dots+X_n$ att
$$
P\left( a< \frac{Y_n-n\mu}{\sigma \sqrt{ n }}\leq b \right) \rightarrow \Phi(b)-\Phi(a) \text{  då } n\rightarrow\infty
$$
observera att $E(Y_n)=n\mu$ ([[Väntevärde\|Väntevärde]]) och $D(Y_n)=\sigma\sqrt{ n }$ ([[Standardavvikelse\|Standardavvikelse]]).

När $n$ växer mot oändligheten kommer hela fördelningen för den angivna standardiserade variabeln att gå mot en [[Standardiserad Normalfördelning\|standardiserad normalfördelning]]

Följande definition är praktisk när man arbetar med [[Stokastisk Variabel\|s.v]] som uppfyller centrala gränsvärdessatsen:

> Om $Z_n$, $n=1,2,\dots$ är en oändlig följd av [[Stokastisk Variabel\|s.v]]. och man kan finna tal $A_n$ och $B_n$ , $n=1,2,\dots$ sådana att 
> $$P\left( a< \frac{Z_n-A_n}{B_n}\leq b \right)\rightarrow \Phi(b)-\Phi(a) \text{ då } n\rightarrow\infty$$
> säges $Z_n$ vara asymptotiskt [[Normalfördelning\|normalfördelad]] med parametrarna $A_n$ och $B_n$, eller kortare
> $$Z_N\in AsN(A_n,B_n).$$

det följer att om $X_{1},X_{2}\dots$ är en följd av [[Oberoende Stokastiska Variabler\|oberoende]] likafördelade [[Stokastisk Variabel\|s.v]]. med [[Väntevärde\|väntevärdet]] $\mu$ och [[Standardavvikelse\|standardavvikelsen]] $\sigma>0$ så gäller att $(X_{1}+\dots+X_n)/n \in AsN(\mu,\sigma/\sqrt{ n })$.

> Under allmänna villkor gäller att summan av många ungefär oberoende och ungefär likafördelade [[Stokastisk Variabel\|stokastiska variabler]] är approximativt [[Normalfördelning\|normalfördelad]].