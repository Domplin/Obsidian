$$
\begin{align}
\text{Draw the Bode Diagram for the transfer function:} \\
H(s)=100 \frac{s+1}{(s+10)(s+100)} = 100 \frac{s+1}{s^2+110s+1000}
\end{align}
$$
1) Rewrite the transfer function in proper form
	Make both the lowest order term in the numerator and denominator unity. The numerator is an order 1 polynomial, the denominator is order 2.

$$
H(s)=\frac{100}{10*100} \frac{\left( \frac{s}{1}+1 \right)}{\left( \frac{s}{10}+1 \right)\left( \frac{s}{100}+1 \right)} = 0.1 \frac{\left( \frac{s}{1}+1 \right)}{\left( \frac{s}{10}+1 \right)\left( \frac{s}{100}+1 \right)}
$$

2) Separate the transfer function into its constituent parts
	The transfer function has 4 components:
	- A constant of $0.1$
	- A pole at $s=-10$
	- A pole at $s=-100$
	- A zero at $s=-1$

3) Draw the Bode diagram for each part
	This is done in the diagram below.
	- The constant is the cyan line (A quantity of 0.1 is equal to -20 dB).  The phase is constant at 0 degrees.
	- The pole at 10 rad/sec is the green line.  It is 0 dB up to the break frequency, then drops off with a slope of -20 dB/dec.  The phase is 0 degrees up to 1/10 the break frequency (1 rad/sec) then drops linearly down to -90 degrees at 10 times the break frequency (100 rad/sec).
	- The pole at 100 rad/sec is the blue line.  It is 0 dB up to the break frequency, then drops off with a slope of -20 dB/dec.  The phase is 0 degrees up to 1/10 the break frequency (10 rad/sec) then drops linearly down to -90 degrees at 10 times the break frequency (1000 rad/sec).
	- The zero at 1 rad/sec is the red line.  It is 0 dB up to the break frequency, then rises at 20 dB/dec.  The phase is 0 degrees up to 1/10 the break frequency (0.1 rad/sec) then rises  linearly to 90 degrees at 10 times the break frequency (10 rad/sec).

4) Draw the overall Bode diagram by adding up the results from step 3

![[Pasted image 20240331183019.png]]![[Pasted image 20240331183029.png]]
