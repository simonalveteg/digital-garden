---
{"dg-publish":true,"permalink":"/controllability/","tags":["reglerteknik"]}
---

We can't always place the poles arbitrarily. This happens if one of our [[Tillståndsvariabler\|state variables]] can't be affected by the control signal $u$. In other words:

> A state [[Vektorer\|vector]] $x_{0}$ is said to be *controllable* if there exists a control signal which brings $x$ from the origin to $x_{0}$ in a finite time. A [[System (matematisk definition)\|System (matematisk definition)]] is controllable if all its states are controllable.

If a [[System (matematisk definition)\|System (matematisk definition)]] is controllable it is possible to place its poles arbitrarily using [[State Feedback\|state feedback]]. 

Wether a [[System (matematisk definition)\|System (matematisk definition)]] is controllable can be determined by studying the [[Controllability Matrix\|Controllability Matrix]]