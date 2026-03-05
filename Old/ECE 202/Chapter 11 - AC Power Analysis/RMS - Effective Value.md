The **Effective Value** of a periodic current is the dc current that delivers the same average power to a resistor as periodic current 


$$
P=\frac{1}{T}\int_{0} ^T i^2R dt
$$
$$
\frac{R}{T}\int _{0}^T i^2 \, dt
$$

Power absorbed by the resistor can be written as:
$$
P=i_{eff}^2 R
$$
using these two equations the **effective value** can be found: 
$$
S_{eff}=\sqrt{\frac{1}{T}\int _{0}^Ts^2 \, dt  }
$$
where $S_{eff}$ is either $V_{eff}$ or $I_{eff}$ depending on what $s$ is, either being voltage:$v$ or current: $i$ 

The effective value is the square root of the average of the periodic signal. Because of this the value is commonly known as the *root-mean-square* value or *RMS*
$$
\begin{align}
I_{eff} = I_{rms} \\
V_{eff}=V_{rms}
\end{align}
$$
For the sinusoid $i(t)=I_{m}\cos(\omega t)$ the effective RMS value is:
$$
\begin{align}
I_{rms}=\sqrt{ \frac{1}{T} \int _{0}^T I_{m}^2\cos^2(\omega t) dt  } \\
= \sqrt{ I_{m}^2\int 0T \frac{1}{2}(1+\cos(2\omega t))  \, dt = \frac{I_{m}}{\sqrt{ 2 }}  }
\end{align}
$$

[[Average Power Transfer]]