$\alpha=\omega_{0}$, $C=\frac{4L}{R^2}$ and
$$
s_{1}=s_{2}=-\alpha=-\frac{R}{2L}
$$
For this case the [[characteristic equation]] yields
$$
i(t)=A_{1}e^{-at}+A_{2}e^{-at}=A_{3}e^{-at}
$$
Where $A_{3}=A_{1}+A_{2}$. This cannot be the solution because the two initial conditions cannot be satisfied with the single constant $A_{3}$.

What could then be wrong. Our assumption of an exponential solution is incorrect for the special case of critical damping. 
When $\alpha=\omega_{0}=\frac{R}{2L}$ the equation becomes:
$$
\frac{d^2i}{dt^2}+\frac{2\alpha di}{dt}+\alpha^2i=0
$$
or
$$
\frac{d}{dt}\left( \frac{di}{dt}+\alpha i \right)+\alpha\left( \frac{di}{dt}+\alpha i \right)=0
$$
If we let
$$
f=\frac{di}{dt}+\alpha i
$$
Than the equation becomes
$$
\frac{df}{dt}+\alpha f=0
$$
which is a first-order differential equation with solution $f=A_{1}e^{-\alpha t}$ where $A_{1}$ is a constant the equation then becomes:
$$
\frac{di}{dt}+\alpha i=A_{1}e^{-\alpha t}
$$
Integrating both sides yields:
$$
e^{\alpha t}i=A_{1}t+A_{2}
$$
or
$$
i=(A_{1}t+A_{2})e^{-\alpha t}
$$
![[Pasted image 20240502193217.png]]
