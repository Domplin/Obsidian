**Resonance** is a condition in an [[Series RLC Circuit]] in which the capacitive and inductive reactance’s are equal in magnitude, thereby resulting in purely resistive impedance


Resonant circuits (*series or parallel*) are useful for constructing filters as their transfer functions can be highly frequency selective.

Consider the series [[Series RLC Circuit]] shown in the frequency domain:
![[Pasted image 20240407213441.png]]

$$
Z = H(\omega)=\frac{V_{s}}{I}=R+j\omega L+\frac{1}{j\omega C}
$$
or
$$
Z=R+j\left( \omega L-\frac{1}{\omega C} \right)
$$
**Resonance** results when the imaginary part of the transfer function is zero or:
$$
Im(Z)=\omega L-\frac{1}{\omega C} =0
$$
The value of $\omega$ that satisfies this condition is called the *resonance frequency* $\omega_{0}$. Thus the resonance condition is
$$
\omega_{0}L=\frac{1}{\omega_{0} C}
$$
or
$$
\omega_{0}=\frac{1}{\sqrt{ LC }}\text{rad/s}
$$
since $\omega_{0}=2\pi f_{0}$ 
$$
f_{0}=\frac{1}{2\pi \sqrt{ LC }}\text{Hz}
$$
**Important**: [[Note About Resonance|Note About Resonance]]

The [[Frequency Response]] of the circuit’s current magnitude:
$$
I=|I| = \frac{V_{m}}{\sqrt{ R^2+\left( \omega L-\frac{1}{\omega C} \right)^2 }}
$$

The symmetry illustrated in this graph when the frequency axis is a logarithm with the average power dissipated by the [[Series RLC Circuit]] is:
![[Pasted image 20240407214439.png]]

$$
P(\omega) = \frac{1}{2} I^2R
$$

The highest power dissipated occurs at resonance, when $I=\frac{V_{m}}{R}$ so that:
$$
P(\omega_{0}) =\frac{1}{2} \frac{V_{m}^2}{R}
$$
At certain frequencies $\omega = \omega_{1}, \omega_{2}$ the dissipated power is half the maximum value that is:
$$
P(\omega_{1})=P(\omega_{2})=\frac{(V_{m}\sqrt{ 2 })^2}{2R}=\frac{V_{m}^2}{4R}
$$
Which is why they are called *[[Half-Power Frequencies]]* 
