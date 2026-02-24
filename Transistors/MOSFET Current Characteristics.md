---
tags:
  - ECE_564
  - Equations
  - Lecture_1
---
- [[MOSFET - Current Flow]]
- [[Current Voltage For high V]]
- [[MOSFET - Current Flow for small V]]
- [[MOSFET - Parallel Plate Capacitor]]


Given the two possibilities of *high* $V_{DS}$ and *low* $V_{DS}$ there are two regions for a MOSFET to operate in:
- **Triode**: $V_{DS} <V_{OV}$ - [[Threshold and Overdrive Voltage|Overdrive Voltage]]
	- Gate controlled resistor 
	- $I = \mu C_{ox}\left( \frac{W}{L} \right)V_{OV} \times V_{DS}$

- **Saturation**: $V_{DS} > V_{OV}$ 
	- Gate controlled current source 
	- $I= \mu_{n} C_{ox}\left( \frac{W}{2L} \right)V_{OV}^2$
![[MOSFET Current Characteristics graph.png]]![[MOSFET Current Characteristics.png]]


![[MOSFET Current Characteristics Summary.png]]
