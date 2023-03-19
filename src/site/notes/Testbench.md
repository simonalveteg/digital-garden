---
{"dg-publish":true,"permalink":"/testbench/","tags":["digitalteknik"]}
---

## Testbench
En testbench används endast för att testa när man simulerar. 

### Basic Structure of Testbench
```vhdl
library IEEE;
use IEEE.STD_LOGIC_1164.all;

entity adder_1bit_tb is
end entity adder_1bit_tb;
		
architecture a_adder_1bit_tb of adder_1bit_tb is
component adder_1bit is
	port(c_i : in STD_LOGIC;
		a : in STD_LOGIC;
		b : in STD_LOGIC;
		z : out STD_LOGIC;
		c_o : out STD_LOGIC);
end component adder_1bit;
signal a_tb, b_tb, z_tb, c_in_tb, c_out_tb : STD_LOGIC;
begin
	port map(c_i => c_in_tb,
			a => a_tb,
			b => b_tb,
			z => z_tb,
			c_o => c_out_tb);
process -- no sensitivity list => always evaluated
begin
	a_tb <= '0';
	b_tb <= '0';
	c_in_tb <= '0';
	wait for 10 ns;
	a_tb <= '1';
	wait for 10 ns;
	a_tb <= '0';
	b_tb <= '1';
	wait for 10 ns;
	wait; -- wait here => simulation is done
end process;
end architecture a_adder_1bit_tb;
```
