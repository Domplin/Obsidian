A **band-reject filter** may be constructed by parallel combination of a [[low-pass filter]], [[high-pass filter]] and a summing amplifier, shown in the block diagram.

![[Pasted image 20240408012629.png]]

The circuit is designed such that the lower [[cutoff frequency]] $\omega_{1}$ is set by the [[low-pass filter]] while the upper cutoff frequency $\omega_{2}$ is set by the [[high-pass filter]]. the gap between $\omega_{1}$ and $\omega_{2}$ is the bandwidth of the filter. As shown in the figure (b), the filter passes frequencies below $\omega_{1}$ and above $\omega_{2}$.

The [[Transfer Function|transfer function]] is:
$$
H(\omega)=\frac{V_{o}}{V_{i}}=-\frac{R_{f}}{R_{i}}\left( -\frac{1}{1+j\omega C_{1}R}-\frac{j\omega C_{2}R}{1+j\omega C_{2}R} \right)
$$

![[Pasted image 20240408013036.png]]
The figure shows how an active band-reject filter would be constructed.

The formulas for calculating the values of $\omega_{1}$, $\omega_{2}$, the center frequency, bandwidth, and [[Quality Factor]] are
$$
\begin{align}
\omega_{2}=\frac{1}{RC_{1}} \\
\omega_{1}=\frac{1}{RC_{2}}
\end{align}
$$

To determine the passband gain $K$ of the filter, we can write the equation in terms of the upper and lower corner frequencies as:
$$
H(\omega)=\frac{R_{f}}{R_{i}} \left( \frac{1}{1+\frac{j\omega}{\omega_{2}}}+\frac{\frac{j\omega}{\omega_{1}}}{1+\frac{j\omega}{\omega_{1}}} \right)=\frac{R_{f}}{R_{i}} \frac{\left( 1+\frac{j2\omega}{\omega_{2}} + \frac{(j\omega)^2}{\omega_{1}\omega_{1}} \right)}{\left( 1+\frac{j\omega}{\omega_{2}} \right)\left( 1+\frac{j\omega}{\omega_{1}} \right)}
$$

Comparing this which the standard form indicates that the two passbands ($\omega \rightarrow 0 \text{ and } \omega \rightarrow\infty$) the gain is:
$$
K=\frac{R_{f}}{R_{i}}
$$
The gain at the center frequency can also be found by finding the magnitude of the transfer function at $\omega_{0}=\sqrt{ \omega_{1}\omega_{2} }$:
$$
H(\omega_{0})=|\frac{R_{f}}{R_{i}} \frac{\left( 1+\frac{j2\omega}{\omega_{2}} + \frac{(j\omega)^2}{\omega_{1}\omega_{1}} \right)}{\left( 1+\frac{j\omega}{\omega_{2}} \right)\left( 1+\frac{j\omega}{\omega_{1}} \right)}| =\frac{R_{f}}{R_{i}} \frac{2\omega_{1}}{\omega_{1}+\omega_{2}}
$$
