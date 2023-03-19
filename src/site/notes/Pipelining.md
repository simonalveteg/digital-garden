---
{"dg-publish":true,"permalink":"/pipelining/","tags":["datorteknik"]}
---

Pipelining är ett sätt att öka prestandan, dvs göra exekveringen av ett program snabbare. Man börjar med nästa instruktion innan nästa instruktion är färdig. Medan instruktion 1 exekveras fetchas instruktion 2 osv. Fler pipeline steg ger alltså bättre prestanda, men det blir också mer overhead att hålla koll på pipeline och därmed en mer komplex processor. Det är även svårt att hålla pipelinen full

För att kunna hantera pipelines behöver processorn delas av med register mellan varje pipeline-steg.

![Pasted image 20230131150824.png](/img/user/images/Pasted%20image%2020230131150824.png)

Det är först när vi har aktivitet i alla pipelines som pipelinen är full. Det är bra att ha pipelinen full med instruktioner.

När vi inte har pipelining kommer vi ha olika exekveringstider för varje instruktion, men med pipelining kommer en instruktion vara klar efter en viss tid hela tiden.

Kontrollenheten måste hålla koll på pipelinesen, vilket gör att processorn blir mer komplex.

[[Pipeline Hazards\|Pipeline Hazards]] är problem som förhindrar att nästa intruktion i programmet exekveras direkt.

[[Branch Prediction\|Branch Prediction]]
[[Instruction Fetch Unit\|Instruction Fetch Unit]]
[[Delayed Branching\|Delayed Branching]]