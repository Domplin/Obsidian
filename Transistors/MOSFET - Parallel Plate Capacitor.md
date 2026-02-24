---
tags:
  - ECE_564
  - Lecture_1
  - Equations
---


![[MOSFET - Parallel Plate Capacitor.png]]


- The gate and the channel region of the MOSFET form a *parallel-plate capacitor* with the oxide layer acting as the capacitor dielectric
- The positive gate voltage causes positive charge to accumulate on the top plate of the capacitor (*The gate electrode*) 
- The corresponding negative charge on the bottom plate is formed by *the electrons in the induced channel* [[MOSFET - Current Flow]]
- An electric field thus develops in the vertical direction. The vertical electric field controls the channel charge, and thus its conductivity and current when $v_{DS}$ is applied
	- Hence the name *field-effect transistor of FET* 



$$
\begin{align}
Q=CV  \\
C=\frac{\epsilon_{ox}A}{d}\text{F} \\
|Q| = CV_{OV}=C_{ox}(WL)V_{OV} \\
C_{ox}= \frac{\epsilon_{ox}}{t_{ox}} \frac{F}{cm^2}
\end{align}
$$
$\epsilon_{ox}=3.9_{\epsilon_{0}}=3.9 \times 8.85 x 10^{-14} \frac{F}{cm}$
