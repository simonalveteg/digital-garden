---
{"dg-publish":true,"permalink":"/decimal-point-to-binary-point/","tags":["numeriskanalys"]}
---


Låt säga att du vill göra om 0.4 från decimal till binärt. Börja med 0.4 och multiplicera med 2. Ta Decimalen och multiplicera med två. Fortsätt så tills du får 0 som decimal, eller 0.4 igen. Om du får 0.4 igen så vet du att den kommer fortsätta för evigt, om du får 0 är den klar.

$$
\begin{align}
0.4\cdot2&=0.8 & 0 \\
0.8\cdot2&=1.6 & 1 \\
0.6\cdot2&=1.2 & 1 \\
0.2\cdot2&=0.4 & 0
\end{align}
$$

Svaret fås av siffran innan decimalen? Decimalen är väl egentligen fel ord för att det har med decimaler att göra, typ "decimal point" och "binary point" är inte samma sak?