---
{"dg-publish":true,"permalink":"/example-pendulum-swinging/","tags":["reglerteknik"]}
---



![Pasted image 20220830152824.png](/img/user/images/Pasted%20image%2020220830152824.png)
$$u-mgsin(\theta)=0$$
$u$ is the [[Torque\|torque]] we apply to the rod. An equlibrium point we can [[Linearization\|linearise]] around could be $u_{0}=0$, $\theta_{0}=0$. We need to introduce new variables that should describe the deviation in our original variables relative to the equlibrium point.
$\Delta \theta=\theta-\theta_{0}$ and $\Delta u = u-u_{0}$
we then substitute these into the original [[Differentialekvationer\|differential equations]] and use the taylor series.
$$\Delta u+u_{0}-mgsin(\Delta \theta+\theta_{0})=m \Delta \ddot{\theta} $$
![Pasted image 20220830161758.png](/img/user/images/Pasted%20image%2020220830161758.png)