---
{"dg-publish":true,"permalink":"/rotort/","tags":["analogelektronik"]}
---


## Vad är rotort?
Rotorten är en grafisk representation av hur [[Systempoler\|systempolerna]] rör sig när [[Slingförstärkning\|slingförstärkningen]] ökar. När [[Slingförstärkning\|slingförstärkningen]] är noll befinner vi oss i våra [[Slingpoler och Slingnollställen\|slingpoler]]. När vi ökar [[Slingförstärkning\|slingförstärkningen]] (ex genom att ändra värden på resistorer? #question) förflyttar vi oss längs rotorten, och [[Systempoler\|systempolerna]] förflyttar sig ut från [[Slingpoler och Slingnollställen\|slingpolerna]]!! 

När man tog fram konceptet behövde man använda det för att geometriskt kunna lösa svåra uträkningar, som vi idag löser med datorer. Idag används det mest för att visualisera, eller få en intuitiv bild av vad som händer när man [[Frekvenskompensering\|frekvenskompenserar]]. - se [[Hur frekvenskompensering kan påverka rotorten - MFM system\|Hur frekvenskompensering kan påverka rotorten - MFM system]]

## Var är rotorten?
Från varje [[Poler\|pol]] går det ut en “gren”. De delar av reella axeln som har udda antal reella start- och ändpunkter (dvs [[Nollställen\|nollställen]] och [[Poler\|poler]]) till höger tillhör rotorten. När olika grenar av rotorten möts bryter de i 90 grader. Sedan går de mot asymptoterna. Asymptoterna bestäms av $\frac{\pi}{n-m}$ (n är antal [[Poler\|poler]] och m är antal [[Nollställen\|nollställen]]. speglas i x-axeln).

Antalet grenar = antalet [[Slingpoler och Slingnollställen\|slingpoler]] (n)
Rötterna till $P(s)=0$ är rotortens startpunkter $A \beta(0)=0$
Rötterna till $N(s)=0$ är rotortens ändpunkter $A \beta(0)\rightarrow\infty$


## Var skär asymptoterna x-axeln? (canonical point)
Om antalet [[Nollställen\|nollställen]] (m)<antal [[Poler\|poler]], går grenar utan ändpunkter till oändligheten. Dessa kallas asymptoter (n-m stycken). Asymptoterna skär x-axeln i punkten som ges av 
$$\frac{\sum\limits p-\sum\limits n}{n-m}$$
dvs summan av [[Poler\|poler]] minus summan av [[Nollställen\|nollställen]] genom (antalet [[Poler\|poler]] minus antalet [[Nollställen\|nollställen]])

bra läsning: [5.1: Root Locus Fundamentals - Engineering LibreTexts](https://eng.libretexts.org/Bookshelves/Industrial_and_Systems_Engineering/Book%3A_Introduction_to_Control_Systems_(Iqbal)/05%3A_Control_System_Design_with_Root_Locus/5.01%3A_Control_System_Design_with_Root_Locus)

## Vad säger den oss?
Den visar hur [[Systempoler\|systempolerna]] förflyttar sig i [[Laplace-planet\|Laplace-planet]]. Ju närmre den imaginära axeln polerna ligger desto mindre är den exponentiella komponenten, vilket ger upphov till ringning i [[Stegsvar\|stegsvaret]].

Ju närmre [[Systempoler\|systempolerna]]/rotorten är den imaginära axeln desto mindre är [[Fasmarginal\|fasmarginalen]]!





Iman gick igenom ett [[Övning i Analog Elektronik 2022-03-29\|exempel för två poler]] på ett övningstillfälle.