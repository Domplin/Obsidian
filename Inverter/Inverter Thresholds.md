---
tags:
  - ECE_571
  - lecture_4
---
Threshold, $V_{inv}$ is where $V_{in}=V_{out}$

For simple inverter models, assume both FETs are saturated - solve for $V_{inv}$:

$$
I_{Dnsat}=-I_{Dpsat}
$$
$$
V_{Tn}=-V_{Tp}
$$
$$
\frac{\beta_{n}}{2}(V_{inv}-V_{Tn})^2=-\frac{\beta_{p}}{2}(V_{inv}-V_{DD}-V_{Tp})^2
$$
Giving $V_{inv}=\frac{V_{dd}}{2}$
