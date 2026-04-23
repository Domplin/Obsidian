---
tags:
  - ECE_564
  - Lecture_11
---
 - Data retention refers to the ability of a NAND flash memory cell to maintain its stored charge (and therefore its threshold voltage state) over time without power 
 - Over time, stored charge gradually leaks away causing Vth drift, which can eventually lead to bit errors


![[Cell Reliability - Data Retention (DR).png]]


- The data retention of Flash technology makes it [[Volatility of Memory|non-volatile]] 
- Typically, 10 years of data retention is expected at room temperature


**Factors affecting data retention***
- Operating temperature
- Tunnel oxide quality and thickness
- Program Vth level 

Possible [[Charge Loss Pathways]]


**Data retention depends on cell usage**
- Fresh Cell:
	- The intrinsic retention is mainly limited by direct tunneling through tunnel oxide
	- Thermionic emission can take place at elevated temperatures

- Worn-out Cell:
	- Electrons stored in the oxides or interface traps are vulnerable and escape soon
	- Trap-assisted tunneling (TAT) also causes Charge loss


**Temperature Dependence of Retention**
	Retention loss is thermally activated. Leakage follows Arrhenius behavior:
	$$
	\text{Charge loss rate} \propto e^{-E_{a}/k_{B}T}
	$$
Accelerated Retention Test:
- 10-year retention at $30^{\degree}C$ may degrade to weeks at $125^{\degree}F$ 
*Acceleration Factor*: 
$$
A= \exp\left[ \frac{E_{a}}{k_{B}}\left( \frac{1}{T_{use}}-\frac{1}{T_{stress}} \right) \right]
$$


*Activation Energy*
- $E_{a}=1.1V$
- $T_{use}=\text{Room Temperature = 300k}$
- $T_{stress}=\text{High temperature}=393K$
- $k_{B}=\text{Boltzmann constant} = 8.167 \times 10^{-5}eV$ $K^{-1}$

You measure time for data corruption ($t_{meas}$=1hrs) at high temperature, $T_{stress}$ 

Convert the measured time for estimating the use time:
$$
t_{use}= A \times t_{meas}
$$
$$
A=\exp\left( \frac{1.1}{k_{B}}\left( \frac{1}{300}-\frac{1}{393} \right) \right)=23610
$$