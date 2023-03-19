---
{"dg-publish":true,"permalink":"/vektorprodukt/","tags":["linjäralgebra"]}
---

Resultatet av vektorprodukten av två [[Vektorer\|vektorer]] är en ny [[Vektorer\|vektor]] som är vinkelrät mot planet som [[Vektorer\|vektorerna]] spänner upp. De tre [[Vektorer\|vektorerna]] tillsammans kan vara positivt eller [[Negativ Orientering\|negativt orienterade]], beroende på åt vilket håll den nya [[Vektorer\|vektorn]] är riktad. 


Beloppet av vektorprodukten (kryssprodukten) av två [[Vektorer\|vektorer]] ges av
$$
|u\times v| = |u|\space|v|\cdot \sin\theta
$$
dvs längderna av [[Vektorer\|vektorerna]] gånger sinus av vinkeln mellan dem. Kan jämföras med [[Skalärprodukt\|Skalärprodukt]] där det är cosinus istället för sinus, och resultatet inte är ett belopp.

[[Orientering\|Orienteringen]] spelar roll, det vill säga att $u\times v \neq v\times u$, då det inte är samma vinkel. Vinkeln är lika stor men negativ, och då sinus är en udda funktion blir $u\times v = -v\times u$. ($sin(-\theta)=-sin(\theta)$).
![vektorprodukt.png](/img/user/images/vektorprodukt.png)
Om man jämför med vårt vanliga XY-koordinatsystem blir v=x, w=y och kryssprodukten=z!

The magnitude $|AB\sin \theta_{AB}|$ is the area of parallelogram with two sides formed by $\vec{A}$ and $\vec{B}$.

The vector product is 
1. NOT cumulative (the magnitude is the same but the direction is reversed)
2. Distributive
3. NOT [[Associativ\|associative]]

# For Orthogonal Coordinates

$$\vec{A} \times \vec{B}=\begin{vmatrix}  \vec{a}_{u_{1}} & \vec{a}_{u_{2}} &  \vec{a}_{u_{3}} \\ A_{u_{1}} & A_{u_{2}} & A_{u_{3}} \\ B_{u_{1}} & B_{u_{2}} & B_{u_{3}}\end{vmatrix}$$

