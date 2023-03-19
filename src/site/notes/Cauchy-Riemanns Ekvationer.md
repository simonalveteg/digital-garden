---
{"dg-publish":true,"permalink":"/cauchy-riemanns-ekvationer/","tags":["funktionsteori"]}
---

Om Cauchy-Riemanns ekvation stämmer så är funktionen [[Holomorf\|holomorf]] på området (dvs deriverbar).

Om man bara har funktionen för imaginärdelen kan man med hjälp av C-R beskriva hur realdelen kan se ut och därmed också hur f kan se ut. 

$$ \begin{cases} u'_{x} (a,b) =  v'_{y}(a,b) \\  u'_{y}(a,b) = -v'_{x}(a,b)
\end{cases}$$


## Bevis
Anta att f är (komplext) deriverbar i punkten $z=a+ib$, dvs att 
$$\lim_{h→0} \frac{f(z+h)-f(z)}{h}$$
om h är rent reellt
$$z = a+ib, z+h = (a+h)+ib$$
$$\begin{align*}
f'(z)=\lim_{h→0}\frac{f(z+h)-f(z)}{h} = \lim_{h→0}\frac{u(a+h,b)+iv(a+h,b)-(u(a,b)+iv(a,b))}{h} \\= \lim_{h→0} \frac{u(a+h,b)-u(a,b)}{h} + i\frac{v(a+h,b)-v(a,b)}{h} \\= u'_{x}(a,b) + iv'_{x}(a,b)
\end{align*}$$
om h är rent imaginärt blir derivatan istället
$$f'(z) = \frac{1}{i}u'_y(a,b)+v'_{y(a,b))}= v'_{y}(a,b)-iu'_y(a,b)$$

dvs om $f'(z)$ existerar så är 
$$f'(z) =  v'_{y}(a,b)-iu'_{y(a,b)} = u'_{x}(a,b) + iv'_{x}(a,b)$$
vilket ger Cauchy-Riemanns ekvationer:
$$ \begin{cases} u'_{x} (a,b) =  v'_{y}(a,b) \\  u'_{y}(a,b) = -v'_{x}(a,b)
\end{cases}$$


## Konsekvenser av C-R’s ekvationer
1. Om $f=u+iv$ är [[Holomorf\|holomorf]], så är u entydigt [[Holomorf\|holomorf]] av v
2. Alla funktioner är inte realdelen till någon [[Holomorf\|holomorf]] funktion
3. Om f är [[Holomorf\|Holomorf]] och $f'(z) = 0$ för alla z, så måste f vara konstant (om [[Definitionsmängd\|definitionsmängden]] är sammanhängande)
	* ![bevis_konsekvens_3_CR.png](/img/user/images/bevis_konsekvens_3_CR.png)
4. 

Sats. Om $f=u+iv$ är [[Holomorf\|holomorf]], så måste både u och v vara [[Holomorf\|holomorfa]]
Bevis: $$u''_{xx}=(u'_x)'_{x}=(v'_y)'_{x}= v''_{xy}$$
(och vice versa). Om u och v är [[Harmonisk Funktion\|harmoniska]] måste du u+iv vara [[Holomorf\|holomorf]]? Nej! u och v måste dessutom tillsammans uppfylla Cauchy-Riemanns ekvationer.

**[[Enkelt sammanhängande\|Enkelt sammanhängande]]**
[[Harmonisk Funktion\|Harmonisk Funktion]]

