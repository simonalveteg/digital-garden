---
{"dg-publish":true,"permalink":"/summa-av-diskreta-stokastiska-variabler/","tags":["matematiskstatistik"]}
---

Om $X, Y$ är diskreta och endast antar heltalsvärden blir [[Sannolikhetsfunktion\|sannolikhetsfunktionen]]
$$
p_Z(k)=P(Z=k)=P(X+Y=k).
$$

Vi bestämmer fördelningen för $Z$ på följande sätt: Man kan ha $X=0,Y=k$ eller $X=1,Y=k-1$ osv ända till $X=k,Y=0$. [[Sannolikhet\|Sannolikheten]] för [[Händelse\|händelsen]] ifråga kan alltså uttryckas som summan
$$
p_Z(k)=P(X+Y=k)=\sum_{i+j=k}p_{X,Y}(i,j)=\sum_{i=0}^{k}p_{X,Y}(i,k-i).
$$
Analogt blir 
$$
F_Z(z)=\sum_{i+j\leq z}p_{X,Y}(i,j).
$$

Om $X$ och $Y$ är [[Oberoende Stokastiska Variabler\|oberoende]], vilket är vanligt!, får vi [[Faltningsformeln för oberoende diskreta stokastiska variabler\|Faltningsformeln för oberoende diskreta stokastiska variabler]]

