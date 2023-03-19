---
{"dg-publish":true,"permalink":"/instruction-fetch-unit/","tags":["datorteknik"]}
---

De flesta processorer har fetch unit som hämtar instruktioner innan de behövs. Dessa lagras i en instruktionskö. Fetch unit kan känna igen hoppinstruktioner och generera hoppadres. Penaltyn minskar för ovillkorliga hopp, men för villkorliga är det svårare då man måste veta om hoppet ska tas eller inte.

Branch History Table håller en historik av hoppinstruktioner och prediction bits.
![Pasted image 20230131165336.png](/img/user/images/Pasted%20image%2020230131165336.png)