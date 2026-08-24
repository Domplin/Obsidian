The [[Parallel RLC Circuit|parallel RLC circuit]] is the dual of the [[Series Resonance]] RLC circuit. The [[Admittance|admittance]] is
$$
Y=H(\omega)=\frac{I}{V} =\frac{1}{R}+j\omega C+\frac{1}{j\omega L}
$$
![[Pasted image 20240407220716.png]]

or
$$
Y=\frac{1}{R}+j\left( \omega C-\frac{1}{\omega L} \right)
$$
Resonance occurs when the imaginary part of $Y$ is zero
$$
\omega C-\frac{1}{\omega L}=0
$$
or
$$
\omega_{0}=\frac{1}{\sqrt{ LC }}\text{rad/s}
$$
which is the same as [[Series Resonance]] circuit. The voltage $|V|$ is shown in the figure as a function of frequency. 
![[Pasted image 20240407221016.png]]
- Notice that at resonance the parallel LC combination acts like an open circuit so that the entire current flows through R
- Also at the inductor and capacitor current can be much more than the source current at resonance 

The duality between the parallel and series circuit shown in [[Series Resonance]] means the equations can be compared by replacing $R$,$L$, and $C$ in the expressions for the series circuit with $\frac{1}{R}$, $C$, $L$ we obtain the equations for the parallel circuit
$$
\begin{align}
\omega_{1}=-\frac{1}{2RC}+\sqrt{ \left( \frac{1}{2RC} \right)^2+\frac{1}{LC} }  \\
\omega_{2}=\frac{1}{2RC}+\sqrt{ \left( \frac{1}{2RC} \right) ^2 +\frac{1}{LC} } \\
\end{align}
$$

$$
B=\omega_{2}-\omega_{1}=\frac{1}{RC}
$$

$$
Q=\frac{\omega_{0}}{B}=\omega_{0}RC=\frac{R}{\omega_{0}L}
$$
It should be noted that the top and bottom equations only apply to a parallel RLC circuit

We can express the [[Half-Power Frequencies|half-power frequencies]] in terms of the [[Quality Factor]]. The result is:
$$
\begin{align}
\omega_{1}\approx \omega_{0}\sqrt{ 1+\left( \frac{1}{2Q} \right)^2 } -\frac{\omega_{0}}{2Q} \\
\omega_{2}=\omega_{0}\sqrt{ 1+\left( \frac{1}{2Q} \right)^2  } - \frac{\omega_{0}}{2Q} 
\end{align}
$$

For the high-$Q$ circuits ($Q > 10$) 
$$
\begin{align}
\omega_{1}\approx \omega_{0}-\frac{B}{2} \\
\omega_{2}\approx \omega_{0}+\frac{B}{2}
\end{align}
$$
The table shows a summary of the characteristics of the series and parallel resonant circuits
![[Table 14.4 - Characteristics of Resonant RLC Circuits.png]]