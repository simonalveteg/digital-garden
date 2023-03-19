---
{"dg-publish":true,"permalink":"/exponentialmatriser/","tags":["systemochtransformer"]}
---


För en [[Kvadratisk Matris\|kvadratisk matris]] $A$ definerar vi
$$e^{A}=I+A+ \frac{A^{2}}{2!}+ \frac{A^{3}}{3!}+...+ \frac{A^{k}}{k!}+.. $$
(det är en [[Maclaurinutveckling\|maclaurinutveckling]] av exponentialfunktionen, med en [[Matris\|matris]] istället för en variabel). Det är mycket lättare att räkna ut [[Matris\|matriser]] upphöjt med en exponent för [[Diagonalmatris\|diagonalmatriser]].

$$e^{\begin{pmatrix}a & 0 \\ 0 & b\end{pmatrix}}=I+\begin{pmatrix}a & 0 \\ 0 & b\end{pmatrix}+ \frac{\begin{pmatrix}a & 0 \\ 0 & b\end{pmatrix}^{2}}{2!}+...=\begin{pmatrix}e^{a} & 0 \\ 0 & e^{b}\end{pmatrix}$$

$e^{\begin{pmatrix}\lambda_{1} & 0 \\ 0 & \lambda_{2}\end{pmatrix}}=\begin{pmatrix}e^{\lambda_{1}} & 0 \\ 0 & e^{\lambda_{2}}\end{pmatrix}$ 
$e^{SAS^{-1}}=Se^AS^{-1}$ för alla [[Kvadratisk Matris\|kvadratiska matriser]] $A$.

om A är [[Diagonalisering\|diagonaliserbar]] så är $e^{A}=e^{SDS^{-1}}=Se^{D}S^{-1}$

1. $e^{\vec{0}}=I_{nxn}$ - analogt med $e^{0}=1$ 
2. $AB=BA \Rightarrow e^{A}e^{B}=e^{B}e^{A}=e^{A+B}$ 
3. $e^{(t_{1}+t_{2})A}=e^{t_{1}A}e^{t_{2}A}=e^{t_{2}A}e^{t_{1}A}$ 
4. $e^{tA}$ är [[Invers Matris\|inverterbar]] för alla $t$, med inversen $(e^{tA})^{-1}=e^{-tA}$ — precis som för tal! $e^{tA}e^{-tA}=e^{\vec{0}}=I$ 
5. $\frac{d}{dt}(e^{tA})=e^{tA}A=Ae^{tA}$ - precis som för tal igen (kan bevisas mha [[Maclaurinutveckling\|maclaurinutveckling]]).  


Den [[Homogena Differentialekvationer\|homogena differentialekvationen]]
$$\begin{cases}\vec{x'}=A \vec{x}, t\geq0\\\\ \vec{x(0)}=\begin{pmatrix}a \\ b\end{pmatrix} \end{cases}$$
har entydig lösning $\vec{x(t)}=e^{tA}\begin{pmatrix}a \\ b\end{pmatrix}$  #todo flytta till hom. diffekv?

Sats som dyker upp många gånger i extentor!!!
> Om $A_{nxn}$ är [[Diagonalisering\|diagonaliserbar]] har $e^{tA_{nxn}}$ bara element av typ $b_{1}e^{\lambda_{1}t}+b_{2}e^{\lambda_{2}t}+...+b_{n}e^{\lambda_{n}t}$, där b är tal. Om de inte gör det kan man direkt dra slutsatsen att $A$ inte är [[Diagonalisering\|diagonaliserbar]]!


>  Om $e^{tA_{nxn}}$ bara har element som är summan av $p(t)e^{\lambda_{i}t}$ där $p(t)$ är ett [[Polynom\|polynom]] av grad < [[Multiplicitet\|multiplicitet]] av [[Egenvärden\|egenvärdet]] $\lambda_{i}$


# Lösningsmetoder
två huvudsakliga metoder
1. Använd definitionen med [[Maclaurinutveckling\|maclaurinutveckling]]
2. Om A är en [[Diagonalisering\|diagonaliserbar matris]] kan man använda sambandet $e^{A}=e^{SDS^{-1}}=Se^{D}S^{-1}$

kan också lösas med [[Lösa exponentialmatris med ensidig laplacetransform\|Lösa exponentialmatris med ensidig laplacetransform]]

