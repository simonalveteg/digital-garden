---
{"dg-publish":true,"permalink":"/selected-signal-assignment/","tags":["digitalteknik"]}
---

![Pasted image 20211108105438.png](/img/user/images/Pasted%20image%2020211108105438.png)

```vhdl
library IEEE;
use IEEE.STD_LOGIC_1164.all;

entity comb1 is 
	port(a, b, c : in STD_LOGIC;
		q : out STD_LOGIC);
end entity comb1;
	
architecture a_comb1 of comb1 is 
	signal abc : STD_LOGIC_VECTOR(2 downto 0);
	with abc select
	q <= '1' when "000" | "001" | "010" | "011",
	'1' when "111",
	'0' when others;
end architecture a_comb1;
```

Kretsen beskrivs på en lite högre [[Abstraktionsnivåer\|abstraktionsnivå]], dvs inte på gate-nivå (till skillnad från [[Simple Signal Assignment\|Simple Signal Assignment]]). abc används som ett [[Switch Case\|Switch Case]].