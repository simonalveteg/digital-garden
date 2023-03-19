---
{"dg-publish":true,"permalink":"/linear-state-space-model-to-transfer-function/","tags":["reglerteknik"]}
---

We have a [[Linear state-space model\|linear state-space model]] of our process
$$\begin{cases}\dot{x}=Ax+Bu \\y=Cx+Du \end{cases}$$
which gives the laplace transform
$$\begin{cases} sX = AX + BU \\ Y = CX+DU \end{cases}$$
. If we solve this set of equations for $Y$ we get 
$$sX-AX=BU \Rightarrow (sI-A)X=BU \rightarrow X = (sI-A)^{-1}BU$$
$$\Rightarrow Y = (C(sI-A)^{-1}B+D)U$$
which is our [[Överföringsfunktion\|transfer function]] ($Y/U$)
