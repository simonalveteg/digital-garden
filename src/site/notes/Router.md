---
{"dg-publish":true,"permalink":"/router/","tags":["kommunikationssystem"]}
---

An internetworking device with two functions
1. Routing - finding the route between two devices
2. Forwarding - sending the information in the right direction

En router arbetar på [[Network Layer\|nätverksnivån]] men måste också kunna förstå [[Physical Layer\|fysiska lagret]] och [[Data Link Layer\|länklagret]] för att kunna kommunicera på LAN.

Routern har **köer** på både in och utgången för att den inte ska behöva slänga [[Packet\|paket]] om den är upptagen. Det innebär en liten fördröjning medan paketen väntar på att bli behandlade. I ingångskön väntar [[Packet\|paket]] på att bli behandlade och på utgångskön väntar de på att bli skickade.

Routing is a part of the [[Network Layer\|Network Layer]] of both the [[OSI model\|OSI model]] and [[TCP IP model\|TCP/IP model]].

[[Routing Algorithms\|Routing Algorithms]]
[[Nätverksparametrar som en ny enhet behöver ta reda på\|Nätverksparametrar som en ny enhet behöver ta reda på]]
