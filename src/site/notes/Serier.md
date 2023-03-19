---
{"dg-publish":true,"permalink":"/serier/","tags":["funktionsteori"]}
---

Serier är oändliga [[Summor\|summor]]. Tal på decimalform är egentligen oändliga [[Summor\|summor]].

Låt $(a_{n})_{n=1}^{\infty}$ vara en talföljd. Bilda en oändlig summa, vars termer är elementen i talföljden, serien $\sum\limits_{k=1}^{\infty}a_{k}=a_{1}+a_{2}+a_{3}+...$
Bilda partialsummor genom att lägga ihop fler och fler tal 
$$s_{N}=\sum\limits_{k=1}^{N}a_{k}=a_{1}+a_{2}+...+a_N$$
Serien $\sum\limits_{k=1}^{\infty}a_{k}$ kallas [[Konvergens\|konvergent]] om följden av partialsummor har ett gränsvärde! dvs om 
$$s=\lim_{N\rightarrow\infty}s_{N}=\lim_{N\rightarrow\infty}\sum\limits_{k=1}^{N}a_{n}$$
existerar (s är ett tal! dvs inte $\pm \infty$ )
Serier som inte är konvergenta kallas divergenta. 

I allmänhet är det hopplöst att beräkna $s_N$ exakt. Går oftast inte att hitta en formel för $s_{N}$. Vi behöver indirekta metoder för att avgöra om en serie [[Konvergens\|konvergerar]] eller divergerar. För [[Geometriska serier\|geometriska serier]] kan man beräkna partialsummor!
 
Det finns flera olika sorters serier
[[Geometriska serier\|Geometriska serier]]
[[Positiva Serier\|Positiva Serier]]
[[P-Serier\|P-Serier]]
[[Allmänna Serier\|Allmänna Serier]]
[[Alternerande Serier\|Alternerande Serier]]
[[Funktionsserier\|Funktionsserier]]
[[Fourierserier\|Fourierserier]]
[[Potensserier\|Potensserier]]

[[Strategier för att avgöra seriers konvergens\|Strategier för att avgöra seriers konvergens]]

# Uppskattning av seriers värde
Om vi har en [[Konvergens\|konvergent]] serie är det naturligt att försöka beräkna summan. Vi kan beräkna ett närmevärde till 

> Det finns inget allmänt sätt att uppskatta en series värde

Ersätt seriens värde med en ändlig partialsumma, men hur stort blir felet i den approximationen? - dvs uppskatta ***resttermen***.
$$
s = \sum\limits_{k=1}^{n}a_{k}+\sum\limits_{k=n+1}^{\infty}a_{k}=s_{n}+r_{n}
$$
vi vill visa att $|r_{n}|$ är litet. Om serien är [[Absolut Konvergent\|absolutkonvergent]] kan vi utnyttja [[Triangelolikheten\|triangelolikheten]];
$$
|r_{n}|=|\sum\limits_{k=n+1}^{\infty}|\leq\sum\limits_{k=n+1}^{\infty}|a_{k}|
$$
### Metod 1: jämförelse
Beräkna resttermen genom att jämföra serien med en *annan* (större) serie, som vi kan beräkna (oftast en [[Geometriska serier\|geometrisk serie]]). “Hur stort fel får vi om vi uppskattar serien med dess n första termer?”
 $r_{x}=s-s_{x}=\sum\limits_{x+1}^{\infty}a_{x}$ 
 där r är resttermen. Serien kan oftast uppskattas uppåt till en [[Geometriska serier\|geometrisk serie]] som faktiskt går att lösa, vilket ger oss en övre gräns för r. Den undre gränsen är 0.

### Metod 2: integraltest
Om $a_{k}=f(k)$ där f avtagande och positivt så gäller
$$
\int_{N+1}^{\infty}f(x)dx\leq r_{N}=\sum\limits_{k=N+1}^{\infty}f(k)\leq\int_{N}^{\infty}f(x)dx
$$
vilket ger
$$
r_{N}\leq\int_{N}^{\infty}f(x)dx
$$
### Metod 3: uppskatta mha Leibniz
Denna metod gäller endast för serier som uppfyller [[Leibniz test för alternerande serier\|Leibniz test för alternerande serier]].
1. visa att serien uppfyller testet

# Uppskattning av resttermen
När man beräknar en serie i praktiken vill man inte välja ett n som är för litet, men samtidigt inte ett n som är onödigt stort. För att avgöra när ett n är lagom stort kan man uppskatta resttermen, dvs skillnaden mellan $s$ och $s_{n}$. 

