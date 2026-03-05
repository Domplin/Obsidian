If $F(s)$ is the Laplace transform of $f(t)$, then
$$
L[f(t-a)u(t-a)]=\int ^\infty_{0^-}f(t-a)u(t-a)e^{-st} \, dt

$$
$$
a \ge 0
$$
But for $u(t-a)=0$ for $t<a$ and $u(t-a)=1$ for $t>1$ Hence:
$$
L[f(t-a)u(t-a)]=\int ^\infty_{0^-} f(t-a)e^{-st}\, dt 
$$
If we let $x=t-a$, then $dx=dt$ and $t=x+a$ as $t \rightarrow 0$ and as $t \rightarrow \infty$, $x \rightarrow \infty$ thus:
$$
\begin{align}
L[f(t-a)u(t-a)] = \int ^\infty_{0^-} f(x)e^{-s(x+a)} \, dx  \\
=e^{-as}\int ^\infty_{0^-}f(x)e^{-sx} \, dx =e^{-as}F(s)
\end{align}
$$
OR
$$
L[f(t-a)u(t-a)] = e^{-as}F(s)
$$

*in other words*: if a function is delayed in time by $a$ the result in the $s$-domain is found by multiplying the [[Previous/ECE 202/Chapter 15 - Introduction to the Laplace Transform/15.2 Definition of the Laplace Transform/Laplace Transform]] of the function (*without the delay*) by $e^{-as}$. This is called the *time-delay* or *time-shift property* of the [[Previous/ECE 202/Chapter 15 - Introduction to the Laplace Transform/15.2 Definition of the Laplace Transform/Laplace Transform]]


As an example we know that 
$$
L[\cos(\omega t)u(t)]=\frac{s}{s^2+\omega^2}
$$
Using the time-shift property
$$
L[\cos \omega(t-a)u(t-a)]=e^{-as} \frac{s}{s^2+\omega^2}
$$
