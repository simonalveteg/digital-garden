---
{"dg-publish":true,"permalink":"/matrismultiplikation/","tags":["linjäralgebra"]}
---


När man multiplicerar två [[Matris\|matriser]] med varandra kan man se det som att man först utför en [[Linjär Avbildning\|linjär avbildning]], och sen en till. [[Matris\|Matrisen]] längst till höger är den som utförs först. Matrismultiplikation är inte [[Kommutativ\|Kommutativ]], och är [[Associativ\|Associativ]].
![matrix multiplication order.png](/img/user/images/matrix%20multiplication%20order.png)
Rad gånger kolumn! Rad ett gånger kolumn ett hamnar på rad ett kolumn ett i den nya [[Matris\|matrisen]].
![Pasted image 20220313005438.png](/img/user/images/Pasted%20image%2020220313005438.png)

För att kunna multiplicera ihop två [[Matris\|matriser]] $AB$ måste det finnas lika många rader i $B$ som kolonner i $A$. Detta eftersom man tar skalärprodukten mellan raderna i $A$ och kolonnerna i $B$, och de måste ha samma typ.

Om A är av typ $p\times q$ och B av typ $q \times r$ blir produkten $p \times r$ .