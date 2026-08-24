The transient response is always a decaying exponential:
$$
\begin{align}
i_{t}=Ae^{-t/\tau} \\
\tau=\frac{L}{R}
\end{align}
$$
Where *A* is to be determined 
The [[Steady-State Response|steady-state response]] is the value of the current a long time after the switch is closed. The transient response essentially dies out after five time constants. 

After that time the inductor becomes a short circuit, and the voltage across it 0.

The [[Steady State Response|steady state response]] is:
$$
i_{ss}=\frac{V_{S}}{R}
$$
We now determine the constant A from the initial value of *i*. Let $I_{0}$ be the initial current through the inductor, which may come from a source other than $V_{s}$. Since the current through an inductor cannot change instantaneously:
$$
i(0^{+})=i(0^{-})=I_{0} 
$$
At $T=0$ it becomes:
$$
I_{0}=A+\frac{V_{S}}{R}
$$
We can obtain A as:
$$
A=I_{0}-\frac{V_{s}}{R}
$$
