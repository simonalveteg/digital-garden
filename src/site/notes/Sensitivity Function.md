---
{"dg-publish":true,"permalink":"/sensitivity-function/","tags":["reglerteknik"]}
---


The sensitivity function is a [[Överföringsfunktion\|transfer function]]. It describes how disturbances are affected by the [[feedback\|feedback]]. Disturbances with frequency $\omega$ for which $|S(i \omega)| <1$ are rejected while  $|S(i \omega)| >1$ are amplified by the [[feedback\|feedback]].

The highest value of the sensitivity function (nominal sensitivity peak) corresponds to the inverse of the shortest distance between the [[Nyquist plot\|nyquist curve]] and the point -1. Explained in the first four minutes of [Understanding The Sensitivity Function](https://www.youtube.com/watch?v=BAWdZvF1O40)

The sensitivity function $S(s)$ for a simple [[Feedback System\|feedback system]] with [[Open-Loop Transfer Function\|open-loop transfer function]] $G_{0}=G_{R}G_{P}$ is given by $$S=\frac{1}{1+G_{P}G_{R}}$$
where $G_R$ is the [[Control System\|controller]] [[Överföringsfunktion\|transfer function]] and $G_{P}$ is the [[Process Models\|process]] [[Överföringsfunktion\|transfer function]].

> Understanding it explains how [[feedback\|feedback]] changes the open loop into the closed loop. #question how?
 

A general rule of thumb is to make the sensitivity function small for low frequencies. It is good when the disturbances have low frequencies. But we only want $S(i \omega)$ to be small for frequencies where the noise is small. 

To make $S$ small we need to make $P(s)C(s)$ big (if we are talking about a classic [[Feedback System\|Feedback System]])


$$Y(s)=\frac{P(s)C(s)}{1+P(s)C(s)}R(s)+\frac{P(s)}{1+P(s)C(s)}D(s)\frac{-P(s)C(s)}{1+P(s)C(s)}N(s)$$
The expression in front of $R(s)$ är [[The complementary sensitivity function\|The complementary sensitivity function]]

