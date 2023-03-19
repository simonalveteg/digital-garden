---
{"dg-publish":true,"permalink":"/reconstruction/","tags":["digitalsignalbehandling"]}
---

A digital circuit that interacts with the real world needs to convert the continuous-time signals to [[Discrete-time signals\|discrete-time signals]] ([[Sampling\|sampling]]) and then back again (reconstruction). 

$$t=nT_{s} \Leftrightarrow n=tF_{s}$$

When [[Sampling\|sampling]] you replace $t$ with $nT_{s}$, but with reconstruction you instead replace $n$ with $tF_{s}$ (makes sense because $T=\frac{1}{F}$). $F_{s}$ will then be combined with the $f$ to form $F$, since $F=fF_{s}$

$t$ is the normal time variable, $n$ is the discrete time variable (number of samples), $T$ is the time period between samples and $F$ is the continuous time frequency.