
- What is a moment generating function?

*first moment* 
$$
E[X] = \int_{-\infty}^{\infty} x P_{X}(x) \, dx  \,  
$$
*second moment*
$$
E[X^2] = \int_{-\infty}^{\infty} x^2P_{X}(x) \, dx
$$
This pattern continues to find whichever moment is needed


**Moment Generating Function**
$$
M_{X}(t)=E[e^{tx}] =\int_{-\infty}^{\infty} e^{tx}P_{X}(x) \, dx 
$$

$E[e^{tx}]$ can then be expanded through a series expansion
$$
E[e^{tx}] = E\left[ 1 +x+\frac{t^2x^2}{2!}+\frac{t^3x^3}{3!}+\dots \right]
$$
Rearranging terms - each part of the equation contains a different moment
$$
E[e^{tx}]=1+tE[x]+\frac{t^2}{2!}E[x^2]+\frac{t^3}{3!}E[x^3]+\dots
$$
To find each of the different moments - Take the derivative respective to the moment that is trying to be obtained. 




**Gaussian**
$$
M_{X}(t)=e^{t\mu+ 1/2\sigma^2t^2}
$$
$$
\frac{dM_{X}(x)}{dt}=\mu e^{t\mu+1/2\sigma^2t^2}+e^{t\mu}\sigma^2te^{1/2\sigma^2t^2}
$$
when $t = 0$ → $= \mu$

