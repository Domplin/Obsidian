A typical low-pass filter is formed when the output of an RC circuit is taken off the capacitor. The [[Transfer Function|transfer function]]:
$$
H(\omega)=\frac{V_{o}}{V_{i}}=\frac{\frac{1}{j\omega C}}{R+ \frac{1}{j\omega C}}
$$
$$
H(\omega)=\frac{1}{1+j\omega RC}
$$
![[Pasted image 20240408001311.png]]

Note that $H(0)=1$, $H(\infty)=0$. The figure shows the plot of $|H(\omega)|$, along with the ideal characteristic, the [[Half-Power Frequencies]], which is equivalent to the corner frequency on the [[Bode Plots]] but in the context of filters is usually known as the *[[cutoff frequency]]* $\omega_{c}$ which is obtained by setting the magnitude of $H(\omega)$ equal to $\frac{1}{\sqrt{ 2 }}$:
$$
H(\omega_{c}) = \frac{1}{\sqrt{ 1+\omega_{c}^2R^2 C^2}}=\frac{1}{\sqrt{ 2 }}
$$
or
$$
\omega_{c}=\frac{1}{RC}
$$
The [[cutoff frequency]] is also called the *rolloff frequency* 

A **low-pass filter** is designed to pass only frequencies from DC and up to the cutoff frequency $\omega_{c}$

A low-pass filter can also be formed when the output of and RL circuit is taken off the resistor. Of course, there are many other circuits for low-pass filters.

[[passive filter conclusion]]