**Magnitude scaling** is the process of increasing all impedances in a network by a factor, the frequency response remaining unchanged 

Recall that [[Impedance]]s of individual elements R, L, and C are given by
$$
\begin{align}
Z_{R}=R \\
Z_{L}=j\omega L &  \\
Z_{C}=\frac{1}{j\omega C} 
\end{align}
$$
In magnitude scaling, we multiply the impedance of each circuit element by a factor of $K_{m}$ and let the frequency remain constant. This gives the new impedance as:
$$
\begin{align}
Z^{'}_{R}=K_{m}Z_{R}=K_{m}R \\
Z^{'}_{L}=K_{m}Z_{L}=j\omega K_{m}L \\
Z^{'}_{C}=K_{m}Z_{C}=\frac{1}{j\omega  \frac{C}{K_{m}}}
\end{align}
$$
Comparing the two groups of equations, the following changes in the elements are noticeable: $R \rightarrow K_{m}R\text{, } L\rightarrow K_{m}L \text{, and } C \rightarrow \frac{C}{K_{m}}$ Thus the new values of the elements and frequency are:
$$
\begin{align}
R^{'}=K_{m}R \\
L^{'}=K_{m}L \\
C^{'}=\frac{C}{K_{m}}
\end{align}
$$
The primed variable are the new values and the unprimed variable and the old values. Consider the series of parallel RLC circuit. We now have:
$$
\omega^{'}_{0}=\frac{1}{\sqrt{ L^{'}C^{'} }}=\frac{1}{\frac{K_{m}LC}{K_{m}}}=\frac{1}{\sqrt{ LC }}=\omega_{0}
$$
This shows that the resonant frequency has not changed. Similarly the [[Quality Factor]] and the bandwidth are not affected by magnitude scaling. It also doesn’t affect [[Transfer Function]]s 

