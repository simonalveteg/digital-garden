---
{"dg-publish":true,"permalink":"/egenvektorer/","tags":["systemochtransformer","linjäralgebra"]}
---

En [[Vektorer\|vektor]] är en egenvektor till en [[Avbildningsmatris\|Avbildningsmatris]] om den behåller samma [[Linjärt Spann\|spann]] efter avbildningen. I planet innebär det att [[Vektorer\|vektorn]] bara skalas upp eller ned med någon faktor. Den faktorn kallas för vektorns [[Egenvärden\|egenvärde]]. 

$$A\vec{v}=\lambda\vec{v}$$
där A är en [[Avbildningsmatris\|avbildningsmatris]] och lambda är en [[Skalär\|skalär]] ([[Egenvärden\|egenvärdet]]). Om man ska skriva [[Skalär\|skalären]] som en [[Matris\|matris]] (och se det som en [[Matrismultiplikation\|matrismultiplikation]] istället) blir det en [[Enhetsmatris\|enhetsmatris]] med $\lambda$ istället för ettor. dvs

$$A \vec{v}=(\lambda I)\vec{v} \Rightarrow (A-\lambda I)\vec{v}=\vec{0}$$
enda sättet för avbildningen $(A-\lambda I)$ att bli noll är om [[Determinant\|determinanten]] är noll.


Istället för att fokusera på hur en [[Linjär Avbildning\|Linjär Avbildning]] flyttar [[Basvektor\|basvektorerna]], ger egenvektorerna en annan bild. Om man har en avbildning som motsvarar en rotation i rummet, så ligger egenvektorerna på den linje runt vilken rotationen sker!

Exempel på hur man beräknar egenvektorerna för en 3x3 [[Matris\|matris]]:
![beräkning av egenvektorer.png](/img/user/images/ber%C3%A4kning%20av%20egenvektorer.png)
[[Matris\|matrisen]] i exemplet ovan är inte [[Diagonalisering\|diagonaliserbar]] då det endast finns två egenvektorer


se: [Eigenvectors and eigenvalues | Chapter 14, Essence of linear algebra - YouTube](https://www.youtube.com/watch?v=PFDu9oVAE-g&list=PL0-GT3co4r2y2YErbmuJw2L5tW4Ew2O5B&index=14)