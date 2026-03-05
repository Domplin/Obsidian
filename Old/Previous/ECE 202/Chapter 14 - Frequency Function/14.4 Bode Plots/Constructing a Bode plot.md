
In Constructing a Bode plot, we plot each factor separately and then add them graphically. The factors may be considered one at a time and them combined additively because of the logarithms involved. 

**Constant Term**: For the gain *K* the magnitude is $20\log_{10} K$ and the phase is $0^{\degree}$. Both are constant with frequency, Thus the magnitude and phase plots of the gain are shown. If *K* is negative, the magnitude remains $20\log_{10} |K|$ but the phase is $\pm 180^{\degree}$ 
![[Pasted image 20240328184052.png]]

**Pole/Zero at the origin**: For the zero ($j\omega$) at the origin the magnitude is $20\log_{10}\omega$ and the phase is $90^{\degree}$. These are plotted, where the slope of the magnitude plot is 20 dB/decade while phase is constant with frequency.
![[Pasted image 20240328184320.png]]

**Simple pole/zero**: For the simple zero $1+\frac{j\omega}{z_{1}}$ the magnitude is $20\log_{10}|1+\frac{j\omega}{z_{1}}|$ and the phase is $\tan^{-1} \frac{\omega}{z_{1}}$ we notice that:
$$
\begin{align}
H_{dB}=20\log_{10}|1+\frac{j\omega}{z_{1}}| \rightarrow 20\log_{10}1=0: As_{.} \omega = 0 \\
H_{dB}=20\log_{10}|1+\frac{j\omega}{z_{1}}| \rightarrow 20\log_{10} \frac{\omega}{z_{1}} : As_{.} \omega = \infty
\end{align}
$$
Showing we can approximate the magnitude as zero (a straight line with zero slope) for small values of $\omega$ and by a straight line with slope 20 dB/decade for large values of $\omega$ the frequency $\omega=z_{1}$ where the two asymptotic lines meet is called the *corner frequency* or *break frequency* 

The phase $\tan^{-1}\left( \frac{\omega}{z_{1}} \right)$ can be expressed as:
![[Pasted image 20240328185146.png]]

