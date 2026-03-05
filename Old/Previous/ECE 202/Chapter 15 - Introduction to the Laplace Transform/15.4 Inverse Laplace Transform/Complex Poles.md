A pair of complex poles is simple if it is not repeated; it is a double or multiple pole if repeated. Simple complex poles may be handled the same way as simple real poles, but because complex algebra is involved the result is always cumbersome. An easier approach is a method  known as *completing the square*. The idea to express each complex pole pair (or quadratic term) in $D(s)$ as a complete square such as $(s+\alpha)^2+\beta^2$ and then use [[Laplace transform pairs]] to find the inverse of the term


Because $N(s)$ and $D(s)$ always have real coefficients and we know that complex roots of polynomials with real coefficients must occur in conjugate pairs, $F(s)$ may have the general form
$$
F(s)=\frac{A_{1}s+A_{2}}{S^2+as+b}+F_{1}(s)
$$
Where $F_{1}(s)$ is the remaining part of $F(s)$ that doe snot have this pair of complex poles. If we complete the square by letting 
$$
S^2+as+b=s^2\alpha s+\alpha^2+\beta^2=(s+\alpha)^2+\beta^2
$$
and we also let
$$
A_{1}s+A_{2}=A_{1}(s+a)+B_{1}\beta
$$
then the $F(s)$ equation becomes
$$
F(s)=\frac{A_{1}(s+\alpha)}{(s+\alpha)^2+\beta^2}+\frac{B_{1}\beta}{(s+\alpha)^2+\beta^2}+F_{1}(s)
$$
From the [[Laplace transform pairs]] table, the inverse transform is:
$$
f(t)=(A_{1}e^{-\alpha t}\cos \beta t+B_{1}e^{-\alpha t}\sin \beta t)u(t)+f_{1}(t)
$$


