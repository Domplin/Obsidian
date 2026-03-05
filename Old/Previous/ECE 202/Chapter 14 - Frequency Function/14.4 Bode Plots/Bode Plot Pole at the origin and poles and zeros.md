$$
\begin{align}
\text{Draw the Bode Diagram for the transfer function:} \\
H(s)=10 \frac{s+10}{s^2+3s}
\end{align}
$$
1) Rewrite the transfer function in proper form
	Make both the lowest order term in the numerator and denominator unity. The numerator is an order 1 polynomial, the denominator is order 2.
$$
H(s)=10 \frac{10}{3} \frac{\left( \frac{s}{10}+1 \right)}{s\left( \frac{s}{3}+1 \right)} = 33.3 \frac{\frac{s}{10}+1}{s\left( \frac{s}{3}+1 \right)}
$$
2) Separate the transfer function into its constituent parts
	The Transfer function has 4 components
	- A constant of 33.3
	- A pole at $s=-3$
	- A pole at $s=0$
	- A zero at $s=-10$
3) Draw the Bode diagram for each part 
	This is done in the diagram below
	- The constant is the cyan line (A quantity of 33.3 is equal to 30 dB).  The phase is constant at 0 degrees.
	- The pole at 3 rad/sec is the green line.  It is 0 dB up to the break frequency, then drops off with a slope of -20 dB/dec.  The phase is 0 degrees up to 1/10 the break frequency (0.3 rad/sec) then drops linearly down to -90 degrees at 10 times the break frequency (30 rad/sec).
	- The pole at the origin.  It is a straight line with a slope of -20 dB/dec.  It goes through 0 dB at 1 rad/sec.  The phase is -90 degrees.
	- The zero at 10 rad/sec is the red line.  It is 0 dB up to the break frequency, then rises at 20 dB/dec.  The phase is 0 degrees up to 1/10 the break frequency (1 rad/sec) then rises  linearly to 90 degrees at 10 times the break frequency (100 rad/sec).

4) Draw the overall Bode diagram by adding up the results from step 3
![[Pasted image 20240331184246.png]]
![[Pasted image 20240331184255.png]]
