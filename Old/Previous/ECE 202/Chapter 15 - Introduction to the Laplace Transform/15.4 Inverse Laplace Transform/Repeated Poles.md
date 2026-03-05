Suppose $F(s)$ has $n$ repeated poles at $s=-p$. Then we may represent $F(s)$ as
$$
\begin{align}
F(s)= \frac{k_{n}}{(s+p)^n}+\frac{k_{n-1}}{(s+p)^{n-1}}+\dots+\frac{k_{2}}{(s+p)^2} \\
+\frac{k_{1}}{s+p}+F_{1}(s)
\end{align}
$$
Where $F_{1}(s)$ is the remaining part of $F(s)$ that does not have a pole at $s=-p$. We determine the expansion of coefficient $k_{n}$ as:
$$
k_{n}=(s+p)^nF(s)|_{s=-p}
$$
As we did above to determine $k_{n-1}$ ew multiply each term in the $F(s)$ equation by $(s+p)^n$ and differentiate to get rid of $k_{n}$ then evaluate the result at $s=-p$ to get rid of the other coefficients except $k_{n-1}$

Thus we obtain:
$$
k_{n-1}=\frac{d}{ds}[(s+p)^nF(s)]|_{s=-p}
$$
Repeating this gives
$$
k_{n-2}=\frac{1}{2!}\frac{d^2}{ds^2}[(s+p)^nF(s)]|_{s=-p}
$$
The *m*th term becomes 
$$
k_{n-m}=\frac{1}{m!} \frac{d^2}{ds^2}[(s+p)^nF(s)]|_{s=-p}
$$
where $m=1,2,\dots ,n-1$. One can expect the differentiation to be difficult as *m* increases. Once we obtain the values of $k_{1},k_{2},\dots,k_{n}$ by partial fraction expansion, we apply the inverse transform
$$
L^{-1}\left[ \frac{1}{(s+a)^n} \right]=\frac{t^{n-1}e^{-at}}{(n-1)!}u(t)
$$
to each term on the right-hand side of the $F(s)$ equation and obtain:
$$
f(t)=\left( k_{1}e^{-pt}+k_{2}te^{-pt}+\frac{k_{3}}{2!}t^2e^{-pt}+\dots+\frac{K_{n}}{(n-1)!}t^{n-1}e^{-pt} \right)u(t)+f_{1}(t)
$$
