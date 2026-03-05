The **step response** of a circuit is its behavior when the excitation is the step function, which may be voltage or current source. 

	$v(0^-)=v(0^+)=V_{0}$
![[Figure 7.40.png]]

Where:
- $v(0^-)$ is the voltage across the capacitor just before switching and $v(0)^+$ is its voltage immediately after switching.

$$
C \frac{dv}{dt}+\frac{v-v_{s}u(t)}{R}=0
$$
or
$$
\frac{dv}{dt}+\frac{v}{RC}=\frac{V_{s}}{RC}
$$

After rearranging and integrating the two equations we get are:
$v(t)=V_{0}:    t<0$
$V_{s}+(V_{0}-V_{s})e^{-t/\tau}:t>0$ 

This is known as the [[RC Complete Response]]