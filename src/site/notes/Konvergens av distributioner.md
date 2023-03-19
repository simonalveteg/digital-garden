---
{"dg-publish":true,"permalink":"/konvergens-av-distributioner/","tags":["systemochtransformer"]}
---


En distributionsföljd [[Konvergens\|konvergerar]] 

$\mathcal{U_{n}}\rightarrow \mathcal{U} \text{ då } n \rightarrow \infty$ om för varje testfunktion $\varphi \in \mathcal{D}$ gäller 
$$<\mathcal{U_{n}},\varphi> \rightarrow<\mathcal{U},\mathcal{\varphi}> \text{ då } n \rightarrow \infty$$
avbildningen [[Konvergens\|konvergerar]] punktvis för varje testfunktion. Man kan definiera en distributionsserie
$$\sum\limits_{k=1}^{\infty}\mathcal{U}_k=\lim_{n \rightarrow \infty}\sum\limits_{k=1}^{n}\mathcal{U_{k}}$$

Om distributionsserien $\sum\limits_{k=1}^{\infty}\mathcal{U_{k}}$ är [[Konvergens\|konvergent]], dvs att gränsvärdet existerar, då gäller 
$$\left(\sum\limits_{k=1}^{\infty}\mathcal{U_{k}}\right)'=\sum\limits_{k=1}^{\infty}(\mathcal{U_{k}}')$$
detta gäller oavsett vilken sorts [[Konvergens\|konvergens]] det är?


[[Faltning\|Faltningen]] mellan $\varphi\in \mathcal{D}$ och en [[Distributioner\|distribution]] $\mathcal{U}$ defineras av $$(\varphi*\mathcal{U})(t)=\int_{-\infty}^{\infty}\varphi(t-\tau)\mathcal{U(\tau)d \tau}$$man kan visa att $\varphi*\mathcal{U}$ är en funktion i $C^{\infty}(\mathbb{R})$ (dvs oändligt deriverbar)

> En [[Distributioner\|distribution]] får allmänt inte multipliceras eller [[Faltning\|faltas]] med en annan [[Distributioner\|distribution]]!

**om** [[Faltning\|faltningen]] är definierad gäller nedanstående
$$\large\begin{cases} \mathcal{U}*\mathcal{V} = \mathcal{V}*\mathcal{U} \\ (\mathcal{U}+\mathcal{V})*\mathcal{W}=\mathcal{U}*\mathcal{W}+\mathcal{V}*\mathcal{W} \\
\mathcal{U}*\delta=\mathcal{U} \\
(\mathcal{U}*\mathcal{V})'=\mathcal{U'}*\mathcal{V}=\mathcal{U}*\mathcal{V'} \\
f(t)*\delta(t)=f(t) \text{ för alla kontinuerliga funktioner} \\
f(t)*\delta'(t)=f'(t) \\
f(t)*\delta''(t)=f''(t)
\end{cases}$$