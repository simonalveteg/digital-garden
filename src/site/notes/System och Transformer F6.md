---
{"dg-publish":true,"permalink":"/system-och-transformer-f6/","tags":["föreläsning","systemochtransformer"]}
---


[[Linjära System\|Linjära System]]
[[Kausala Funktioner\|Kausala Funktioner]]

**EXEMPEL:**
[[System (matematisk definition)\|Systemet]] $w(t)\xrightarrow{S}x(t)$ ges av 
$$\begin{cases}x'=2x+w(t)\\\\x(0)=0 \end{cases}$$
där insignalen $w(t)$ och utsignalen $x(t)$ är [[Kausala Funktioner\|kausala]]. Lösning ges av en standardformel som han gick igenom på [[System och Transformer F1\|System och Transformer F1]]
$$x(t)=\int_{0}^{t}e^{2(t-\tau)}w(\tau)d \tau =\int_{0}^{\infty}\theta(t-\tau)e^{2(t-\tau)}w(\tau)d \tau$$
[[Stegfunktion\|Stegfunktion]] är noll för $t-\tau<0$, så i intervallet $t \rightarrow\tau$ blir integralen noll och bidrar alltså ingenting, vilket är varför omskrivningen funkar. Vi får
$$=\int_{-\infty}^{\infty}\theta(t-\tau)e^{2(t-\tau)}w(\tau)d \tau$$
vilket kan jämföras med definitionen för [[Linjära System\|Linjära System]] och få [[Impulssvar\|impulssvaret]] 
$$k(t,\tau)=\theta(t-\tau)e^{2(t-\tau)}$$


[[Tidsinvarianta System\|Tidsinvarianta System]]
[[Impulssvar\|Impulssvar]]
[[Linjära och Tidsinvarianta System\|Linjära och Tidsinvarianta System]]
[[Delta Funktionen\|Delta Funktionen]]
[[Insignal-utsignalstabilt\|Insignal-utsignalstabilt]]
[[Kausala System\|Kausala System]]

# Subject
[[FMAF05 System och Transformer\|FMAF05 System och Transformer]]
