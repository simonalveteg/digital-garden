---
{"dg-publish":true,"permalink":"/funktioner-av-en-stokastisk-variabel/","tags":["matematiskstatistik"]}
---

Man är ofta intresserad av att betrakta en funktino $Y=g(X)$ av en [[Stokastisk Variabel\|stokastisk variabel]] $X$. Då är $Y$ en [[Stokastisk Variabel\|stokastisk variabel]] vars fördelning kan bestämmas om fördelningen för $X$ är känd. 

# Vid diskret fördelning
Om $X$ har en diskret fördelning kan man bestämma $g(x)$ för alla tänkbara värden på $X$ och få fördelningen direkt genom lämpligt utförd addition av [[Sannolikhetsfunktion\|sannolikhetsfunktionen]].
$$
p_Y(k)=\sum_{j:g(j)=k}p_x(j)
$$
# Allmänt
Genom att bestämma [[Fördelningsfunktion\|fördelningsfunktionen]] $F_{Y}(y)$ för $Y$, sedan kan man på känt sätt bestämma [[Täthetsfunktion\|täthetsfunktionen]]/[[Sannolikhetsfunktion\|sannolikhetsfunktionen]] #question hur?. Tillvägagångssättet är eklast om $g(x)$ är antingen strängt växande för alla x eller strängt avtagande för alla x. 
