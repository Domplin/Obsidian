---
tags:
  - ECE_564
  - Lecture_1
  - Equations
---
- Having induced a channel, if a positive voltage is applied $V_{DG}>0$ between drain and source, a drain current is $I_{D}$ starts to flow 
- Currents carried by free electrons traveling from source to drain 
	- By convention the direction of the current flow is opposite to that of the flow of negative charge
- First consider the case where $V_{DS}$ is small (*50mV or so*) 
	- The effective voltage between the gate and the various points along the channel remains equal to $V_{OV}$ ([[Threshold and Overdrive Voltage]]) and the channel charge *Q per unit length* is still given by
$$
I = Q \times V_{\text{drift}}
$$
$$
V_{\text{drift }}= \mu_{n} E_{\text{field}} \text{ and } E_{\text{field}}= \frac{V_{DS}}{L}
$$
	$\mu_{n} =$ Electron mobility in silicone
![[MOSFET - Current Flow for small V.png]]

Therefore for small $V_{DS}$ the channel behaves as a linear resistance controlled by the gate overdrive voltage $V_{OV}$ ([[Threshold and Overdrive Voltage]])

