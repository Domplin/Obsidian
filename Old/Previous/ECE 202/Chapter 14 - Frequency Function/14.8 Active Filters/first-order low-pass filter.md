One type of first order filter is shown, The components selected for $Z_{i}$ and $Z_{f}$ determine whether its a [[low-pass filter]] or [[high-pass filter]], but one of the components must be reactive
![[Pasted image 20240408005918.png]]


The figure shows a typical active [[low-pass filter]]. For this filter, the transfer function is:
$$
H(\omega)=\frac{V_{o}}{V_{i}}=-\frac{Z_{f}}{Z_{i}}
$$
![[Pasted image 20240408010057.png]]

Where $Z_{i}=R_{i}$ and
$$
Z_{f}=Rf// \frac{1}{j\omega C_{f}}=\frac{R_{f}/j\omega C_{f}}{R_{f}\omega C_{f}}=\frac{R_{f}}{1+j\omega C_{f}R_{f}}
$$
Therefore:
$$
H(\omega)=\frac{R_{f}}{R_{i}} \frac{1}{1+j\omega C_{f}R_{f}}
$$
The corner frequency is:
$$
\omega_{c}=\frac{1}{R_{f}C_{f}}
$$
which dose not depend on $R_{i}$. This means that several inputs with different $R_{i}$ could be summed if required, and the corner frequency would remain the same for each input