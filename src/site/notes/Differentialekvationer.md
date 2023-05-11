---
{"dg-publish":true,"permalink":"/differentialekvationer/","tags":["systemochtransformer"]}
---


Differential equations relates a function or set of function to its derivatives.

[[Ordinary Differential Equations\|Ordinary Differential Equations]]
[[Homogena Differentialekvationer\|Homogena Differentialekvationer]]
[[Inhomogena Differentialekvationer\|Inhomogena Differentialekvationer]]

## Steg för steg
1. Räkna ut [[Egenvärden\|egenvärden]] och [[Egenvektorer\|egenvektorer]] för att kunna ta fram en [[Diagonalmatris\|diagonalmatris]], samt basbytesmatrisen S.
	1. Om $\vec{F(t)}\neq0$ ta fram $S^{-1}$
2. Utför variabelbyte (oftast $\vec{x}=S\hat{x}$) 
3. Om A är [[Diagonalisering\|diagonaliserbar]] kan den skrivas om som $SDS^{-1}$. Nu kan du byta ut dina äckliga x mot fina x med hattar.
4. Sätt in alla värden du har, och ta fram uttryck för $\hat{x}'$. Använd [[Integrerande Faktor\|integrerande faktor]] för att få fram $\hat{x}$. 
5. $\vec{x}=S\hat{x}$, dvs multiplicera med S för att få fram $\vec{x}$. 
6. Använd eventuella begynnelsevillkor. kukhuvud 🤪