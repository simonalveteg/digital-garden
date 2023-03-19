---
{"dg-publish":true,"permalink":"/system-och-transformer-f16/","tags":["föreläsning","systemochtransformer"]}
---


[[Ensidig Laplacetransform\|Ensidig Laplacetransform]]

# Kvadratisk form
$$f(x_{1},x_{2},x_{3})=3x_{1}^{2}+2x_{1}x_{2}+x_{2}x_{3}-x_{3}^{2}=(x_{1},x_{2},x_{3})\begin{pmatrix}k_{11} & k_{12} & k_{13} \\ k_{21} & k_{22} & k_{23} \\ k_{31} & k_{32} & k_{33} \end{pmatrix}\begin{pmatrix}x_{1} \\ x_{2} \\ x_{3}\end{pmatrix}$$
där k… kallas k-matrisen.

Inte så viktigt. “om ni inte hinner, hoppa över”.


# Ex 16.1
Beräkna $e^{tA}$ för $A=\begin{pmatrix}0 & -1 \\ 1 & 0\end{pmatrix}$.
### lösning
börja med [[Resolventmatris\|resolvent matris]] $(sI-A)^{-1}=\begin{pmatrix}s & 1 \\ -1 & s\end{pmatrix}^{-1}=\frac{1}{s^{2}+1}\begin{pmatrix}s & -1  \\ 1 & s\end{pmatrix}$ 
leder till att $$e^{tA}\theta(t)=\mathcal{L}^{-1}_\text{kausal}\left((sI-A)^{-1}\right)=\mathcal{L}^{-1}_\text{kausal}\left(\begin{pmatrix} \frac{s}{s^{2}+1} & \frac{-1}{s^{2}+1} \\ \frac{1}{s^{2}+1} & \frac{s}{s^{2}+1}\end{pmatrix}\right)=\begin{pmatrix}cost \theta(t)  & -sint \theta(t) \\ sint \theta(t) & cist \theta(t)\end{pmatrix}$$ där sista steget står i formelbladet? $\theta(t)$ kan flyttas ut ur [[Matris\|matrisen]]. Gäller för alla $t\neq0$ (för $\theta$ är inte definerad i noll). 

Nu delar vi upp i de två fallen 
för $t>0$ gäller 
$$e^{tA}=\begin{pmatrix}cost & -sint \\ sint & cost\end{pmatrix}$$
Om två [[Holomorfa Funktioner\|holomorfa funktioner]] sammanfaller någonstans så sammanfaller de överallt (antar att han menar att om derivatorna är lika också i en punkt typ?) #question

 $e^{zA}$ och $\begin{pmatrix}cost & -sint \\ sint & cost\end{pmatrix}$ är [[Holomorf\|holomorfa]] i hela komplexa planet $z\in\mathbb{C}$ 
 altså gäller det även för alla $t\leq0$! 


# Ex 16.2
Lös $\begin{cases}y''+3y'+2y=1, t>0 \\ y(0)=1 \\ y'(0)=-3 \end{cases}$

det går att lösas mha standardmetoden från endim med partikulär och homogen lösning. Om vi vill lösa med laplace kan vi inte använda tvåsidig, då det finns begynnelsev
illkor. Även med [[Ensidig Laplacetransform\|ensidig laplacetransform]] är det inte säkert att det funkar, man måste dubbelkolla så att ens lösning klarar villkoren.
### lösning
$$\mathcal{L}_{I}(y''+3y'+2y)(s)=\mathcal{L}_{I}(1)(s)=\mathcal{L}(1\cdot\theta(t))(s)=\frac{1}{s}$$
$$s^{2}\mathcal{L}_{I}(y(t))(s)-sy(0)-y'(0)+3(s \mathcal{L}_{I}(y(t))(s)-y(0))+2\mathcal{L}_{I}(y(t))(s)=\frac{1}{s}$$
sen kan man bryta ut $\mathcal{L}_{I}$
$$(s^{2}+3s+2)\mathcal{L}_{I}(y)(s)=s+\frac{1}{s}$$
$$\mathcal{L}_{I}(y)(s)=\frac{s+\frac{1}{s}}{s^{2}+3s+2}=\frac{s^{2}+1}{s(s^{2}+3s+2)}$$
nu kan den [[Ensidig Laplacetransform\|ensidiga laplacetransformen]] bytas mot en tvåsidig genom att lägga till en faktor $\theta(t)$, och då kan vi använda våra tidigare kunskaper. 
$$y(t)\theta(t)=\mathcal{L}^{-1}_\text{kausal}\left(\frac{s^{2}+1}{s(s+1)(s+2)}\right)(t)$$
sen använder vi [[Residy\|residy]] på de tre [[Poler\|polerna]], och vi väljer den [[Kausal\|kausala]] strimlan.

$$Res\left(\frac{e^{st}(s^{2}+1)}{s(s+1)(s+2)}\right)=\left.\frac{e^{st}(s^{2}+1)}{s(s+1)(s+2)}\right|_{\text{för varje pol}}$$
och svaret blir då

$$y(t)\theta(t)=\theta(t)\left(Res_{0}+Res_{-1}+Res_{-2}\right)$$
för $t>0$ kan vi ta bort [[Stegfunktion\|stegfunktionen]].

Glöm inte verifiera att begynnelsevillkoren stämmer!!



# Subject
[[System och Transformer\|System och Transformer]]
