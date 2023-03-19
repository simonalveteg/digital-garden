---
{"dg-publish":true,"permalink":"/linjaer-regression/","tags":["matematiskstatistik"]}
---

Linear regression has two main objectives. The first is to **establish if there is a relationship** between two variables - more specifically, if there is a statistically significant relationship between them. The second is to **forecast new observations**. Can we use what we know about the relationship to forecast unobserved values?

The dependent variable is a variable whose values we want to explain or forecast. It depends on something else and is denoted $y_i$. The independent variable explains the other variable, and is denoted $x_i$. 

$$
y_i=\alpha+\beta x_i+\varepsilon_i
$$
where $\varepsilon \in N(0,\sigma)$ ([[Normalfördelning\|Normalfördelning]]) is the error.