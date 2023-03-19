---
{"dg-publish":true,"permalink":"/simple-signal-assignment/","tags":["digitalteknik"]}
---

ex:
![Pasted image 20211108104739.png](/img/user/images/Pasted%20image%2020211108104739.png)
```vhdl
library IEEE;
use IEEE.STD_LOGIC_1164.all;

entity comb1 is 
	port(a, b, c : in STD_LOGIC;
		q : out STD_LOGIC);
end entity comb1;
	
architecture a_comb1 of comb1 is
	signal d : STD_LOGIC;
begin
	d <= b and c;
	q <= (not a) or d;
end architecture a_comb1
```

Ordningen spelar ingen roll, så man kan skriva q före d. Man kan också skita i att skriva d och bara skriva allt på en rad
```vhdl
 q <= (not a) or (b and c)
```