---
{"dg-publish":true,"permalink":"/transfer-function-vs-linear-state-space-model/","tags":["reglerteknik"]}
---


[[Överföringsfunktion\|Transfer functions]] and [[Linear state-space model\|state-space models]] are two types of [[Process Models\|Process Models]]. They are good for different things.

### [[Överföringsfunktion\|Transfer functions]]
**Good**:
* Turns everything into [[Funktionsteori\|complex analysis]]. 
* Good for interconnection - turns it into algebra
* Can handle delays
**Bad**:
- Computations is hard
- MIMO mess

### [[Linear state-space model\|Linear State-space model]]
**Good**:
- Can use [[Linjär Algebra\|Linear Algebra]] theory for studying our [[feedback\|feedback]] control problem. 
* Great for computation
* Good for MIMO (multiple input multiple output)
**Bad**:
* interconnection is messy (e.g having several "blocks" in a circuit)
* delays are very hard to model