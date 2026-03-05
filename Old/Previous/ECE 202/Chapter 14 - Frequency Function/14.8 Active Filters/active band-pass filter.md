The [[first-order high-pass filter]] can be combined with the [[first-order low-pass filter]] that will have a gain $K$ over the required range of frequencies. 

By cascading a unity-gain low-pass filter, a unity-gain high-pass filter, and an inverter with gain $-\frac{R_{f}}{R_{i}}$, as shown in the block diagram.

![[Pasted image 20240408011217.png]]

We can construct a [[band-pass filter]] whose frequency response is that in (b). With the figure showing how to construct a [[band-pass filter]] 

![[Pasted image 20240408011350.png]]


The analysis of the band filter can be obtained by multiplying the two equations:
$$
H(\omega)=- \frac{R_{f}}{R_{i}+\frac{1}{j\omega C_{i}}}=\frac{j\omega C_{i}R_{f}}{1+j\omega C_{i}R_{i}}
$$
and
$$
H(\omega)=\frac{R_{f}}{R_{i}} \frac{1}{1+j\omega C_{f}R_{f}}
$$
which becomes:
$$
-\frac{R_{f}}{R_{i}} \frac{1}{1+j\omega C_{f}R_{f}} \frac{j\omega C_{i}R_{f}}{1+j\omega C_{i}R_{i}}
$$


The low-pass section sets the upper corner frequency as:
$$
\omega_{2}=\frac{1}{RC_{1}}
$$
while the high-pass section sets the lower corner frequency as
$$
\omega_{1}=\frac{1}{RC_{2}}
$$
With these values of $\omega_{1}$ and $\omega_{2}$, the center frequency, bandwidth, and [[Quality Factor]] are found as follows:
$$
\begin{align}
\omega_{0}=\sqrt{ \omega_{1}\omega_{2} } \\
B=\omega_{2}-\omega_{1}  \\
Q=\frac{\omega_{0}}{B}
\end{align}
$$
To find the passband gain $K$, we write found equation in the standard form as:
$$
H(\omega)=-\frac{R_{f}}{R_{i}} \frac{\frac{j\omega}{\omega_{1}}}{\left( 1+\frac{j\omega}{\omega_{1}} \right)\left( 1+\frac{j\omega}{\omega_{2}} \right)}=-\frac{R_{f}}{R_{i}} \frac{j\omega \omega_{2}}{(\omega_{1}+j\omega)(\omega_{2}+j\omega)}
$$
at the center frequency $\omega_{0}=\sqrt{ \omega_{1}\omega_{2} }$ the magnitude of the transfer function is
$$
|H(\omega_{0})|= |\frac{R_{f}}{R_{i}} \frac{j\omega \omega_{2}}{(\omega_{1}+j\omega)(\omega_{2}+j\omega)}|=\frac{R_{f}}{R_{i}} \frac{\omega_{2}}{\omega_{1}+\omega_{2}}
$$
Thus the passband gain is
$$
K=\frac{R_{f}}{R_{i}} \frac{\omega_{2}}{\omega_{1}+\omega_{2}}
$$
