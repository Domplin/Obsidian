-Parallel RLC circuits find many practical applications, notably in communication networks and filter designs


Consider the parallel RLC circuit shown:
![[Pasted image 20240502193411.png]]
Assume initial inductor current $I_{0}$ and initial capacitor voltage $V_{0}$ 
$$
\begin{align}
i(0)=I_{0} =\frac{1}{L}\int ^0_{-\infty } v(t)\, dt \\
v(0)=V_{0} &  
\end{align}
$$

Because the three elements are in parallel, they have the same voltage $v$ across the. According to passive sign convention, the current is entering each element; that is, the current through each element is leaving the top node. Thus applying KCL at the top node gives:
$$
\frac{v}{R}+\frac{1}{L}\int ^t_{-\infty}v(\tau) \, d\tau+C \frac{dv}{dt}=0
$$
Taking the derivative with respect to $t$ and dividing by *C* results in:
$$
\frac{d^2v}{dt^2}+\frac{1}{RC} \frac{dv}{dt}+\frac{1}{LC}v=0
$$
We obtain the characteristic equation by replacing the first derivative by $s$ and the second derivative by $s^2$.
By following the same reasoning as [[Series RLC Circuit]] the [[characteristic equation]] is obtained as:
$$
s^2+\frac{1}{RC}s+\frac{1}{LC}=0
$$
The roots of the [[characteristic equation]] are 
$$
s_{1,2}=-\frac{1}{2RC}\pm \sqrt{ \left( \frac{1}{2RC} \right)^2-\frac{1}{LC} }
$$
or
$$
s_{1,2}=-\alpha\pm \sqrt{ \alpha^2-\omega_{0}^2 }
$$
where 
$$
\begin{align}
\alpha=\frac{1}{2RC} \\
\omega_{0}=\frac{1}{\sqrt{ LC }}
\end{align}
$$
The names of these terms remain the same as  in the [[characteristic equation]] section, and play the same role in the solution.

Again there are three possible solutions depending on
- $\alpha>\omega_{0}$
- $\alpha=\omega_{0}$
- $\alpha<\omega_{0}$

1) [[Parallel RLC Overdamped]]
2) [[Parallel RLC Critically Damped]]
3) [[Parallel RLC Underdamped]]