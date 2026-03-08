---
tags:
  - ECE_571
  - lecture_4
---
What happens when $\beta_{n} \neq \beta_{p}$ $\Rightarrow$ It makes a "skewed" inverter
[[HI and LO-Skew]]


$$
r = \frac{\beta_{p}}{\beta_{n}}
$$

**Ideal:**
$$
V_{inv}= \frac{V_{DD}+V_{Tp}+V_{Tn}\sqrt{ \frac{1}{r} }}{1+\sqrt{ \frac{1}{r} }}
$$

**Velocity Saturated**
$$
V_{inv}=\frac{V_{DD}+V_{Tp}+V_{Tn} \frac{1}{r}}{1+\frac{1}{r}}
$$



**$\beta$ in VLSI CMOS** 
- The beta ration in CMOS is determined completely by the mobilities ($\mu_{n},\mu_{p}$) and the aspect ratios (W/L) of the FETs
- This is because $C_{ox}$ can be assumed ot 