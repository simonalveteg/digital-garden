---
{"dg-publish":true,"permalink":"/stop-and-wait-arq/","tags":["kommunikationssystem"]}
---


Send a packet and wait for ACK. Retransmit upon timeout. 
![Pasted image 20230123163647.png](/img/user/images/Pasted%20image%2020230123163647.png)

Om sändaren tar emot ett ACK för ett äldre sekvensnummer kommer den ignorera det. Den bryr sig bara om det senaste sekvensnumret. Ex: skickar 13, väntar tills den får ACK13, skickar 14...

The sender never sends more than one package at a time. Leads to too much waiting. The solution is to keep the pipe full but not too full → [[Sliding Window\|Sliding window]].