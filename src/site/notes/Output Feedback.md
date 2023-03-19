---
{"dg-publish":true,"permalink":"/output-feedback/","tags":["reglerteknik"]}
---

![output feedback.png](/img/user/images/output%20feedback.png)
A [[System (matematisk definition)\|System (matematisk definition)]] with output [[feedback\|feedback]] uses the estimated states instead of the actual states to close the [[Feedback System\|feedback loop]]. The equations that describe the [[System (matematisk definition)\|System (matematisk definition)]] above are
$$\begin{cases} \dot{\hat{x}}=A \hat{x}+Bu+L(y-\hat{y}) \\
\hat{y}=C \hat{x}  \\
u=-K\hat{x}+r_{k}k_{r} \end{cases}$$
to investigate the closed-loop system in state space we can choose the state vecor as $x_{e}=\begin{pmatrix}x \\ \tilde{x}\end{pmatrix}$, where $\tilde{x}=x-\hat{x}$. Our [[Linear state-space model\|state-space]] equations can now be written
$$\begin{flalign}&\dot{x}=Ax+Bu=Ax+Bk_{r}r-Bk \hat{x}=Ax+Bk_{r}r-BK(x-\tilde{x})=(A-BK)x+BK\tilde{x}+Bk_{r}r \\&\dot{\tilde{x}}=\dot{x}-\dot{\hat{x}}=Ax+Bu-A \hat{x}-Bu-LC(x-\hat{x})=(A-LC)\tilde{x} \\&y=Cx\end{flalign}$$
which on matrix form is
$$\begin{flalign}&\begin{pmatrix}\dot{x} \\ \dot{\tilde{x}}\end{pmatrix}=\begin{pmatrix}A-BK & BK \\ 0 & A-LC\end{pmatrix}\begin{pmatrix}x \\ \tilde{x}\end{pmatrix}+\begin{pmatrix}Bk_{r} \\ 0\end{pmatrix}r=A_{e}\begin{pmatrix}x \\ \tilde{x}\end{pmatrix}+B_{e}r \\&
y=\begin{pmatrix}C & 0\end{pmatrix}\begin{pmatrix}x \\ \tilde{x}\end{pmatrix}=C_{e}\begin{pmatrix}x \\ \tilde{x}\end{pmatrix}
\end{flalign}
$$
The $_{e}$ stands for expanded. Since we chose $x_{e}=\begin{pmatrix}x \\ \tilde{x}\end{pmatrix}$ earlier our matrices $A_{e}, B_{e}, C_{e}$ contain a number of zeros, which will make our lives easier. Since $A_{e}$ is a triangular matrix, it's [[Karaktäristiska Polynomet\|characteristic polynomial]] is given by 
$$det(sI-A_{e})=det(sI-(A-BK))\cdot det(sI-(A-LC))$$







