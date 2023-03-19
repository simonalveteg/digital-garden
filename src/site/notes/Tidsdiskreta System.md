---
{"dg-publish":true,"permalink":"/tidsdiskreta-system/","tags":["systemochtransformer"]}
---


Tidsdiskreta [[System (matematisk definition)\|System (matematisk definition)]] är samma sak som rekursionsformler? [[System (matematisk definition)\|System (matematisk definition)]] som inte har kontinuerlig tid ([[Tidskontinuerliga System\|Tidskontinuerliga System]])

Ett [[System (matematisk definition)\|System (matematisk definition)]] $S: \begin{pmatrix}x_{0}\\y_{0}\end{pmatrix}\rightarrow\begin{pmatrix}x_{k}\\y_{k}\end{pmatrix}$ för $k=0,1,2,3..$ ges av **rekursionsformeln**
$$
\begin{pmatrix}x_{k}\\y_{k}\end{pmatrix}=\begin{pmatrix}a\space b\\c\space d\end{pmatrix}\begin{pmatrix}x_{k-1}\\y_{k-1}\end{pmatrix}+\begin{pmatrix}c_{k}\\d_{k}\end{pmatrix}

$$
$$\vec{v_{k}}=A \vec{v_{k-1}}+\begin{pmatrix}c_{k}\\d_{k}\end{pmatrix}$$
där [[Matris\|matrisen]] abcd är [[Avbildningsmatris\|avbildningsmatrisen]] A, abcd är konstanter och $c_k$ och $d_{k}$ är konstanter för olika k. För varje diskret värde på k ges värdet på x och y av A multiplicerat med de föregående värdena. Det ser likadant ut för större [[System (matematisk definition)\|System (matematisk definition)]] (xk,yk,zk osv). [[System (matematisk definition)\|Systemet]] kallas **homogent** om $c_{k}$ och $d_{k}$ är noll. Annars är det inhomogent.
Rekursionsformlen kan lösas med en homogen lösning och en partikulärlösning. Precis som för [[Differentialekvationer\|Differentialekvationer]] och [[Rekursionsekvationer\|Rekursionsekvationer]].


## Homogen lösning
Om $A_{2x2}$ är [[Diagonalisering\|diagonaliserbar]] så har [[System (matematisk definition)\|systemet]] ovan en **homogen** (allmän) **lösning**

$$\vec{v_{k}^{h}}=\begin{pmatrix}x_{0}\\y_{0}\end{pmatrix}=c_{1}\lambda_{1}^{k}\vec{s_{1}}+c_{2}\lambda_{2}^{k}\vec{s_{2}}$$
för alla k=1,2,3.. där $S_{1}$ och $S_{2}$ är [[Egenvektorer\|egenvektorer]] till A. 

Om $max(|\lambda_{1}|, ... , |\lambda_{n}|<1$ är [[System (matematisk definition)\|systemet]] [[Stabila och Instabila System\|stabilt]] ($\lambda<1$ leder till att det går mot noll när $k \rightarrow\infty$)
Om $max(|\lambda_{1}|, ... , |\lambda_{n}|=1$ är [[System (matematisk definition)\|systemet]] [[Neutralt Stabil\|neutralt stabilt]]
Om $max(|\lambda_{1}|, ... , |\lambda_{n}|>1$ är [[System (matematisk definition)\|systemet]] [[Stabila och Instabila System\|instabilt]]



## Partikulär lösning
**Partikulärlösningen** blir
$$\vec{v_{k}^{p}}=(I-A)^{-1}\begin{pmatrix}c_{0}\\d_{0}\end{pmatrix}$$
om $\begin{pmatrix}c_{k}\\d_{k}\end{pmatrix}=\begin{pmatrix}c_{0}\\d_{0}\end{pmatrix}$, dvs om de alltid är samma oavsett k.

Om $\begin{pmatrix}x_{0}\\y_{0}\end{pmatrix}$ är en [[Egenvektorer\|egenvektor]] blir det mycket lättare att räkna ut $A^{k}\begin{pmatrix}x_{0}\\y_{0}\end{pmatrix}$, då $A^{k}$ blir lika med [[Egenvärden\|egenvärdet]]. Men om det inte är en [[Egenvektorer\|egenvektor]] måste man använda [[Diagonalisering\|diagonalisering]], dvs A *måste* vara [[Diagonalisering\|diagonaliserbar]]! Annars går det ej att lösa. 

förhållandet mellan $y_{k}$ och $x_{k}$ efter lång tid ges av $\lim_{k\rightarrow\infty} \frac{x_{k}}{y_{k}}$ 

# Tillvägagångssätt för lösning 
1. Ta fram [[Egenvärden\|egenvärden]]
2. Ta fram [[Egenvektorer\|egenvektorerna]]
3. Ta fram homogenlösning mha formeln för [[Diagonalisering\|diagonaliserbar]] [[Matris\|matris]]
4. Ta fram partikulärlösning mha formeln
5. $\vec{v_{k}}=\vec{v_{k}^{h}}+\vec{v_{k}^{p}}$, använd eventuella villkor för att bli av med konstanter från homogenlösning.

# Jobbig ekvation

Om man har en ekvation med en jobbig faktor framför sin konstantterm vill man utföra någon sorts variabelbyte för att få samma faktor framför övriga termer så att den kan förkortas bort.

ex: $\begin{pmatrix}x_{k}  \\ y_{k} \end{pmatrix}=2^{k}\vec{w_{k}}$, om $2^{k}$ är faktorn man vill bli av med. 