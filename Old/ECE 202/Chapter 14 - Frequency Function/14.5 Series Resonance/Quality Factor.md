The “Sharpness” of the resonance in a resonant circuit is measured quantitatively by the **quality factor** $Q$. At resonance, the reactive energy in the circuit oscillates between the inductor and the capacitor. The quality factor relates the maximum or peak energy stores to the energy dissipated in the circuit per cycle of oscillation.

**Note**: Although the same symbol is used for the reactive power, the two are not equal and should not be confused. $Q$ here is dimensionless, where as reactive power $Q$ is in VAR.

$$
Q=2\pi  \frac{\text{ Peak Energy Stored in the Circuit}}{\text{Energy dissipated by the Circuit}} \text{ *in one period at resonance}

$$

Its also regarded as a measure of the energy storage property of a circuit in relation to its energy dissipation property. In the series [[Series RLC Circuit]] the peak energy stored is $\frac{1}{2}LI^2$ while the energy dissipated on one period is $\frac{1}{2}(I^2R)\left( \frac{1}{f_{0}} \right)$:
$$
Q=2\pi   \frac{\frac{1}{2}LI^2}{\frac{1}{2}I^2R\left( \frac{1}{f_{0}} \right)}= \frac{2\pi f_{0}L}{R}
$$
$$
Q=\frac{\omega_{0}L}{R}=\frac{1}{\omega_{0}CR}
$$


Notice that the quality factor is dimensionless. The relationship between the bandwidth $B$ and the quality factor $Q$ is obtained by substituting:
$$
B=\frac{R}{R}=\frac{\omega_{0}}{Q}
$$
Or
$$
B=\omega_{0}^2CR
$$

The **Quality Factor** of a resonant circuit is the ratio of its resonant frequency to its bandwidth

The **Quality Factor** is a measure of the selectivity (or “sharpness” of resonance) of the circuit

![[Pasted image 20240329130832.png]]
As illustrated the higher the value of $Q$, the more selective the circuit is but smaller the bandwidth. The *selectivity* of an [[Series RLC Circuit]] is the ability of the circuit to respond to a certain frequency and discriminate again all other frequencies 