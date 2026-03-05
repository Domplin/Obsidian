The process of taking a rational expression and decomposing it into simpler rational expressions that we can add or subtract to get the original rational expression is called **partial fraction decomposition** 

Many integrals involving rational expressions can be done if we first do partial fraction on the integrand

A quick review:
$$
f(x)=\frac{P(x)}{Q(x)}
$$
where both $P(x)$ and $Q(x)$ are polynomials and the degree of $P(x)$ is smaller than the degree of $Q(x)$ 

Once its been determined that partial fractions can be done we do the following:
- factor the denominator as much as possible
- For each factor in the denominator we can use the following table to determine the term(S) we pick up in the partial fraction decomposition
![[Pasted image 20240501204745.png]]



**Example 1:** Evaluate the following integral
$$
\int \frac{3x+11}{x^2-x-6} \, dx
$$

*Solution:*
- The first step is to factor the denominator as much as possible and get the form of the partial fraction decomposition. Doing this gives:
$$
\frac{3x+11}{(x-3)(x+2)} = \frac{A}{x-3} + \frac{B}{x+2}
$$
- The next step is to add the right side back up:
$$
\frac{3x+11}{(x-3)(x+2)} = \frac{A(x+2)+B(x-3)}{(x-3)(x+2)}
$$
- Now we need to choose **A** and **B** so that the numerators of these two are equal for every $x$. To do this we’ll set the numerators equal 
$$
3x+11=A(x+2)+A(x-3)
$$
- There are two ways to proceed. One will always work but is more work. The other will sometimes work and is quicker. In this example I will use the *shorter* method.
- What we’re going to do here is to notice that the numerators must be equal for *any* $x$ that we would choose to use. In particular the numerators must be equal for $x=-2$ and $x=3$. So lets plug these in and see what we get.

$$
\begin{align}
x=-2 \rightarrow 5=A(0)+B(-5) \rightarrow B=-1  \\
x=3 \rightarrow{   }  20=A(5)+B(0) \rightarrow A=4
\end{align}
$$
- at this point there really isn’t a whole lot to do besides to do the integral

$$
\int \frac{3x+11}{x^2-x-6}dx=\int \frac{4}{x-3} - \frac{1}{x+2} \,   \, dx 
$$
$$
=4\ln|x-3| -\ln|x+2|+c
$$