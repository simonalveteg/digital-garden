---
{"dg-publish":true,"permalink":"/talfoeljder/","tags":["funktionsteori"]}
---

En följd av (komplexa) tal.

Man kan se en talföljd som en funktion där man oftast skriver $a_4$ istället för $a(4)$.

## Tre sätt att beskriva talföljder
1. Räkna upp några element i början, avsluta med … och hoppas att det är tillräckligtt tydligt
	- Kan vara vilken talföljd som helst, så det är inte direkt entydigt.
2. Explicita uttryck “formel på $a_n$”
	- ex $a_{n}=2^{n}$
3. [[Rekursion\|Rekursivt]] - nästa element skapas av något (eller alla) föregående tal i följden
	- Oftast är det så man bygger upp talföljder. [[Rekursionsekvationer\|Rekursionsekvationer]] är ett förhållandevis lätt sätt att räkna ut talföljder
## Egenskaper för talföljder
uppåt begränsad - det finns ett tal K så att alla tal i talföljden är mindre än K
nedåt begränsad - det finns ett tal K så att alla tal i talföljden är större än K
begränsad - både uppåt och nedåt begränsad
strikt växande - nästa tal i följden är större än föregående
strikt avtagande - nästa tal i följden är mindre än föregående
monoton - växande eller avtagande
## Gränsvärden för talföljder
![Pasted image 20220201091923.png](/img/user/images/Pasted%20image%2020220201091923.png)
En talföljd $(a_{n})^{\infty}_{n=0}$ har gränsvärdet L då $n \rightarrow \infty$ om det till varje $\epsilon > 0$ finns N så att 
$$|a_{n}-L|<\epsilon$$ om $n \geq N$ . ($N$ beror av $\epsilon$)