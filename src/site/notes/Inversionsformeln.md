---
{"dg-publish":true,"permalink":"/inversionsformeln/","tags":["systemochtransformer"]}
---


$f(t)\xrightarrow{\mathcal{L}}F(s) \Rightarrow f(t)$ kallas för den inversa [[Laplacetransformationer\|Laplacetransformen]] av $F(s)$. Det skriver vi som 
$$f(t)=\mathcal{L}^{-1}(F(s))(t)$$
men detta är för jobbigt för att använda när man räknar. Man kan istället använda
$$f(t)=\frac{1}{2\pi i}\int_{\gamma\sigma}e^{st}F(s)ds$$
där $\gamma\sigma$ är en vertikal linje som ligger i den vertikala strimlan som är [[Definitionsmängd\|definitionsmängden]] till $F(s)$. Men den är också jobbig???? Vi använder formler i formelbladet och går baklänges för att hitta inversa [[Laplacetransformationer\|laplacetransformationen]]. För att göra det måste vi veta information om strimlan, alltså om $Re(s)$ är större eller mindre än noll.

## Se också
[[Inversionsformeln för Fouriertransformationer\|Inversionsformeln för Fouriertransformationer]]