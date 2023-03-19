---
{"dg-publish":true,"permalink":"/selective-repeat-arq/","tags":["kommunikationssystem"]}
---


Mottagaren har möjligheten att spara [[Framing\|ramar]] som kom i fel ordning. Fördelen är att man inte behöver skicka om [[Framing\|ramar]] när de tagits emot korrekt. Man skickar alltså bara om [[Framing\|ramar]] som inte kommit fram ordentligt. Nackdelen är att mottagaren blir mer komplex.
![Pasted image 20230123165711.png](/img/user/images/Pasted%20image%2020230123165711.png)

Om sändaren får en ACK för ett tidigare sekvensnummer kommer den skicka om specifikt den ramen och sedan fortsätta där den var.

#question hur reagerar den på NAK?
