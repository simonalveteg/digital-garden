---
{"dg-publish":true,"permalink":"/stabila-och-instabila-system/","tags":["systemochtransformer","analogelektronik"]}
---


[[System (matematisk definition)\|System (matematisk definition)]] brukar kallas **instabila** om en liten förändring av insignalerna kan leda till ett obegränsat växande av [[Tillståndsvariabler\|tillståndsvariablerna]]. Är ett [[System (matematisk definition)\|System (matematisk definition)]] stabilt å andra sidan så svänger det in sig snabbt. Tänk en pendel, det finns ett fall där den hänger rakt ned, och ett annat fall när den pekar rakt upp. När den hänger rakt ned är det ett stabilt [[System (matematisk definition)\|System (matematisk definition)]], för om man puttar lite på pendeln kommer den svänga in sig själv till samma position. Om den pekar rakt upp däremot behöver man bara peta på den för att den ska falla ned, och aldrig återgå till samma position.

> För stabila [[System (matematisk definition)\|System (matematisk definition)]] går den homogena lösningen mot noll då $t \rightarrow\infty$ 

En rationell fuktion H(s) är överföringen till ett stabilt [[System (matematisk definition)\|System (matematisk definition)]] då 
* Antalet [[Poler\|poler]] ≥ antalet [[Nollställen\|nollställen]]
* Alla [[Poler\|poler]] ligger i vänstra halvplanet
![stabiltellerinstabilt.png](/img/user/images/stabiltellerinstabilt.png)
På vänster sida AVTAR den exponentiella komponenten (det är ett [[Laplace-planet\|laplace-plan]]), medan den ökar på höger vilket ger upphov till instabilitet!! 


# Stabilitet för [[Differentialekvationer\|differentialekvationen]] $\vec{x}'=A \vec{x}+\vec{f(t)}$

$\sigma(A)$ defineras som $max_{1\leq k\leq n}(Re(\lambda_{k}))$ och används för att se om en [[Differentialekvationer\|differentialekvation]] är stabil eller inte. Det finns tre fall:
## Homogen [[Differentialekvationer\|differentialekvation]]
1. $\sigma(A)<0$, dvs alla [[Egenvärden\|egenvärden]] är negativa $\Rightarrow$ **stabil**
2. $\sigma(A)=0$, dvs alla [[Egenvärden\|egenvärden]] är negativa eller noll $\Rightarrow$ **[[Neutralt Stabil\|neutralt stabil]]** eller **instabil**
3. $\sigma(A)>0$, dvs alla [[Egenvärden\|egenvärden]] är positiva $\Rightarrow$ **instabil**

## Homogen [[Differentialekvationer\|differentialekvation]] med [[Diagonalisering\|diagonaliserbar]] [[Matris\|matris]] A
1. $\sigma(A)<0$, dvs alla [[Egenvärden\|egenvärden]] är negativa $\Rightarrow$ **stabil**
2. $\sigma(A)=0$, dvs alla [[Egenvärden\|egenvärden]] är negativa eller noll $\Rightarrow$ **[[Neutralt Stabil\|neutralt stabil]]** 
3. $\sigma(A)>0$, dvs alla [[Egenvärden\|egenvärden]] är positiva $\Rightarrow$ **instabil**

## [[Inhomogena Differentialekvationer\|Inhomogen Differentialekvation]]
tolkas som ett [[System (matematisk definition)\|System (matematisk definition)]] där insignalen är $\vec{f(t)}$ och utsignalen är $\vec{x}'$.
1. $\sigma(A)<0$, dvs alla [[Egenvärden\|egenvärden]] är negativa $\Rightarrow$ **[[Insignal Stabil\|insignal stabil]]**
2. $\sigma(A)=0$, dvs alla [[Egenvärden\|egenvärden]] är negativa eller noll $\Rightarrow$ **icke [[Insignal Stabil\|insignal stabil]]** 
3. $\sigma(A)>0$, dvs alla [[Egenvärden\|egenvärden]] är positiva $\Rightarrow$ **icke [[Insignal Stabil\|insignal stabil]]**

# Stabil
alla lösningar $\vec{x(t)}\rightarrow \vec{0}$

# Instabil
det finns någon lösning som är obegränsad! 

[[Neutralt Stabil\|Neutralt Stabil]]
[[Insignal Stabil\|Insignal Stabil]]
[[Insignal-utsignalstabilt\|Insignal-utsignalstabilt]]
