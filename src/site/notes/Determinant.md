---
{"dg-publish":true,"permalink":"/determinant/","tags":["systemochtransformer","linjäralgebra"]}
---


Determinanten kan ses som ett mått på hur arean som spänns upp av två [[Linjärt Oberoende\|linjärt oberoende]] [[Vektorer\|vektorer]] förändras av en [[Linjär Avbildning\|Linjär Avbildning]]. 

$$
\det A = \begin{vmatrix} a&b\\c&d\end{vmatrix}=ad-bc
$$
![determinantdefinitiongeometriskt.png|500](/img/user/images/determinantdefinitiongeometriskt.png)
beräkningen funkar likadant som i bilden ovan för [[Matris\|matriser]] med n>2. Tänk bara att man tar högerdiagonaler minus vänsterdiagonaler (som ovan), fast att man “wrappar” runt när man kommer till kanten. Alla diagonaler ska ha gåtts igenom, som i bilden nedan
![determinantberäkning.png](/img/user/images/determinantber%C3%A4kning.png)

Övrigt gäller också att 
$$
\det(M_{1}M_{2})=\det(M_{1})\det(M_{2})
$$
vilket kan rättfärdigas genom att tänka att varje [[Linjär Avbildning\|linjär avbildning]] förändrar arean med en viss faktor, och att slå ihop determinanterna av den ena och den andra är samma sak som att räkna ut en determinant av kombinationen av de båda [[Avbildningsmatris\|avbildningsmatriserna]].


Determinanten av en [[Linjär Avbildning\|linjär avbildning]] blir noll om avbildningen trycker ihop rummet till en lägre dimension. För att determinanten ska bli noll måste minst två kolonner i [[Matris\|matrisen]] vara [[Linjärt Beroende\|linjärt beroende]]. Om rummet trycks ihop till ett plan finns det en hel linje med [[Vektorer\|vektorer]] som landar i origo. “Rummet” som dessa [[Vektorer\|vektorer]] spänner upp kallas för [[Nollrum\|Nollrum]].

Om determinanten är negativ är det samma sak som att byta vektorernas [[Orientering\|orientering]].