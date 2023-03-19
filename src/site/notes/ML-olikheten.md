---
{"dg-publish":true,"permalink":"/ml-olikheten/","tags":["funktionsteori"]}
---


Ett fundamentalt verktyg för att uppskatta storleken av en [[Komplexa Kurvintegraler\|komplex kurvintegral]]

Om $\gamma$ är en (styckvis) [[Slät Kurva\|slät kurva]] och $f$ en kontinuerlig funktion på $\gamma$ som uppfyller att $|f(z)|\leq M$ för alla $z\in\gamma$ så gäller
$$ 
\left|\int_{\gamma}f(z)dz\right| \leq Ml(\gamma)
$$
där $l(\gamma)$ är längden av $\gamma$ (ex: längden av en cirkel är dess omkrets). M begränsar absolutbeloppet av funktionen.

> ML-olikheten är en övre begränsning av [[Komplexa Kurvintegraler\|kurvintegralen]] som kurvans längd L gånger en övre begränsing M av beloppet $|f(z)|$ 

tänk dig att längden $l$ gånger höjden $M$ bildar en rektangel. Enda fallet då arean blir lika med integralen är när funktionen är en rät linje. I alla andra fall (givet att $M$ är funktionens högsta värde) blir integralen mindre än $Ml(\gamma)$.

[[Komplexa Kurvintegraler\|Kurvintegralen]] bestäms helt av [[Singularitet\|singulariteterna]] som omsluts av kurvan. Ibland är det jobbigt att använda [[Residykalkyl\|residykalkyl]] för att beräkna integralen. Då kan det vara lättare att använda ML-olikheten för att skriva upp ett uttryck som beror på radien $R$, och visa att uttrycket går mot noll när $R$ går mot oändligheten. Då integralen bestäms av [[Singularitet\|singulariteterna]] har man alltså visat att integralen blir noll. Använd $M=4/R^{n-m}$ där m är graden av täljaren och n är graden av nämnaren, och $l=2\pi R$ (om området är en cirkel). Om alla [[Singularitet\|singulariteter]] är utanför området kan man använda [[Cauchys Integralsats\|Cauchys integralsats]] istället.