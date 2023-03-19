---
{"dg-publish":true,"permalink":"/link-state-routing-algorithm/","tags":["kommunikationssystem"]}
---

The local topology info is flooded globally. The routing tables are updated upon link state changes and cost changes. 

The link state is the cost of every link
![Pasted image 20230214160011.png](/img/user/images/Pasted%20image%2020230214160011.png)

Link state använder [[Dijkstras Algorithm\|Dijkstras Algoritm]] när varje router bygger upp ett komplett träd med sig själv som rot.

See also -> [[Routing Algorithms\|Routing Algorithms]]