Consider the series RLC circuit shown
![[Pasted image 20240502184408.png]]

The circuit is being excited by the energy initially stored in the capacitor and inductor.
The energy is represented by the initial capacitor voltage $V_{0}$ and initial inductor current $I_{0}$ 
At $t=0$
$$
v(0)=\frac{1}{C}\int ^0_{-\infty}idt \,=V_{0} 

$$
$$
i(0)=I_{0}
$$
Applying KVL around the loop:
$$
Ri+L \frac{di}{dt}+\frac{1}{C}\int ^t_{-\infty}i(\tau) \, d\tau=0
$$
To eliminate the integral, we differentiate with respect to $t$ and rear-range terms we get:
$$
\frac{d^2i}{dt^2}+\frac{R}{L} \frac{di}{dt}+\frac{i}{LC}=0
$$
This is a *second-order differential equation* and is the reason for calling the RLC circuits second-order circuits

To solve the second-order equation requires that we have two initial conditions such as the initial value of $i$ and its first derivative or initial values of some $i$ and $v$ 

The initial value of $i$ is given from the initial $i(0)$ equation above.

Using the above equations we obtain:
$$
Ri(0)+L \frac{di(0)}{dt}+V_{0}=0
$$
or
$$
\frac{di(0)}{dt}=-\frac{1}{L}(RI_{0}+V_{0})
$$
From the previous chapter we let 
$$
i=Ae^{st}
$$
Where $A$ and $s$ are constants to be determined. Substituting this and carrying out the needed differentiations we obtain
$$
As^2e^{st}+\frac{AR}{L}se^{st}+\frac{A}{LC}e^{st}=0
$$
or
$$
Ae^{st}\left( s^2+\frac{R}{L}s+\frac{1}{LC} \right)=0
$$
Since $i=Ae^{st}$ is the assumed solution we are trying to find only the expression in parentheses can be zero:
$$
s^2+\frac{R}{L}s+\frac{1}{LC} =0
$$
This quadratic equation is known as the *[[characteristic equation]]* 