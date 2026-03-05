If $F_{1}(s)$ and $F_{2}(s)$ are respectively, the Laplace transform of $f_{1}(t)$ and $f_{2}(t)$, then:
$$
L[a_{1}f_{1}(t)+a_{2}+f_{2}(t)] = a_{1}F_{1}(s)+a_{2}F_{2}(s)
$$
where $a_{1}$ and $a_{2}$ are constants 

we may write the linearity property as:
$$
L[\cos \omega u(t)] =L\left[ \frac{1}{2}e^{j\omega t}+e^{-j\omega t} \right]=\frac{1}{2} L[e^{j\omega t}]+\frac{1}{2}L[e^{-j\omega t}]
$$
But $L[e^{at}]=\frac{1}{(s+a)}$ hence:
$$
L[\cos \omega tu(t)]=\frac{1}{2}\left( \frac{1}{s-j\omega}+\frac{1}{s+j\omega} \right)=\frac{s}{s^2+\omega^2}
$$
