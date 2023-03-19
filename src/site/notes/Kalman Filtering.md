---
{"dg-publish":true,"permalink":"/kalman-filtering/","tags":["reglerteknik"]}
---

The kalman filter is a method to obtain an estimate of the [[State Vector\|state vector]] from the control and measurement signals. If the [[System (matematisk definition)\|System (matematisk definition)]] is [[Observability\|observable]] it is possible to estimate the [[State Vector\|state vector]] by studying the input $u$ and the output $y$ by filtering them through a Kalman filter. 

The kalman filter makes use of both the control signal and the measurement signals in order to estimate the [[State Vector\|state vector]] in the following way:
$$\begin{flalign}&\dot{\hat{x}}=A \hat{x}+Bu+L(y-\hat{y}) \\&\hat{y}=C\hat{x} \end{flalign}$$
The estimation error 
$$\dot{\tilde{x}}=\dot{x}-\dot{\hat{x}}=Ax+Bu-A \tilde{x}-Bu-LC(x-\hat{x})=(A-LC)\tilde{x}$$
where $L$ is a column [[Vektorer\|vector]], which we want to choose so that the eigenvalues for $(A-LC)$  are placed appropriately. The choice is a compromise between speed and sensitivity towards disturbances and modelling errors. The speed is how quickly the kalman filter finds the correct [[State Vector\|state vector]] typ. 

dvs använd [[Karakteristiska polynomet för matriser\|karakteristiska polynomet]] för att få fram [[Egenvärden\|egenvärden]] som beror på $\vec{L}$, jämför med önskade [[Egenvärden\|egenvärden]] och använd identifiering för att ta reda på vad $L$ ska vara.

> We generally want the kalman filter to be fast in relation to the [[Output Feedback\|output feedback]]. #question why? något med att balansera en pinne

[[example of kalman filter estimating the state vector.png]]