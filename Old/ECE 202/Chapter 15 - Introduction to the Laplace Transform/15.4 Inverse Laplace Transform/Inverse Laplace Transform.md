Given $F(s)$ how do we transform it back to the time domain and obtain the corresponding $f(t)$?

By matching entries in [[Properties of the Laplace Transform]] table we can avoid using an equation to find $f(t)$ 

Suppose $F(s)$ has the general form of 
$$
F(s) \frac{N(s)}{D(s)}
$$
where $N(s)$ is the numerator polynomial and $D(s)$ is the denominator polynomial. The roots of $N(s)=0$ are called the *zeros* of $F(s)$ while the roots of $D(s)=0$ are the *poles* of $F(s)$ 
*[[Zeros and Poles]]


We use *[[Partial Fraction Decomposition]]* to break $F(S)$ down into simple terms whose inverse transform we obtain from [[Laplace transform pairs]] table


**Steps to Find the Inverse Laplace Transform:**
1) Decompose $F(s)$ into simple terms using partial fraction expansion
2) Find the inverse of each term by matching entries in [[Laplace transform pairs]]


**Possible forms of $F(s)$ are:**
1) [[Simple Poles]]
2) [[Repeated Poles]]
3) [[Complex Poles]]

Whether the pole is simple, repeated, or complex, a general approach that can always be used in finding the expansion coefficients is the *method of algebra*. To apply the method we 
- set $F(s)= \frac{N(s)}{D(s)}$ equal to an expansion containing unknown constants. 
- We multiply the result through by a common denominator.
- We then determine the unknown constants by equating coefficients


Another general approach is to substitute specific, convenient values of $s$ to obtain as many simultaneous equation as the number of known coefficients, and then solve for the unknown coefficients. We must make sure that each selected value of $s$ is not one of the poles of $F(s)$
