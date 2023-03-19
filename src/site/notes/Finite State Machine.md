---
{"dg-publish":true,"permalink":"/finite-state-machine/","tags":["digitalteknik"]}
---

A finite state machine is a machine that can be in exactly one out of a finite number of states.

I [[VHDL\|VHDL]] behövs:
1. List of all possible states
2. List that describes how and when we should change states
3. Specify initial state
Often visualized in a [[Tillståndsgraf\|State Diagram]]

I [[VHDL\|VHDL]] kan vi definiera en [[Process in VHDL\|process]]för den kombinatoriska delen och en för minnesdelen.

Man behöver inte använda någon sorts [[State Assignment\|Tillståndskodning]] i [[VHDL\|VHDL]], utan man låter syntes-verktyget göra det åt en. Deklarera istället en ny data-typ. Exemepelvis
```vhdl
architecrue a_my_fsm of my_fsm is
	type state is (start, pause, stop); 
	signal current_state : state;
begin
...
	if current_state = start then
		...
```
där state är namnet på data-typen, och start, pause och stop är möjliga värden. Kretsen optimeras av programmet!

## Se också:
[[Mealy-maskin\|Mealy-maskin]]
[[Moore-maskin\|Moore-maskin]]