---
{"dg-publish":true,"permalink":"/inhomogena-differentialekvationer/","tags":["systemochtransformer"]}
---


För specialfallet $\vec{x'}=A \vec{x}+e^{st}\begin{pmatrix}f_{1} \\ f_{2}\end{pmatrix}$ (tänk på att s kan vara noll och då blir $e^{st}=1$)
1. Om $s=bi$ kallas $\vec{x_{p}(t)}=(sI-A)^{-1}e^{st}\begin{pmatrix}f_{1} \\ f_{2}\end{pmatrix}$ för en **stationär lösning** till ekvationen.
2. Om $s=a+bi$ kallas det istället för en **generaliserad stationär lösning**.
3. $\vec{x_{h}(t)}=c_{1}e^{\lambda_{1}t}\vec{s_{1}}+c_{2}e^{\lambda_{2}t}\vec{s_{2}}$ kallas den **transienta lösningen** till det [[Stabila och Instabila System\|stabila systemet]]


> Tolkas som ett [[System (matematisk definition)\|System (matematisk definition)]] där insignalen är $\vec{f(t)}$ och utsignalen är $\vec{x}'$.


Lös matrisekvationen 
$$\begin{pmatrix}x_{1}'(t) \\ x_{2}'(t)\end{pmatrix}=\begin{pmatrix}a_{1} & a_{2} \\ a_{3} & a_{4}\end{pmatrix}\begin{pmatrix}x_{1}(t) \\ x_{2}(t)\end{pmatrix}+\begin{pmatrix}f_{1}(t)  \\ f_{2}(t)\end{pmatrix}$$
där $A=\begin{pmatrix}a_{1} & a_{2} \\ a_{3} & a_{4}\end{pmatrix}$ är [[Diagonalisering\|diagonaliserbar]].

Problemet kan lösas med flera olika metoder. Om man kan bryta ut en faktor $e^{st}$ ur insignalen $f(t)$ – använd metod 1!!! Annars metod 2. 

## metod 1
Ekvationen har en allmän lösning (tack vare att det är en linjär matrisekvation)
$$\vec{x(t)}=\vec{x_{h}(t)}+\vec{x_{p}(t)}$$
där $\vec{x_{h}(t)}=c_{1}e^{\lambda_{1}t}\vec{s_{1}}+c_{2}e^{\lambda_{2}t}\vec{s_{2}}$, tack vare att A är [[Diagonalisering\|diagonaliserbar]].
och $\vec{x_{p}(t)}$ är en partikulärlösning (vilken som helst). Vi kan inte bestämma $\vec{x_{p}(t)}$ för alla $\vec{F(t)}$, endast för specalfall.

I fallet då $\vec{F(t)}=e^{st}\begin{pmatrix}f_{1} \\ f_{2}\end{pmatrix}$, där $s$,$f_{1}$ och $f_{2}$ är givna tal, har vi partikulärlösningen
$$\vec{x_{p}(t)}=(sI-A)^{-1}e^{st}\begin{pmatrix}f_{1} \\ f_{2}\end{pmatrix}$$
där $(sI-A)^{-1}$ kallas **[[Resolventmatris\|resolventmatrisen]]**. Funkar endast om inversen till [[Resolventmatris\|resolventmatrisen]] existerar, dvs om $det(sI-A)\neq0$, vilket är uppfyllt då $s$ inte är ett [[Egenvärden\|egenvärde]] till den. *varför?*


## metod 2
A är [[Diagonalisering\|diagonaliserbar]], alltså kan man skriva 
$$S^{-1}AS=\begin{pmatrix}\lambda_{1} & 0 \\ 0 & \lambda_{2}\end{pmatrix}=D \Leftrightarrow A=SDS^{-1}$$
$$\vec{x}=A \vec{x} +\vec{F(t)}=SDS^{-1}\vec{x}+\vec{F(t)}$$
multiplicera båda led med $S^{-1}$ från vänster
$$\Rightarrow (S^{-1}\vec{x})'=D(S^{-1}\vec{x})+S^{-1}\vec{F(t)}$$
gör variabelbyte genom att sätta $S^{-1}\vec{x(t)}=\hat{x(t)}$ dvs $\vec{x(t)}=S\hat{x(t)}$. Då är 
$$\hat{x}'=D\hat{x}+S^{-1}\vec{F(t)}$$
eftersom att [[Matris\|matrisen]] D är en [[Diagonalmatris\|diagonalmatris]] kan man enkelt lösa ekvationen ovan:
$$\begin{cases} \hat{x_{1}}'=\lambda_{1}\hat{x_{1}}+ F_{1}(t)\\ \hat{x_{2}}'=\lambda_{2}\hat{x_{2}}+F_{2}(t) \end{cases}$$

där man antar att $S^{-1}\vec{F(t)}=\begin{pmatrix}F_{1}(t) \\ F_{2}(t)\end{pmatrix}$

$$\Rightarrow \begin{cases}\hat{x_{1}}=e^{\lambda_{1}t}\int e^{-\lambda_{1}t}F_{1}(t)\\ \hat{x_{2}}=e^{\lambda_{2}t}\int e^{-\lambda_{2}t}F_{2}(t) \end{cases}$$
genom att använda $\vec{x}=S\begin{pmatrix}\hat{x_{1}} \\ \hat{x_{2}}\end{pmatrix}$ kan vi gå tillbaka till $\vec{x}$.

