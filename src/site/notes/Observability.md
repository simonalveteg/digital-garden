---
{"dg-publish":true,"permalink":"/observability/","tags":["reglerteknik"]}
---

Normally all process states are not directly measurable. It is only possible to estimate the [[State Vector\|state vector]] merely by studying the control signal $u$ and the output signal $y$ if the [[System (matematisk definition)\|System (matematisk definition)]] is **observable**.

> A [[State Vector\|state vector]] $x_{0} \neq 0$ is not observable if the output is $y(t)=0$ when the initial [[State Vector\|state vector]] is $x(0)=x_{0}$ and the input is given by $u(t)=0$. A [[System (matematisk definition)\|System (matematisk definition)]] is observable if it lacks non-observable states.

Whether a [[System (matematisk definition)\|System (matematisk definition)]] is observable can be determined by studying the [[Observability Matrix\|Observability Matrix]].