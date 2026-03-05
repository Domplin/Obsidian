$$
\text{CPU Time} = \text{CPU Clock Cycles}*\text{Clock Cycle Time}=\frac{\text{CPU Clock Cycles}}{\text{Clock Rate}}
$$
- *CPU performance improved by:*
	- Reducing the number of clock cycles 
	- Increasing clock rate

- Hardware designer must often trade off clock rate against cycle count
	- almost all techniques that decrease the number of clock cycles also decrease the clock rate




**CPU Time Example:**
- A program runs on computer A with a 2 GHz clock in 10 seconds
- What clock rate must computer B run at to run this program in 6 seconds?
	- *Caveat*: to accomplish this, computer B will require 1.2 times as many clock cycles as computer A to run the program

$$
\begin{align}
\text{Clock Rate}_{B} = \frac{\text{Clock Cycles}_{B}}{\text{CPU Time}_{B}}=\frac{1.2*\text{Clock Cycles}_{A}}{6s}  \\
\text{Clock Rate}_{A} = \text{CPU Time}_{A}*\text{Clock Rate}_{A} \\
\text{Clock Rate}_{B} = \frac{1.2*20*10^9}{6s}=\frac{24*10^9}{6s}=4\text{GHz} 
\end{align}
$$
**In general you cannot expect performance to double just by doubling clock frequency**
