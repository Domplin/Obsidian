*note*: all notes and linked notes are taken from:
https://lpsa.swarthmore.edu/Bode/Bode.html


1) Rewrite the [[Transfer Function|transfer function]] in proper form
**Example 1** 
- $H(s) = 30\frac{s+10}{s^2+3s+50}=30 \frac{10 \frac{s}{10}+1}{50 \left( \frac{s^2}{50}+\frac{3s}{50} +1 \right)} =6 \frac{\frac{s}{10}+1}{\frac{s^2}{50}+\frac{3s}{50}+1}$
*note*: the final result has the lowest (zero) order power of numerator and denominator polynomial equal to unity

**Example 2**
- $H(s) = 30 \frac{5s}{s^2+3s+50} = 30 \frac{5}{50} \frac{\frac{s}{1}}{\frac{s^2}{50}+\frac{3s}{50}+1} =3 \frac{\frac{s}{1}}{\frac{s^2}{50}+\frac{3s}{50}+1}$
*note*: that in this example, the lowest power in the numerator was one

**Example 3**
- $H(s) = 30 \frac{s+10}{(s+3)(s+50)} = 30 \frac{10}{3 * 50} \frac{\frac{s}{10}+1}{\left( \frac{s}{3} +1 \right) \left( \frac{s}{50}+ 1 \right)}$
*note*: In this example the denominator was already factored. In cases like this, each factored term needs to have unity as the lowest order power of s (zero in this case)

2) Separate the transfer function into its constituent parts
	1) A constant
	2) Poles at the origin
	3) Zeros at the origin
	4) Real poles
	5) Real Zeros
	6) Complex conjugate poles
	7) Complex conjugate zeros

Using the above examples:
**Example 1**
- $H(s) = 30\frac{s+10}{s^2+3s+50}=30 \frac{10 \frac{s}{10}+1}{50 \left( \frac{s^2}{50}+\frac{3s}{50} +1 \right)} =6 \frac{\frac{s}{10}+1}{\frac{s^2}{50}+\frac{3s}{50}+1}$
This function has
- A constant of 6
- a zero at $s=-10$
- complex conjugate poles at the roots of $s^2+3s+50$
The complex conjugate poles are at $s=-1.5 \pm j 6.9$ where $j = \sqrt{ -1 }$. A more common (and useful for out purposes) way to express this is to use the standard notation for a second order polynomial
$$
\left( \frac{s}{\omega_{0}} \right)^2+2c\left( \frac{s}{\omega_{0}} \right)+1
$$
In this case:
$$
\begin{align}
\omega_{0}=\sqrt{ 50 }=7.07 \\
c=\frac{3\sqrt{ 50 }}{2*50} =0.21
\end{align}
$$
**Example 2**
- $H(s) = 30 \frac{5s}{s^2+3s+50} = 30 \frac{5}{50} \frac{\frac{s}{1}}{\frac{s^2}{50}+\frac{3s}{50}+1} =3 \frac{\frac{s}{1}}{\frac{s^2}{50}+\frac{3s}{50}+1}$
This function has
- a constant of 3
- a zero at the origin
- a complex conjugate poles at the roots of $s^2+3s+50$ 
$$
\begin{align}
\omega_{0}=\sqrt{ 50 }=7.07 \\
c=\frac{3\sqrt{ 50 }}{2*50}=0.21
\end{align}
$$
**Example 3**
- $H(s) = 30 \frac{s+10}{(s+3)(s+50)} = 30 \frac{10}{3 * 50} \frac{\frac{s}{10}+1}{\left( \frac{s}{3} +1 \right) \left( \frac{s}{50}+ 1 \right)}$
This function has
- a constant of 2
- a zero at $s=-10$
- poles at $s=-3$ and $s=-50$ 


3) Draw the Bode diagram for each part
	*The Rules for drawing the Bode diagram for each part are on a different page*: [[Drawing a Bode Plot]]

4) Draw the overall Bode diagram by adding the results from step 3
	1) **Example 1** - A simple pole: [[Bode Plot Simple Pole Example]]
	2) **Example 2** - Multiple poles and zeros: [[Bode Plot Multiple Poles and Zeros]]
	3) **Example 3** - Pole at the origin and poles and zeros: [[Bode Plot Pole at the origin and poles and zeros]]
	4) Other examples are available on the site 