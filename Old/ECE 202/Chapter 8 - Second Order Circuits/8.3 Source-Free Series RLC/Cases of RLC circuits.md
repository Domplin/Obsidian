The two values of $s$ from the [[characteristic equation]] indicate that there are two possible solutions for $i$ each of which is of the form of the assumed solution:
$$
\begin{align}
i_{1}=A_{1}e^{s_{1}t} \\
i_{2}=A_{2}e^{s_{2}t}
\end{align}
$$
Since the equation is a linear equation, any linear combination of the two distinct solutions, $i_{1}$ and $i_{2}$ is also a solution.

A complete or total solution would therefore require a linear combination of $i_{1}$ and $i_{2}$. Thus the natural response of the [[Series RLC Circuit]] is:
$$
i(t)=A_{1}e^{s_{1}t}+A_{2}e^{s_{2}t}
$$
where the constants $A_{1}$ and $A_{2}$ are determined from the initial values $i(0)$ and $\frac{di(0)}{dt}$ 

The response is *overdamped* when the roots of the circuit’s [[characteristic equation]] are unequal and real

*critically damped* when the roots are equal and real

*underdamped* when the roots are complex

From that we can infer that there are three types of solutions

| Cases                                                          |
| -------------------------------------------------------------- |
| 1) if $\alpha >\omega_{0}$ we have *overdamped* case           |
| 2) if $\alpha=\omega_{0}$ we have the *critically damped* case |
| 3) if $\alpha<\omega_{0}$ we have the *underdamped* case       |

Looking at each of these separately:
[[Series RLC Overdamped]]
[[Series RLC Critically Damped]]
[[Series RLC Underdamped Case]]