---
{"dg-publish":true,"permalink":"/syntax-of-a-process-in-vhdl/","tags":["digitalteknik"]}
---

```vhdl
process(a,b) -- sensitivity list - which signals triggers the process
begin
	z <= a or b;
	z <= a nor b;
	z <= a and b;
end process;
```
