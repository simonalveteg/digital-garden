---
{"dg-publish":true,"permalink":"/laplacetransformation-av-tempererade-funktioner/","tags":["systemochtransformer"]}
---


[[Distributioner\|distribution]]
$$\mathcal{L}(\mathcal{U})(s)=\int_{-\infty}^{\infty}\mathcal{U}(t)e^{-st}dt=<\mathcal{U},e^{-st}>$$
[[Delta Funktionen\|deltafunktionen]]
$$\mathcal{L}(\delta(t))(s)=\int_{-\infty}^{\infty}\delta(t)e^{-st}dt=\int_{-\infty}^{\infty}e^0\delta(t)dt=1$$
dvs $\delta(t)\xrightarrow{\mathcal{L}}1$ för alla s.

$$\mathcal{L}(\delta_{a}(t))(s)=\mathcal{L}(\delta(t-a))(s)\stackrel{26/27}{=}e^{-as}\mathcal{L}(\delta(t))(s)$$
$$\mathcal{L}(\delta'(t))(s) \stackrel{28-29}{=} s \mathcal{L}(\delta(t))(s)=s$$
$$\mathcal{L}(\delta^{(n)}(t))(s)=s^{n}\mathcal{L}(\delta(t))(s)=s^{n}$$