A filter that prevents a band of frequencies between two designated values ($\omega_{1}$ and $\omega_{2}$) from passing is variably known as a **band-stop**, **band-reject**, or **notch** filter. A band-stop filter is formed when the output RLC [[Series Resonance]] circuit taken off the LC series combination.

The transfer function is:
$$
H(\omega)=\frac{V_{o}}{V_{i}}=\frac{j\left( \omega L-\frac{1}{\omega C} \right)}{R+j\left( \omega L-\frac{1}{\omega C} \right)}
$$
![[Pasted image 20240408003904.png]]

Notice that $H(0)=1$, $H(\infty)=1$. The graph shows the plot of $|H(\omega)|$. Again the center frequency is given by
$$
\omega_{0}=\sqrt{ LC }
$$
![[Pasted image 20240408004032.png]]

while the [[Half-Power Frequencies]], the bandwidth, and the [[Quality Factor]] are calculated using the formulas from 14.5 for a series resonant circuit.

Here $\omega_{0}$ is called the *frequency of rejection*, while the corresponding bandwidth ($B=\omega_{2}-\omega_{1}$) is known as the *bandwidth of rejection*


A **band-stop filter** is designed to stop of eliminate all frequencies within a band of frequencies $\omega_{1}<\omega<\omega_{2}$



[[passive filter conclusion]]




