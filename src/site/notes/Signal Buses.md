---
{"dg-publish":true,"permalink":"/signal-buses/","tags":["digitalteknik"]}
---


![Pasted image 20211108110220.png](/img/user/images/Pasted%20image%2020211108110220.png)
[[Signal Bus Assignment\|Signal Bus Assignment]]

### Ways to assign value
1. Set all bits to a value
```vhdl 
z <= (others => '1');
```
2. Set specific bits to a value
```vhdl 
z(0) <= '0';
z(1) <= '0';
z(2) <= '1';
z(3) <= '0';
```
3. Or do it on a single line
```vhdl 
z <= (1|3 => '1', 0|2 => '0'); -- 1010
```
4. Or like this
```vhdl 
z <= (1|3 => '1', others => '0'); -- 1010
```
5. 
![Pasted image 20211108111228.png](/img/user/images/Pasted%20image%2020211108111228.png)

[[Aggregating Vectors\|Aggregating Vectors]]