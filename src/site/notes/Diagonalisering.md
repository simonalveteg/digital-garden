---
{"dg-publish":true,"permalink":"/diagonalisering/","tags":["linjäralgebra","systemochtransformer"]}
---

En [[Matris\|matris]] är diagonaliserbar om alla dess rader eller kolonner är [[Linjärt Oberoende\|linjärt oberoende]] [[Egenvektorer\|egenvektorer]]?? #todo

A är diagonalliserbar om A har 2 stycken [[Linjärt Oberoende\|linjärt oberoende]] [[Egenvektorer\|egenvektorer]], $s_{1}$ och $s_{2}$ med [[Egenvärden\|egenvärden]] $\lambda_{1}$ och $\lambda_{2}$. Skriv $S=(s_{1}, s_{2})$ då ges den diagonaliserade A av $S^{-1}AS=\begin{pmatrix}\lambda_{1} & 0 \\ 0 & \lambda_{2} \end{pmatrix}$. dvs $A=S\begin{pmatrix}\lambda_{1} &  0\\0  & \lambda_2 \end{pmatrix}S^{-1}$. $S$ diagonaliserar [[Matris\|matrisen]]! $A=SDS^{-1}$ där $D$ är [[Diagonalmatris\|diagonalmatrisen]]

> Diagonalisering innebär att man gör ett basbyte så att alla [[Basvektor\|basvektorer]] blir [[Egenvektorer\|egenvektorer]]!


## Egenskaper av diagonaliserbara [[Matris\|matriser]] $A=A_{nxn}$ 
1. En [[Matris\|matris]] är [[Invers Matris\|inverterbar]] om och endast om den har $n$ stycken [[Linjärt Oberoende\|linjärt oberoende]] [[Egenvektorer\|egenvektorer]]. Då är $S^{-1}AS=D \Leftrightarrow A=SDS^{-1}$.
2. $A_{nxn}$ har $n$ stycken **olika** [[Egenvärden\|egenvärden]]  $\Rightarrow A_{nxn}$ är diagonaliserbar
3. Om $A_{nxn}$ är reell och [[Symmetrisk Matris\|symmetrisk]] är den också diagonaliserbar
4. $\lambda_{1}...\lambda_{n}=det(A_{nxn})$, dvs produkten av alla [[Egenvärden\|egenvärden]] är lika med [[Determinant\|determinanten]]
	1. $det(A)=det(SDS^{-1})=det(S)det(D)det(S^-1)=det(SS^{-1})det(D)=det(D)$.
5. $\lambda_{1}+\lambda_{2}+...+\lambda_{n}=tr(A_{nxn})=$ summan av alla element i diagonalen i $A_{nxn}$. dvs: om du vill dubbelkolla att du har fått rätt [[Egenvärden\|egenvärden]] kan du räkna ut [[Spår\|spåret]], som ska vara lika med summan av alla [[Egenvärden\|egenvärden]].