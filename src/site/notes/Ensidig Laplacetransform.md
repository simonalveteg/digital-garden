---
{"dg-publish":true,"permalink":"/ensidig-laplacetransform/","tags":["systemochtransformer"]}
---

Hittils när vi pratat om laplacetransformer har vi implicerat tvåsidiga laplacetransformer $L_{II}$. För ensidiga laplacetransformer tillkommer det en term som beror på begynnelsevärdet? 

För
$$y''+y'+y=\theta(t)$$
fungerar [[Laplacetransformationer\|laplacetransformen]] väldigt bra ( $\mathcal{L}(y')=s\mathcal{L}(y)$ ). Men om man dessutom har begynnelsevillkor fungerar det inte lika bra. Då kan man använda ensidiga laplacetransformer! ($\mathcal{L}_{I}$)

Den ensidiga [[Laplacetransformationer\|laplacetransformen]] definieras
$$\mathcal{L}_I(f(t))(s)\stackrel{def}{=}\int_{0}^{\infty}e^{-st}f(t)dt.$$
För [[Kausala Funktioner\|kausala funktioner]] finns det ingen skillnad mellan ensidig och tvåsidig, då man ändå bara integrerar över positiva $t$. Kan skrivas som integralen från $-\infty$ till $\infty$ gånger $\theta(t)$.

Om man vill utföra ensidig [[Laplacetransformationer\|laplacetransform]] på ett [[System (matematisk definition)\|System (matematisk definition)]] med begynnelsevillkor kan man använda formeln nedan
$$\mathcal{L}_{I}(f'(t))(s)=s \mathcal{L}_{I}(f(t))(s)-f(0)$$



[[Lösa exponentialmatris med ensidig laplacetransform\|Lösa exponentialmatris med ensidig laplacetransform]]