*note*: also see [[Constructing a Bode plot]]



- Constant $K$
	- *magnitude*: $20\log_{10}(|K|)$ 
	- *phase*: $K>0: 0^\degree$  $K < 0: \pm 0^\degree$


- Pole at Origin - (Integrator) $\frac{1}{s}$ 
	- *magnitude*: -20dB/decade passing through 0dB at $\omega=1$ 
	- *phase*: $-90^\degree$


- Zero at Origin - (Differentiator) $s$
	- *magnitude*: +20dB/decade passing through 0dB at $\omega=1$
	- *phase*: $+90^\degree$


- Real pole - $\frac{1}{\frac{s}{\omega_{0}}+1}$
	- *magnitude*:
	1) Draw low frequency asymptote at 0dB
	2) Draw high frequency asymptote at -20dB/decade
	3) Connect lines at $\omega_{0}$
	- *phase*:
	1) Draw low frequency asymptote at $0^\degree$
	2) Draw high frequency asymptote at $-90^\degree$
	3) Connect with a straight line from $0.1*\omega_{0}$ to $10*\omega_{0}$


![[Pasted image 20240331180255.png]]


For multiple order poles and zeros, simply multiply the slope of the magnitude plot by the order of the pole (or zero) and multiply the high and low frequency asymptotes of the phase by the order of the system.

**For example** 
Second order real pole: $\frac{1}{\left( \frac{s}{\omega_{0}}+1 \right)^2}$
1) Draw low frequency asymptote at 0 dB
2) Draw high frequency asymptote at -50 dB/decade
3) Connect lines at break frequency 
*-40 dB/decade is used because of order of pole = 2. For a third order pole, asymptote is -60 dB/decade* 

1) Draw low frequency asymptote at $0^\degree$
2) Draw high frequency asymptote at $-180^\degree$
3) Connect with a straight line from $0.1*\omega_{0}$ to $10*\omega_{0}$ 
*$-180^\degree$ is used because order of pole = 2 For a third order pole, high frequency asymptote is at $-270^\degree$
