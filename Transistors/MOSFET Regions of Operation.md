---
tags:
  - ECE_571
  - Lecture_2
  - Equations
---

**Cutoff region**: 
$$
\begin{align}
V_{GS}=0V \\
(V_{GB}=V_{GS}): Ids=0 -\text{No Channel}
\\
 \\
0<V_{GS}<V_{T}:Ids = 0-\text{No chennel depletion region forming}
\end{align}
$$

**Linear / Triode region**
- $V_{GS}=V_{T}$ 
- $V_{GD}=V_{GS}$
- $V_{DS}=0$
- $Ids=0$
- n-Channel formed 

- $V_{GS}>V_{T}$
- $V_{GS}>V_{GD}>V_{T}$
- $0<V_{DS}<V_{GS}-V_{T}$
- $I_{dS}>0$ - Increases linearly with $V_{DS}$ when $V_{DS}$ close to 0
- Also called the "Ohmic" region

**Saturation Region**
- $V_{GS}>V_{T}$
- $V_{GD}<V_{T}$
- $V_{DS}>V_{GS}-V_{T}$
- Channel pinched off 
- $I_{DS}$ independent of $V_{DS}$ (ideally)


**Ideal Linear/Triode Region Equations**
$$
I_{DS}=\beta\left[ (V_{GS}-V_{T})V_{DS}-\frac{V_{DS}}{2}^2 \right]
$$
$$
\beta=\frac{\mu \epsilon_{ox}}{t_{ox}}\left( \frac{W}{L} \right)
$$
- $\mu$ - Carrier mobility
- $\epsilon_{ox}$ - Permittivity of gate oxide layer
- $t_{ox}$ - Thickness of gate oxide layer
- 