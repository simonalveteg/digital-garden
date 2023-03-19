---
{"dg-publish":true,"permalink":"/phantom-zero/","tags":["analogelektronik"]}
---


Det kallas fantom för att fantomnollan inte blir synlig i ekvationen för den [[Sluten förstärkning\|slutna förstärkningen]]. 

$\beta$  ska öka för höga frekvenser

Man kan placera fantomnollan på tre ställen i $\beta$
1. I [[feedback\|återkopplingsnätet]]
2. På förstärkarens utgång
3. På förstärkarens ingång

När du impementerar fantomnollan på ingången eller utgången:
	Sträva efter att göra källan/lasten mer ideal för höga frekvenser
Om källan/lasten ej är ideal kan vi inte förbättra [[Impedans\|impedansen]], vilket gör att man inte kan öka $\beta$, och där**med är kompensering med fantomnollställe inte möjligt.

## Metod
använd den naturliga metoden för a och beta
[[Nollställen\|nollställen]] i beta är fantomnollställen 
övriga [[Nollställen\|nollställen]] är [[Slingpoler och Slingnollställen\|slingnollställen]] 
fantomnollan är inte synlig i $A_{t}$ men en oönskad [[Poler\|pol]] uppstår (effektiviteten viktig, $\delta\geq7$)

Fantomnollställe uppstår då $|z_{1}|$ ökar eller $|z_{2}|$ minskar.

![Pasted image 20220412105042.png](/img/user/images/Pasted%20image%2020220412105042.png)
+glöm inte att $c_{\pi}\rightarrow \infty$ också i $\beta_{ph}$

för två [[Förstärkande Steg\|förstärkande steg]]:
$$n_{ph}=\frac{-\omega_{0}^{2}}{\sqrt{2}\omega_{0}+p_{1}+p_{2}}$$
$$n_{ph}=-\frac{1}{RC} =- \frac{R}{L}$$
$$C_{ph}=-
\frac{1}{n_{ph }R}$$
$$L_{ph}=-\frac{R}{n_{ph}}$$

## Var kan man sätta sin komponent?
Man vill sätta en [[Spole\|spole]] eller [[Kapacitans\|kondensator]] någonstans i sin slinga så att strömmen genom $r_{\pi}$ blir större! En [[Kapacitans\|kondensator]] parallellt med en resistans gör så att mer ström kan flöda för höga frekvenser (blir kortslutning), en [[Spole\|spole]] i serie gör så att ingen ström kan flöda för höga frekvenser (blir avbrott). Med en [[Spole\|spole]] kan man alltså “blockera” vissa vägar, och med [[Kapacitans\|kondensator]] kan man göra en väg lättare!


# Fantomnollans effektivitet
För ett andra ordningens [[System (matematisk definition)\|System (matematisk definition)]] med [[Systempoler\|systempoler]] i [[Butterworthposition\|Butterworthposition]] är det effektivt om $\delta\geq7$. 

när man räknar ut $\beta_{ph }(s)$ får man alltid en [[Poler\|pol]] $p_{ph }$ och ett [[Nollställen\|nollställe]] $n_{ph }$. $\delta= \frac{p_{ph}}{n_{ph}}$ ska alltså vara minst 7. 
