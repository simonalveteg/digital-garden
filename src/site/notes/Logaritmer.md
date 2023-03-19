---
{"dg-publish":true,"permalink":"/logaritmer/","tags":["funktionsteori"]}
---


invers till en exponentialfunktion
# Komplext
Varje [[Komplexa Tal\|komplext tal]] har oändligt många logaritmer. 

Lös $e^w=z$ ($z$ givet). 
En lösning $w$ kallas en komplex logaritm till $z$.
Enklaste sättet att lösa ekvationen är att skriva $z$ på [[Polär form\|polär form]] och $w$ på [[Rektangulär Form\|rektangulär form]]:
$$
e^ae^{ib}= e^{a+ib} = e^{w} = z = re^{i\theta}
$$
$ib$ och $i\theta$ är tal på enhetscirkeln, $e^a$ och $r$ är absolutbeloppet.
$$
\begin{cases}
e^{a=r}\\ e^{ib}=e^{i\theta}
\end{cases}
\Rightarrow
\begin{cases}
a=lnr \\ b = \theta + 2\pi n
\end{cases}
$$
Om $z=re^{i\theta}$ så blir lösningarna till $e^w=z$ $logz=w=ln|z|+iargz$ 
### Problem
1. Om $z=0$ saknas lösning
2. om $z\neq 0$ är lösningen inte entydig: varje val av $argz$ ger en logaritm.
(man skriver log för att skilja på den reella logaritmfunktionen och den komplexa logaritmfunktionen. Det är den naturliga logaritmen) 


man vill få en [[Definitionsmängd\|definitionsmängd]] som är [[Enkelt sammanhängande\|enkelt sammanhängande]], vilket kan göras genom att ta bort en axel eller en halvaxel, vilket ger olika grenar beroende på vad man tar bort
## Principalgrenen
> $Logz = ln|z|+iArgz$

och $Logz$ är principalgrenen, där $Argz$ är principalargumentet av z, dvs det [[Argument\|argument]] som ligger mellan $-\pi$ och $\pi$

> Om man ska beräkna principalgrenen så vet man att argumentet ska vara principalargumentet, och därmed ligga mellan $-\pi$ och $\pi$

[[Definitionsmängd\|definitionsmängden]] blir inte hela det komplexa planet, men man får ett bestämt svar, istället för oändligt många.

De vanliga räknereglerna gäller inte fullt ut.
ex:
$Logi = \frac{i\pi}{2}$
$Logi^{2} = Log(-1) \neq 2Logi$ - inte ens definierat!
> Räknereglerna gäller som vanligt om argumentet är principalargumentet

## Naturliga grenen
Ett annat sätt? Ta bort positiva reella tal och välj argument mellan $0$ och $2\pi$ . Oavsett om man väljer principalgrenen eller någon annan typ av logaritm så blir den alltid deriverbar.