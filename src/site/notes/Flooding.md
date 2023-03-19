---
{"dg-publish":true,"permalink":"/flooding/","tags":["kommunikationssystem"]}
---

With flooding all incoming packets are copied out on all other ports. It is a very easy "algorithm", but it has flaws. A lot more packets are sent than what is needed, increasing congestion. It can also lead to looping, where a [[Packet\|packet]] that gets sent out comes back and blablabla loop du fattar.

See also -> [[Routing Algorithms\|Routing Algorithms]]