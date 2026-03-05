![[Pasted image 20240328165137.png]]

By Voltage division the transfer function is given by:
$$
H(\omega)=\frac{V_{o}}{V_{s}}=\frac{\frac{1}{j\omega C}}{R+{\frac{1}{j\omega C}}}=\frac{1}{1+j\omega RC}
$$

Comparing this with [[Operations of complex numbers]] (*using the reciprocal operation*) the magnitude and phase can be found:
$$
\begin{align}
H=\frac{1}{\sqrt{ 1+\left( \frac{\omega}{\omega_{o}} \right)^2 }} \\
\phi=-\tan^{-1}\left( \frac{\omega}{\omega_{o}} \right)
\end{align}
$$

where $\omega_{o}=\frac{1}{RC}$ to plot $H$ and $\phi$ for $0<\omega<\infty$ some critical points are needed then sketch.

At $\omega = 0$, $H=1$, and $\phi = 0$ 
At $\omega=\infty$, $H=0$, and $\phi = -90$ 
And $\omega = \omega_{o}$, $H=\frac{1}{\sqrt{ 2 }}$, and $\phi=-45$ 

The table shows the frequency response:
![[Table 14.1.png]]

The graphs show the the amplitude response and phase response:
![[Pasted image 20240328174444.png]] 
