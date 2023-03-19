---
{"dg-publish":true,"permalink":"/parametrisering/","tags":["linjäralgebra"]}
---

Metoden att använda ett tal för att säga var på en kurva man är.

$z: R \rightarrow C$ 

När vi låter parametern t variera får vi olika punkter på kurvan. Om t går från a till b kommer a vara startpunkten på kurvan och b vara slutpunkten. Den vanligaste fysikaliska motsvarigheten är att t motsvarar tid.

Väljer man en parametrisering väljer man också en riktning eller [[Orientering\|Orientering]] på kurvan. 

Kurvans tangent ges av $z'(t) = x'(t)+iy'(t)$ och motsvarar hastigheten av kurvan.

För att kunna parametrisera behöver kurvan vara “[[Slät Kurva\|slät]]”, dvs ha tangenter. En kvadrat är inte [[Slät Kurva\|slät]] då det inte finns någon tangent i hörnen. Man kan dela upp kurvan i flera [[Slät Kurva\|släta kurvor]] och summera dess [[Kurvintegraler\|kurvintegraler]]. 

> Det finns oändligt många parametriseringar

## Parameterform
För en **rät linje i planet** kan en parametrisering se ut som
$$
\begin{cases}
x=a_{0}+ta \\ y=b_{0}+tb 
\end{cases}
\space,\space t\in \mathbb{R}
$$
det kallas en *ekvation på parameterform* (trots att det egentlige är ett [[System (matematisk definition)\|System (matematisk definition)]] med två ekvationer). För att avgöra om två punkter ligger på linjen är det bara att mata in x och y värdet och se vad man får för värde på t (man måste veta vilken linje det är, dvs $t$ är den enda obekanta). Om det är samma $t$ för både x och y kan man konstatera att punkten ligger på linjen.

För ett **plan i rummet** behöver man två parametrar ($s$ och $t$), men konceptet är exakt samma. Kan se ut som följande
$$
\begin{cases}
x=a_{0}+sa_{1}+ta_{2} \\
y=b_{0}+sb_{1}+tb_{2} \\
z=c_{0}+sc_{1}+tc_{2} 
\end{cases} \space,\space s,t\in \mathbb{R}
$$

se också [[Normalform\|Normalform]]
