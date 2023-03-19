---
{"dg-publish":true,"permalink":"/homogena-differentialekvationer/","tags":["systemochtransformer"]}
---


[[System (matematisk definition)\|Systemet]]
$$\begin{pmatrix}x_{1}(t) \\ x_{2}(t)\end{pmatrix}'= \begin{pmatrix}a_{1} & a_{2} \\ a_{3} & a_{4}\end{pmatrix} \begin{pmatrix}x_{1}(t) \\ x_2(t)\end{pmatrix}+\begin{pmatrix}f_{1}(t) \\ f_{2}(t)\end{pmatrix}
$$
dvs
$$
\vec{x(t)'}=A \vec{x(t)}+\vec{f(t)}
$$
sägs vara homogen om $\vec{f(t)}$ är nollvektorn. 

För en homogen ekvation där A är [[Diagonalisering\|diagonaliserbar]] är det väldigt lätt att lösa. Skriv upp ekvationen med [[Diagonalmatris\|diagonalmatrisen]] istället för A, vilket ger ett [[Ekvationssystem\|ekvationssystem]] där varje ekvation endast har en sorts x. [[Integrerande Faktor\|Integrerande faktor]] => svar.

>$\vec{x'}=A \vec{x}$ har en allmän lösning $\vec{x(t)}=c_{1}e^{\lambda_{1}t}\vec{s_{1}}+c_{2}e^{\lambda_{2}t}\vec{s_{2}}$.

där c är konstanter, lambda är [[Egenvärden\|egenvärden]] och s är [[Egenvektorer\|egenvektorer]] till A. 

```ad-Bevis
collapse: closed




$$\vec{x'}=S\begin{pmatrix}\lambda_{1} & 0 \\ 0 & \lambda_2\end{pmatrix}S^{-1}\vec{x}$$
om man multiplicerar med S-invers till vänster på båda sidor får man
$$(S^{-1}\vec{x})'=\begin{pmatrix}\lambda_{1} & 0 \\ 0 & \lambda_2\end{pmatrix}(S^{-1}\vec{x})$$
där man kan införa en ny [[Vektorer|vektor]] $\hat{x}(t)=S^{-1}\vec{x}(t)$  vilket ger
$$(\hat{x})'=\begin{pmatrix}\lambda_{1} & 0 \\ 0 & \lambda_2\end{pmatrix}\hat{x}$$
som ger (med [[integrerande faktor]])
$$\hat{x}(t)=\begin{pmatrix}c_{1}e^{\lambda_{1}t} \\ c_{2}e^{\lambda_{2}t}\end{pmatrix}$$
vilket man kan sätta in i hur vi definierade xhat


```

Man kan ocksåo använda $e^{tA}$ metoden:

[[System (matematisk definition)\|Systemet]]
$$\begin{cases} \vec{x}'=A \vec{x} \\ \vec{x}(0)=\begin{pmatrix}a \\ b\end{pmatrix}\end{cases}$$
har entydig lösning 
$$\vec{x}(t)=e^{tA}\begin{pmatrix}a \\ b\end{pmatrix}$$