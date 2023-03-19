---
{"dg-publish":true,"permalink":"/bandbreddsuppskattning/","tags":["analogelektronik"]}
---

[[Bandbredd\|Bandwidth]] estimation gives us the maximum achievable [[Bandbredd\|bandwidth]] when we compensate a [[System (matematisk definition)\|System (matematisk definition)]] with some [[Slingpoler och Slingnollställen\|loop-poles]]. [[Bandbredd\|Bandwidth]] estimation is done using LP: [[LP-produkten\|Loop-gain pole product]] $= | 1-AB(0) |p_1p_2p_3…p_n$(n [[Dominanta och Icke-dominanta poler\|dominanta poler]]).
$$BW=\omega_0=LP_{n}^\frac{1}{n}$$

# Flöde för bandbreddsuppskattning
Beräkna [[LP-produkten\|LP-produkten]]
Skatta [[Bandbredd\|bandbredden]]
Välj [[Systempoler\|systempolernas]] lägen (Butterworth) för skattad [[Bandbredd\|bandbredd]]
Beräkna summan av [[Slingpoler och Slingnollställen\|slingpolerna]] respektive [[Systempoler\|systempolerna]]
Kontrollera att [[Slingpoler och Slingnollställen\|slingpolerna]] är [[Dominanta och Icke-dominanta poler\|dominanta]] 
Finns [[Dominanta och Icke-dominanta poler\|icke-dominant pol]], ta bort den mest negativa och börja om
KLART 🤪🤪🤪🤪🤪🤪🤪🤪🤪🤪