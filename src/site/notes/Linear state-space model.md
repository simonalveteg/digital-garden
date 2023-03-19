---
{"dg-publish":true,"permalink":"/linear-state-space-model/","tags":["reglerteknik"]}
---

a structured set of [[Differentialekvationer\|differential equations]]
$$\begin{cases}\dot{x}=Ax+Bu\\y=Cx+Du \end{cases}$$
where $\dot{x}$ is a [[Tillståndsvariabler\|state variable]]. x is a [[Vektorer\|vector]] variable. A is nxn [[Matris\|matrix]], B is nx1, C is 1xn and D is 1x1. If we have more things to measure we make C taller. The first equation is the *state equation* and the second is the *output equation*.

[[Transfer Function vs Linear State-Space Model\|Transfer Function vs Linear State-Space Model]]

The [[Differentialekvationer\|differential equation]] can be written in state space form, if we introduce n states $x_{1},x_{2},x_{3}...x_{n}$ the equation can be written as a [[System (matematisk definition)\|System (matematisk definition)]] of first order [[Differentialekvationer\|differential equations]]

If we have higher order derivatives we need to introduce new variables to capture the value since the model only works with a first order derivative of x?