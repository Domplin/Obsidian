The RLC series resonant circuit provides a **band-pass filter** when the output is taken of the resistor. The [[Transfer Function|transfer function]] is:
$$
H(\omega)=\frac{V_{o}}{V_{i}}=\frac{R}{R+j\left( \omega L-\frac{1}{\omega C} \right)}
$$
![[Pasted image 20240408002716.png]]
we observe that $H(0)=0$, $H(\infty)=0$ shows the plot of $|H(\omega)|$
The band-pass filter passes a band of frequencies $\omega_{1}<\omega<\omega_{2}$ centered at $\omega_{0}$ the center frequency is given by:
$$
\omega_{0}=\frac{1}{\sqrt{ LC }}
$$
![[Pasted image 20240408002940.png]]

A **band-pass filter** is designed to pass all frequencies within a band of frequencies, $\omega_{1}<\omega<\omega_{2}$. Because the band-pass filter shown was a [[Series Resonance]] circuit, the [[Half-Power Frequencies]], the bandwidth, and the [[Quality Factor]] are determined as in 14.5.

A band-pass filter can also be formed by cascading the [[low-pass filter]](where $\omega_{2}=\omega_{c}$). However, the result would not be the same as just adding the output of the [[low-pass filter]] to the input of the [[high-pass filter]], because one circuit loads the other and alters the desired transfer function.


[[passive filter conclusion]]