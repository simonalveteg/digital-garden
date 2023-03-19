---
{"dg-publish":true,"permalink":"/likformig-konvergens/","tags":["funktionsteori"]}
---

Ett “starkare” konvergensbegrepp än [[Punktvis konvergens\|Punktvis konvergens]].

Enklaste sättet att definiera likformig konvergens är att först införa ett sätt att mäta “storleken av en funktion” - [[Supremumnormen\|Supremumnormen]]

En [[Funktionsföljder\|funktionsföljd]] kallas likformigt konvergent mot någon funktion $f$ (på $D$) om [[Supremumnormen\|supremumnormen]] går mot noll när k går mot oändligheten.
$$
\lim_{k\rightarrow\infty}||f_{k}-f||_{D}=0
$$
obs: om $f_k$ konvergerar likformigt mot $f$, så måste $f_{k}$ [[Punktvis konvergens\|konvergera punktvis]] mot f

> Det är oftast enklast att först visa att [[Funktionsföljder\|funktionsföljden]] [[Punktvis konvergens\|konvergerar punktvis]]

För att visa att en [[Funktionsserier\|funktionsserie]] är likformigt konvergent, försök hitta en [[Gränsfunktion\|gränsfunktion]] genom att resonera kring funktionens utseende (vad händer för olika värden på x). Sätt in [[Gränsfunktion\|gränsfunktionen]] i definitionen ovan och se om gränsvärdet blir 0 .


Det finns många bra satser om likformig konvergens:
___
Om $f_{k}$ är en följd av kontinuerliga funktioner som konvergerar likformigt mot $f$ (på någon [[Definitionsmängd\|definitionsmängd]] $D$), så är $f$ också kontinuerlig på $D$.

Från detta följer att om $f_k$ är en följd av kontinuerliga funktioner som [[Punktvis konvergens\|konvergerar punktvis]] mot en diskontinuerlig funktion, så kan konvergensen omöjligt vara likformig
___
Låt $I=[a,b]$ vara ett begränsat intervall och $f_k\rightarrow f$ likformigt på $I$. Då gäller 
$$
\lim_{k\rightarrow\infty}\int_{a}^{b}f_{k}(x)dx=\int_{a}^{b}\left(\lim_{k\rightarrow\infty}f_k(x)dx\right)=\int_{a}^{b}f(x)dx
$$
___
Låt $D\subset C$  vara ett område och anta att $f_{n} : D \rightarrow C$ är en följd av kontinuerliga funktioner som konvergerar likformigt mot $f$. Om $\gamma$ är en kurva av ändlig längd i $D$, så gäller att
$$
\lim_{n\rightarrow\infty}\int_{\gamma}f_{n}(z)dz=\int_{\gamma}f(z)dz
$$
___
Om $D\subset C$ är ett område och $f_{k}$ är en följd av [[Holomorf\|holomorfa]] funktioner som konvergerar likformigt mot $f$ på $D$. Då gäller
1. $f$ är [[Holomorf\|holomorf]]
2. $f'_{k} \rightarrow f'$ [[Lokalt likformig\|lokalt likformigt]] på $D$
___
Anta att $I$ är ett intervall på $\mathbb{R}$ och att $f_k$ är en följd av $\mathbb{C}^{1}$ (dvs kontinuerlig, deriverbar och kontinuerlig derivata) som [[Punktvis konvergens\|konvergerar punktvis]] mot $f$ *och* anta dessutom att $f'_{k}$ konvergerar likformigt mot någon funktion $g$. 