As we learned in the previous chapter the step response is obtained by the sudden application of a DC source

Consider the [[Series RLC Circuit|series RLC circuit]] shown below
![[Pasted image 20240502210937.png]]

Applying KVL around the loop for $t>0$ 
$$
L \frac{di}{dt}+Ri+v=V_{s}
$$
But
$$
i=c \frac{dv}{dt}
$$
Substituting an rearranging terms
$$
\frac{d^2v}{dt^2}+\frac{R}{L} \frac{dv}{dt}+\frac{v}{LC}=\frac{V_{s}}{LC}
$$
The [[characteristic equation]] is not affected by the presence of the DC source

The solution to the equation has two components:
- the [[Old/ECE 202/Chapter 8 - Second Order Circuits/8.5 Step response of a Series RLC Circuit/Transient Response]] $v_{t}(t)$ 
- [[Steady-State Response]] $v_{ss}(t)$ 
$$
v(t)=v_{t}(t)+v_{ss}(t)
$$
Therefore the [[Old/ECE 202/Chapter 8 - Second Order Circuits/8.5 Step response of a Series RLC Circuit/Transient Response]] $v_{t}(t)$ for the [[Series RLC Overdamped]], [[Series RLC Critically Damped]], and [[Series RLC Underdamped Case]]


Thus the complete solutions for the overdamped, underdamped, and critically damped cases are:
$$
\begin{align}
v(t)=V_{s}+A_{1}e^{s_{1}t}+A_{2}e^{s_{2}t} \\
v(t)=V_{s}+(A_{1}+A_{2}t)e^{-\alpha t} \\
v(t)=V_{s}+(A_{1}\cos(\omega_{d}t)+A_{2}\sin \omega_{d}t)e^{-\alpha t}
\end{align}
$$
The values of constants $A_{1}$ and $A_{2}$ are obtained from the initial conditions $v(0)$ and $\frac{dv(0)}{dt}$ 

Keep in mind that $v$ and $i$ are, respectively, the voltage across the capacitor and the current through the inductor.

Once the capacitor voltage $v_{c}=v$ is known we can determine $i=C \frac{dv}{dt}$, which is the same current through the capacitor, inductor, and resistor.

Hence, the voltage across the resistor is $V_{R}=iR$, while the inductor voltage is $v_{L}=L \frac{di}{dt}$ 

Alternatively, the complete response for any variable $x(t)$ can be found directly, because is has the general form
$$
x(t)=x_{ss}(t)+x_{t}(t)
$$
Where $x_{ss}=x(\infty)$ is the final value and $x_{t}(t)$ is the transient response

