---
{"dg-publish":true,"permalink":"/signal-bus-assignment/","tags":["digitalteknik"]}
---

```vhdl
library IEEE;
use IEEE.STD_LOGIC_1164.all;

entity my_circuit is
	port(a : in STD_LOGIC_VECTOR(3 downto 0);
		b : in STD_LOGIC_VECTOR(3 downto 0);
		z : out STD_LOGIC_VECTOR(3 downto 0));
end entity my_circuit;
	
architecture a_my_circuit of my_circuit is
begin
	z <= a and b; -- bitwise and-operator, dvs (0011) and (1010) = (0010)
end architecture a_my_circuit;
```




