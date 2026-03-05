Because KCL is valid for [[Phasor]]s, we can analyze ac circuits by nodal analysis. 
*Find $i_x$ in the circuit of [[Figure 10.1.png]] using nodal analysis*
![[Figure 10.1.png]]

**Solution:**
1) Convert the circuit to the frequency domain - 
$$
20\cos(4t) = 20\angle 0^{\degree}
$$
$$
\begin{align}
\text{1 H Inductor -> } j\omega L=j 4 \\
\text{0.5 H Inductor -> } j\omega L=j2 \\
\text{0.1 F Capacitor -> } \frac{1}{j\omega C}=-j2.5
\end{align}
$$


![[Figure 10.2.png]]

- Applying KCL at node 1:
$$
\frac{20-V_{1}}{10}=\frac{V_{1}}{-j2.5}+\frac{V_{1}-V_{2}}{j_{4}}
$$
or
$$
(1+j1.5)V_{1}+J2.5V_{2}=20
$$
- At node 2:
$$
2I_{x}+\frac{V_{1}-V_{2}}{j4}=\frac{V_{2}}{j 2}
$$

Because $I_{x} = \frac{V_{1}}{-j2.5}$ substituting in and simplifying we get:
$$
11V_{1}+15V_{2} = 0
$$
![[Solving Nodal analysis with matri.png]]
It can then be transformed into time domain:
$$
i_{x}=7.59\cos(4t+108.4^{\degree})A
$$
