---
{"dg-publish":true,"permalink":"/hypotesproevning/","tags":["matematiskstatistik"]}
---

Hypotesprövning är en metod för att testa om en given teori är sann eller inte. Det görs genom att man formulerar en [[Nollhypotes\|nollhypotes]], det vill säga ett antagande som gör att teorin inte kan bevisas falskt. Sedan mäter man ett faktiskt resultat och jämför det med vad som förväntas enligt [[Nollhypotes\|nollhypotesen]]. Om det faktiska resultatet är så avvikande att det är osannolikt att det kan förklaras av slumpen, så kan man dra slutsatsen att [[Nollhypotes\|nollhypotesen]] är falsk och att teorin man testar är sann.

För att pröva [[Nollhypotes\|nollhypotesen]] $H_{0}$ hittar vi först på en lämplig *testvariabel* eller *teststorhet* $t=t_{obs}=t(x)$. Testvariabeln $t_{obs}$ är en observation av en stickprovsvariabel $t(X)$. Vi anger också ett kritiskt område $C$. Detta är en viss del av hela det område som $t$ varierar över. Sedan används [[Signifikanstest\|signifikanstest]]:

> Om
> $t_{obs}\in C$ förkasta $H_{0}$ (signifkant)
> $t_{obs}\notin C$ förkasta ej $H_{0}$. (icke-signifikant)

Vi avpassar $C$ så att 
$$
P(t(X)\in C)=\alpha \text{ om } H_{0} \text{ sann},
$$
där $\alpha$ väljs på förhand och kallas testets *signifikansnivå* eller *felrisk*. Den anger [[Sannolikhet\|sannolikheten]] att $H_{0}$ förkastas om $H_{0}$ är sann.

Hypotesprövning är nära sammanknutet med [[Intervallskattning\|Intervallskattning]].
