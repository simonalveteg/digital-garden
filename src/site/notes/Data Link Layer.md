---
{"dg-publish":true,"permalink":"/data-link-layer/","tags":["kommunikationssystem"]}
---

Länkprotokoll används för att applikationsprotokollen inte ska behöva veta vilken slags länk som används i dataöverföringen. Termen [[Framing\|ram]] brukar användas istället för [[Packet\|paket]].


I data link layer ([[OSI model\|OSI model]]) måste vi kunna lösa tre problem
1. [[Error detection\|Error detection]]
2. [[Error correction\|Error correction]]
3. [[Flow control\|Flow control]]

Ett fel (error) i ett [[Kommunikationssystem\|kommunikationssystem]] är när den mottagna bitsekvensen inte stämmer med den sända.

![Pasted image 20230123153720.png](/img/user/images/Pasted%20image%2020230123153720.png)
Man kan lägga till extra bitar i slutet som encodas på ett specifikt sätt, så att mottagaren kan kontrollera att datan är felfri.
