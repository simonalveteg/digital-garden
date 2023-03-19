---
{"dg-publish":true,"permalink":"/laplacetransformationer/","tags":["systemochtransformer"]}
---



[[Fouriertransformationer\|Fouriertransformen]] avbildas från reella axeln till reella axeln? #question 
$f(t)\xrightarrow{\mathcal{F}}F(w)$, där $F(w)=\int_{-\infty}^{\infty}e^{iwt}f(t)dt$

Laplacetransformen av $f(t)$ i $\mathbb{R}$ är
$$\mathcal{L}(f(t))(s)=\mathcal{L}_{II}=\int_{-\infty}^{\infty}e^{-st}f(t)dt$$
för alla [[Komplexa Tal\|komplexa tal]] $s$ sådana att integralen exister (är [[Konvergens\|konvergent]]). $\mathcal{L}_{II}$ står för tvåsidig Laplacetransform. 

[[Definitionsmängd\|Definitionsmängden]] av $\mathcal{L}(f(t))(s)$ är en vertikal strimla där realdelen ligger mellan två tal ($a<Re(s)<b$) i komplexa planet, där $a,b$ kan vara $\pm\infty$.

[[Överföringsfunktion\|Överföringsfunktionen]] $H(s)=\mathcal{L}(h(t))(s)$ då $S$ är ett [[Linjära och Tidsinvarianta System\|LTI-system]].

$\mathcal{L}(\theta(t))(s)=\int_{-\infty}^{\infty}e^{-st}\theta(t)dt=\int_{0}^{\infty}e^{-st}dt=\left[\frac{e^{-st}}{-s}\right]_{t=0}^{\infty}=\begin{cases} \frac{1}{s},Re(s)>0 \\ \text{divergent , }Re(s)<0 \end{cases}= \frac{1}{s}\text{ där } Re(s)>0$

Om $f(t)\xrightarrow{\mathcal{L}}F(s)$ och $g(t)\xrightarrow{\mathcal{L}}G(s)$ så finns det massa fina formler från formelsamlingen:
![laplaceformelsamling.png](/img/user/images/laplaceformelsamling.png)

$$\mathcal{L}(e^{at}\theta(t))(s)=\mathcal{L}(\theta(t))(s-a)=\frac{1}{s-a} \text{ då } Re(s-a)>0$$
[[Laplacetransformation av tempererade funktioner\|Laplacetransformation av tempererade funktioner]]
[[Inversionsformeln\|Inversionsformeln]]
[[Ensidig Laplacetransform\|Ensidig Laplacetransform]]
