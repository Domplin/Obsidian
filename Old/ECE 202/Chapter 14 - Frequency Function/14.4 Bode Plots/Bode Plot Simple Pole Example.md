$$
\begin{align}
\text{Draw the Bode Diagram for the transfer function} \\
H(s) = \frac{100}{s+30}
\end{align}
$$
1) Rewrite the Transfer function in proper form
	- Make both the lowest order term in the numerator and denominator unity. The numerator is and order 0 polynomial, the denominator is order 1.
	- $H(s)=\frac{100}{30} \frac{1}{\frac{s}{30}+1} = 3.3 \frac{1}{\frac{s}{30}+1}$

2) separate the transfer function into its constituent parts
	- The transfer function has 2 components
		- A constant of $3.3$
		- A pole at $-30$
3) Draw the Bode Diagram for each part
	- This is done in the diagram below
		- The constant is the cyan line (A quantity of 3.3 is equal to 10.4 dB). The phase is constant at 0 degrees
		- The pole at 30 rad/sec is the blue line. It is 0 dB up to the break frequency then drops off with a slope of -20 dB/dec. The phase is 0 degrees up to 1/10th the break frequency (3 rad/sec) then drops linearly down to -90 degrees at 10 time the break frequency (300 rad/sec).
4) Draw the overall Bode diagram by adding up the results from step 3.
![[Pasted image 20240331182006.png]]![[Pasted image 20240331182017.png]]
