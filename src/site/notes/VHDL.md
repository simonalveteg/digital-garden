---
{"dg-publish":true,"permalink":"/vhdl/","tags":["digitalteknik"]}
---

## Vad är VHDL?
Very high speed integrated circuit
Hardware
Description
Language

I VHDL skriver man en beskrivning av hur [[Signal\|signaler]] ska genereras. Man väljer portar som in och utsignaler, och sen definierar man utsignalerna med [[Signal Assignment\|Signal Assignment]]. Om koden inte ger ett output för alla inputs, så kommer syntes-verktyget anta att det ska vara samma output som föregående, och lägga till en latch.

## Syntax

### Signaler
för att skapa en intern [[Signal\|Signal]] använder man
```vhdl
signal c1 : STD_LOGIC;
```
in och ut-[[Signal\|signaler]] definieras i port
```vhdl
port(a : in STD_LOGIC_VECTOR(3 downto 0);
	b : in STD_LOGIC_VECTOR(3 downto 0);
	z : out STD_LOGIC_VECTOR(3 downto 0));
```

### <= och =>


### Downto och to
(3 downto 0) betyder att vi får fyra bits, och att bitten längst till vänster är 3, och den går ned till 0 när man går till höger. Ordningen blir samma som när man skriver binärt på papper, dvs den mest signifikanta biten till vänster. (0 to 3) är motsatsen.


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/syntax-of-a-process-in-vhdl/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




```vhdl
process(a,b) -- sensitivity list - which signals triggers the process
begin
	z <= a or b;
	z <= a nor b;
	z <= a and b;
end process;
```


</div></div>


### Assert Command
```vhdl
...
assert z_tb = '0' report "Assertion violation." severity error;
```
Throws an error if $z_{tb}$ is not $0$.


## Structural Description
A schematic at block level, describing text. Describe which components should be in the block diagram, and how they should be connected with each other. 

Att definiera component är typ samma sak som när man definierar en entity innan architecture, som visas i [[Signal Assignment\|Signal Assignment]]
![Pasted image 20211108112318.png](/img/user/images/Pasted%20image%2020211108112318.png)

Fördelen med structural design är att man kan beskriva större [[System (matematisk definition)\|System (matematisk definition)]] med många mindre [[System (matematisk definition)\|System (matematisk definition)]], och kanske även återanvända komponenter.


### Alternativ
Verilog
På högre [[Abstraktionsnivåer\|abstraktionsnivå]]:
SystemC
Catapult C
Matlab

## Se också
[[Signal Assignment\|Signal Assignment]]
[[Signal Buses\|Signal Buses]]
[[Process in VHDL\|Process in VHDL]]
[[Finite State Machine\|Finite State Machine]]
[[Testbench\|Testbench]]
