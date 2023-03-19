---
{"dg-publish":true,"permalink":"/multithreading/","tags":["datorteknik"]}
---

Istället för att ett program utför alla sina operationer på en tråd kan programmet använda flera trådar. När ett program behöver läsa något från I/O exempelvis, så blockas tråden tills inläsningen är klar. Multithreading gör att man kan byta tråd och exekvera något annat undertiden.

![Pasted image 20230120145857.png](/img/user/images/Pasted%20image%2020230120145857.png)
varje kolumn ovan är en [[Pipeline\|Pipeline]]. Fördelen med Simultaneous multithreading (SMT) är att mer kan göras samtidigt, men det blir även mer komplext att hålla reda på en sådan arkitektur.

# Interleaved Multithreading
![Pasted image 20230120145644.png](/img/user/images/Pasted%20image%2020230120145644.png)
Varje tråd får en liten tid att utföra sina operationer

# Blocked multithreading
![Pasted image 20230120145731.png](/img/user/images/Pasted%20image%2020230120145731.png)
Så länge en tråd kan exekvera får den exekvera, men när den blockar byter man tråd.