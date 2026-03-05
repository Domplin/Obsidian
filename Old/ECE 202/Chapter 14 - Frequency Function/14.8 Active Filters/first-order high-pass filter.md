The [[Transfer Function]] is the same as before:
$$
H(\omega)=\frac{V_{o}}{V_{i}}=-\frac{Z_{f}}{Z_{i}}
$$
![[Pasted image 20240408010551.png]]

Where $Z_{i}=R_{i}+\frac{1}{j\omega C_{i}}$ and $Z_{f}=R_{f}$ so that 
$$
H(\omega)=- \frac{R_{f}}{R_{i}+\frac{1}{j\omega C_{i}}}=\frac{j\omega C_{i}R_{f}}{1+j\omega C_{i}R_{i}}
$$
This is similar to the [[high-pass filter]] equation except that at very high frequencies $(\omega \rightarrow \infty)$ the gain tends to $-\frac{R_{f}}{R_{i}}$ 

The corner frequency is 
$$
\omega_{c}=\frac{1}{R_{i}C_{i}}
$$
