---
{"dg-publish":true,"permalink":"/conditional-signal-assignment/","tags":["digitalteknik"]}
---

![Pasted image 20211108104910.png](/img/user/images/Pasted%20image%2020211108104910.png)

Börja med en sanningstabell
![Pasted image 20211108104930.png](/img/user/images/Pasted%20image%2020211108104930.png)

```vhdl
library IEEE;
use IEEE.STD_LOGIC_1164.all;

entity comb1 is 
	port(a, b, c : in STD_LOGIC;
		q : out STD_LOGIC);
end entity comb1;
	
architecture a_comb1 of comb1 is
begin
	q <= '1' when a='0'else
		'1' when (b='1'and c='1') else
		'0';
end architecture a_comb1;
```

Jämför med [[Simple Signal Assignment\|Simple Signal Assignment]]. Här beskriver man kretsens beteende, men det beskrivs inte på gate-nivå. I denna koden har $a$ högst prioritet.