---
{"dg-publish":true,"permalink":"/punktskattning/","tags":["matematiskstatistik"]}
---

Punktskattning går ut på att välja ut en representativ grupp individer från populationen och sedan använda data från dessa för att dra slutsatser om hela populationen. Vid den statistiska bedömningen betraktas det stickprov man gör som ett stickprov taget ur den hypotetiska mängden av alla stickprov.

> En *punktskattning* $\theta_{obs}^{*}=\theta^{*}(x_{1},x_{2},\dots,x_n)$ av en parameter $\theta$ är en funktion av mätdata $x_{1},x_{2},\dots,x_n$. Dessa mätdata ses som [[Utfall\|utfall]] av [[Stokastisk Variabel\|stokastiska variabler]] $X_{1},X_{2},\dots,X_n$ vilkas fördelning beror av parametern $\theta$. Punktskattningen $\theta_{obs}^{*}$ är ett [[Utfall\|utfall]] av *stickprovsvariabeln* $\theta^{*}=\theta^{*}(X_{1},X_{2},\dots,X_n)$.

$\theta_{obs}^{*}$ är alltså ett tal som är ett [[Utfall\|utfall]] av den [[Stokastisk Variabel\|stokastiska variabeln]] $\theta^{*}$ - stickprovsvariabeln. Att bestämma fördelningen för en stickprovsvariabel kan göras via simulering eller den analytiska metoden. 

Man vill att det slumpmässiga felet $\theta^{*}-\theta$ ska vara litet, ett mått på det ges av [[Medelkvadratfelet\|Medelkvadratfelet]]
[[Väntesvärdesriktig Punktskattning\|Väntesvärdesriktig Punktskattning]]
[[Konsistent Punktskattning\|Konsistent Punktskattning]]
[[Effektivitet av Punktskattning\|Effektivitet av Punktskattning]]
[[Medelfel för en skattning\|Medelfel för en skattning]]


En punktskattning ger inte alltid tillräcklig information om en okänd parameter, och det är ofta lämpligare att använda en [[Intervallskattning\|Intervallskattning]].