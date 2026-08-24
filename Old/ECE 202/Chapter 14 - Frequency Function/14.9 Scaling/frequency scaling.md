**Frequency scaling** is the process of shifting the [[Frequency Response|frequency response]] of a network up or down the frequency axis while leaving the [[Impedance|impedance]] the same

We achieve frequency scaling by multiplying the frequency by a factor $K_{f}$ while keeping the impedance the same. From the equations from [[Impedance]] we can see they are frequency dependent. If we apply frequency scaling to $Z_{L}(\omega)$ and $Z_{C}(\omega)$ we obtain:
$$
\begin{align}
Z_{L}=j(\omega K_{f})L^{'}=j\omega L \rightarrow L^{'}=\frac{L}{K_{f}} \\
Z_{C}=\frac{1}{j(\omega K_{f})C^{'} } =\frac{1}{j\omega C} \rightarrow C^{'}=\frac{C}{K_{f}}
\end{align}
$$
Since the impedance of the inductor and capacitor must remain the same after frequency scaling. We notice the following changes in the element values: $L \rightarrow \frac{L}{K_{f}}$ and $C \rightarrow \frac{C}{K_{f}}$. The value of R is not affected since its [[Impedance]] does not depend on frequency. Thus in frequency scaling, the new values of the elements and frequency are
$$
\begin{align}
R^{'}=R \\
L^{'}=\frac{L}{K_{f}} \\
C^{'}=\frac{C}{K_{f}^{'}} \\
\omega^{'}=K_{f}\omega
\end{align}
$$

Again if series or parallel RLC circuits are considered for the [[Series Resonance]] 
$$
\omega^{'}_{0}=\frac{1}{\sqrt{ L^{'}C^{'} }}=\frac{1}{\sqrt{ \frac{L}{K_{f}} \frac{C}{K_{f}} }}= \frac{K_{f}}{\sqrt{ RC }}= K_{f}\omega_{0}
$$
and for bandwidth
$$
B^{'}=K_{f}B
$$
the [[Quality Factor]] stays the same $Q^{'}=Q$
