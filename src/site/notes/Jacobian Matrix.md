---
{"dg-publish":true,"permalink":"/jacobian-matrix/","tags":["reglerteknik"]}
---

Using the partial derivatives we can get the matrices needed to write the system on [[Linear state-space model\|state-space form]].

$$\begin{pmatrix}\frac{\partial f_{1}}{dx_{1}} & \frac{\partial f_{1}}{dx_{2}} & \frac{\partial f_{1}}{dx_{3}} \\ \frac{\partial f_{2}}{dx_{1}} & \frac{\partial f_{2}}{dx_{2}} & \frac{\partial f_{2}}{dx_{3}} \\ \frac{\partial f_{3}}{dx_{1}} & \frac{\partial f_{3}}{dx_{2}} & \frac{\partial f_{3}}{dx_{3}}\end{pmatrix}=\begin{pmatrix}A & A & B \\ A & A & B \\ C & C & D\end{pmatrix}$$
