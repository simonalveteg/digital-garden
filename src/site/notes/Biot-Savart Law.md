---
{"dg-publish":true,"permalink":"/biot-savart-law/","tags":["elektromagnetiskfältteori"]}
---

Allows us to determine the [[Magnetic Field\|magnetic field]] at a point in space, and is one of the most generally true laws.
$$
\vec{B}=\frac{\mu_{0}}{4\pi}\int\frac{ Id\vec{l}\times \hat{r}}{r^2}
$$
where $\mu_{0}$ is the [[Permeabilitet\|magnetic permeability]] in free space, $I$ is the current (which can typically be taken out of the integral), $\hat{r}$ is the [[Enhetsvektor\|unit vector]] of $r$, which is the distance from $d\vec{l}$ to the point.
![image-biot-savart.png](/img/user/images/image-biot-savart.png)
The direction can be found easily using the [[Right Hand Rule\|right hand rule]], which means that we can use a **simpler version** of the biot-savart law that only gives us the magnitude.
$$
\left| \vec{B} \right| =\frac{\mu_{0}I}{4\pi} \int \frac{\left| d\vec{l}\times\hat{r} \right| }{r^{2}}=\frac{\mu_{0}I}{4\pi}\int \frac{dl\sin\theta}{r^2}
$$
 
