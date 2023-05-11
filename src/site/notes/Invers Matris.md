---
{"dg-publish":true,"permalink":"/invers-matris/","tags":["systemochtransformer, linjäralgebra"]}
---

För den [[Kvadratisk Matris\|kvadratiska matrisen]] A är den inversa [[Matris\|matrisen]] $A^{-1}$ den [[Matris\|matris]] som, när multiplicerad med A via [[Matrismultiplikation\|Matrismultiplikation]] bildar [[Enhetsmatris\|Enhetsmatrisen]]

$$
AA^{-1}= A^{-1}A=I
$$
det vill säga, $A^{-1}$ är den linjära avbildning som gör motsatsen till $A$. Om man utför $A$ följt av $A^{-1}$ kommer man tillbaka till sin startpunkt.

Om man har en matrisekvation, ex $Ax=V$, kan man lösa ut sin [[Vektorer\|vektor]] $x$ genom att multiplicera båda sidor med inversen på vänster sida: $A^{-1}Ax=A^{-1}V \Leftrightarrow x=A^{-1}V$. 

Om [[Determinant\|determinanten]] är 0 kan man inte hitta en invers [[Matris\|matris]]. I planet innebär en [[Linjär Avbildning\|linjär avbildning]] med [[Determinant\|determinanten]] 0 att alla [[Vektorer\|vektorer]] avbildas på en linje. Det finns därmed inte endast en entydigt bestämd [[Matris\|matris]] som blir inversen.

$$M^{-1}=\frac{adj(M)}{det(M)}$$


## 2x2 Matriser
För 2x2-[[Matris\|matriser]] finns det en lätt formel som använder [[Adjunkt Matris\|Adjunkt Matris]]
$$
\begin{pmatrix}a & b \\ c & d\end{pmatrix}^{-1}=\frac{1}{det(A)}\begin{pmatrix}d & -b  \\ -c & a\end{pmatrix}
$$


För [[Matris\|matriser]] som inte är [[Kvadratisk Matris\|kvadratiska]] finns det inte en invers som funkar på både vänster och höger sida. 

## Högerinvers

$$AA^{-1}=I$$

## Vänsterinvers

$$A^{-1}A=I$$

