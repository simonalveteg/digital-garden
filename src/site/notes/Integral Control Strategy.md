---
{"dg-publish":true,"permalink":"/integral-control-strategy/","tags":["reglerteknik"]}
---


$$u(t)=K_{i}\int_{0}^{t}e(\tau)d \tau$$
If we haven't driven our error signal to zero the area under the "error-graph" will build up until the [[Control System\|control system]] gets rid of it? #question 

If the error signal reaches zero we don't want the [[Control System\|control system]] to do anything, but the integral term still contains all the area under the error signal up to this point (integrator windup), which means that our [[Control System\|control system]] will still change the value

If the error is not zero, integral action increases/decreases the ouptut at a rate of $K_{i}$ % per second for every 1% of error.