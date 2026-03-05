$\alpha<\omega_{0}$, $\frac{C<4L}{R^2}$ The roots may be written as 
$$
s_{1}=-\alpha+\sqrt{ -(\omega_{0}^2-\alpha^2) }=-\alpha+j\omega_{d}
$$
$$
s_{2}=-\alpha-\sqrt{ -(\omega_{0}^2-\alpha_{2}) }=-\alpha-j\omega_{d}
$$
where $j=\sqrt{ -1 }$ and $\omega_{d}=\sqrt{ \omega_{0}^2 -\alpha^2}$
This is called the damped frequency. Both $\omega_{0}$ and $\omega_{d}$ are natural frequencies because they help determine the natural response. While $\omega_{0}$ is often called the *undamped natural frequency*, $\omega_{d}$ is called the *damped natural frequency* 

The natural response is:
$$
i(t)-A_{1}e^{-(\alpha-j\omega_{d})t}+A_{2}e^{-(\alpha+j\omega_{d})t}=e^{-at}(A_{1}e^{-j\omega_{d}t}+A_{2}e^{-j\omega_{d}t})
$$
using Euler’s Identities
$$
\begin{align}
e^{j\theta}=\cos \theta+j\sin \theta  \\
e^{-j\theta}=\cos \theta-j\sin \theta
\end{align}
$$
We get
$$
e^{-\alpha t}[(A_{1}+A_{2})\cos \omega_{d}t+J(A_{1}-A_{2})\sin \omega_{d}t]
$$
Replacing $(A_{1}+A_{2})$ and $j(A_{1}-A_{2})$ with constants $B_{1}$ and $B_{2}$ we write:
$$
i(t)=e^{-\alpha t} (B_{1}\cos \omega_{d}t+B_{2}\sin \omega_{d}t)
$$


![[Pasted image 20240502193206.png]]
