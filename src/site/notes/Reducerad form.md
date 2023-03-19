---
{"dg-publish":true,"permalink":"/reducerad-form/","tags":["digitalteknik"]}
---


## Reducerad form av [[Linear Sequential Circuit\|linjära sekvensnät]]
1. Ta fram [[Diagnostic Matrix\|K-matrisen]] och räkna ut dess [[Rang\|rang]]. Om rangen är mindre än antalet rader så går kretsen att minimera. 

2. Bilda en ny [[Matris\|matris]] T genom at ta de X första raderna från K.  (X=rangen) 

3. Hitta en [[Invers Matris#Högerinvers\|högerinvers]] R till T
Tänk att $$T = \begin{pmatrix}M N\end{pmatrix}$$ där M är en [[Kvadratisk Matris\|kvadratisk matris]]. För att bilda M tar man tre [[Linjärt Oberoende\|Linjärt Oberoende]] kolumner från T. Hitta $M^{-1}$ istället. 
$$R=\begin{pmatrix}M^{-1}\\0\end{pmatrix}$$
man kan alltså skita i N, då den kommer multipliceras med nollan.

4. För att hitta den reducerade formen multiplicerar man sedan sina [[Matris\|matriser]] A, B, C och H (se [[Linear Sequential Circuit\|linjära sekvensnät]]) på följande vis:
![Pasted image 20211028104922.png](/img/user/images/Pasted%20image%2020211028104922.png)