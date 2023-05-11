---
{"dg-publish":true,"permalink":"/laboration-datorteknik-4/","tags":["laboration","datorteknik"]}
---



This lab is about Interrupt Handling. The goal is to understand how to use interrupts and learn how to write interrupt service routines. 

We need to write a state machine

first we can do polling, then it's a security systems run - function from library does stuff in the background to simulate other processes going on. The whole point is to see the difference between polling and interrupts. 

Write the code with polling, and avoid while loops. Keep some kind of state variable. Use a switch case. Then we replace it with interrupts. We can put the whole code in a interrupt routine, which is not the best solution but it works. The longer our interrupt routine is the higher the chance that we miss another input. Better solution: simply change the state of a variable in the interrupt and let the main program read those variables. 

[[Interrupt Handling\|Interrupt Handling]]
