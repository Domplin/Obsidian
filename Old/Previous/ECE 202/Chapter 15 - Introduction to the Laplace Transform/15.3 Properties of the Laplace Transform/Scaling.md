If $F(s)$ is the Laplace transform of $f(t)$ then
$$
L[f(at)]=\int ^\infty _{0^-}f(at)e^{-st}  \, dt
$$
where $a$ is a constant and $a>0$. If we let $x=at$, $dx=a$ $dt$ then:
$$
L[f(at)]=\int ^\infty _{0^-}f(x)e^{-x(s/a)} \, \frac{dx}{a}=\frac{1}{a}\int ^\infty _{0^-}f(x)e^{-x(s/a)}\, dx
$$
Comparing this integral with the definition of the Laplace transform from the equation in [[Previous/ECE 202/Chapter 15 - Introduction to the Laplace Transform/15.2 Definition of the Laplace Transform/Laplace Transform]] it shows that $s$ must be replaced by a $\frac{s}{a}$ while the dummy variable $t$ is replaced by $x$ 

We obtain the scaling property as:
$$
L[f(at)]=\frac{1}{a}F\left( \frac{s}{a} \right)
$$
**Example**
we know that 
$$
L[\sin \omega tu(t)] = \frac{\omega}{s^2+\omega^2}
$$
Using the scaling property:
$$
L[\sin_{2}\omega tu(t)]=\frac{1}{2} \frac{\omega}{\left( \frac{s}{2} \right)^2+\omega^2}=\frac{2\omega}{s^2+\omega^2}
$$
Which may also be obtained from replacing $\omega$ with $2\omega$ in the second equation