Consider the parallel RLC circuit shown. We want to find $i$ due to a sudden application of a DC circuit
![[Pasted image 20240502213041.png]]

Applying KCL at the top node for $t>0$
$$
\frac{v}{R}+i+c \frac{dv}{dt}=I_{s}
$$
But
$$
v=L \frac{di}{dt}
$$
Substituting for $v$ and dividing $LC$ we get
$$
\frac{d^2i}{dt^2}+\frac{1}{RC} \frac{di}{dt}+\frac{i}{LC}=\frac{I_{s}}{LC}
$$
The complete solution consists of the [[Previous/ECE 202/Chapter 7 - First-Order Circuits/Transient Response|Transient Response]] $i_{t}(t)$ and the [[Steady-State Response]] $i_{ss}$:
$$
i(t)=i_{t}(t)+i_{ss}(t)
$$
The steady-state response is the final value of $i$. the final value of the current through the inductor is the same as the source current $I_{s}$:
$$
i(t)=I_{s}+A_{1}e^{s_{1}t}+A_{2}e^{s_{2}t}
$$
$$
i(t)=I_{s}+(A_{1}+A_{2}t)e^{-\alpha t}
$$
$$
i(t)=I_{s}+(A_{1}\cos \omega_{d}t+A_{2}\sin \omega_{d}t)e^{-\alpha t}
$$
The constants $A_{1}$ and $A_{2}$ in each case can be determined from the initial conditions for $i$ and $\frac{di}{dt}$. The equations only apply for finding the inductor current $i$. But once the inductor current $i_{L}-i$ is known, we can find $v=L \frac{di}{dt}$ which is the same voltage across inductor, capacitor, and resistor. Hence, the current through the resistor is $i_{R}=\frac{v}{R}$ while the capacitor current is $i_{c}=C \frac{dv}{dt}$ 

Alternatively, the complete response for any variable $x(t)$ may be found directly using
$$
x(t)=x_{ss}(t)+x_{t}(t)
$$
where $x_{ss}$ and $x_{t}$ are its final value and transient response