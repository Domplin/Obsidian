The **Half-Power Frequencies** are obtained by setting Z equal to $\sqrt{ 2 }R$ and writing
$$
\sqrt{ R^2+\left( \omega L-\frac{1}{\omega C} \right)^2 }=\sqrt{ 2 }R
$$
Solving for $\omega$ we obtain
$$
\begin{align}
\omega_{1}=-\frac{R}{2L}+\sqrt{ \left( \frac{R}{2L} \right)^2 +\frac{1}{LC}} \\
\omega_{2}=\frac{R}{2L}+\sqrt{ \left( \frac{R}{2L} \right)^2 +\frac{1}{LC}} 
\end{align}
$$
We can relate the *half-power frequencies* with the resonant frequency from the above equations and the equation:
$$
\omega_{0}=\frac{1}{\sqrt{ LC }}\text{rad/s}
$$
getting:
$$
\omega_{0}=\sqrt{ \omega_{1}\omega_{2} }
$$


The height of the curve from the graph in [[ECE 202/Chapter 14 - Frequency Function/Series Resonance/Series Resonance|Series Resonance]] is determined by $R$ the width of the response curve depends on the *bandwidth* $B$ which is defined as the difference between the two half-power frequencies,
$$
B=\omega_{2}-\omega_{1}
$$

The “Sharpness” of the resonance in a resonance circuit is measured quantitatively by the [[Quality Factor]] $Q$ 