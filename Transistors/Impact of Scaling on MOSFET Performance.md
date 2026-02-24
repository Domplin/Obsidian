---
tags:
  - ECE_564
  - Equations
  - Lecture_1
---

What happens to the MOSFET $V_{th}$ $I_{DS}$ from [[Dennard's Scaling Rules|Dennard Scaling]]

[[Dennard's Scaling Rules]]:
$\hat{W}= \frac{W}{x}$ 
$\hat{L}=\frac{L}{x}$ 
$\hat{N}_{d}=N_{D}x$
$\hat{V_{DD}}=\frac{V_{DD}}{x}$
$C_{g}=\frac{\epsilon_{OX}WL}{t_{ox}}$
$\frac{\hat{C}_{G}}{C_{g}}=\frac{1}{x}$

$C_{ox} =$ Gate oxide capacitance per unit area $= \frac{\epsilon_{OX}}{t_{ox}}$

[[MOSFET - Parallel Plate Capacitor]] 

**How does the drain current scale**:

$$
\frac{\hat{I_{D}}}{I_{D}} = \frac{\frac{1}{2}\mu_{n}\hat{C_{ox}}\left( \frac{\hat{W}}{\hat{L}} \right)(\hat{V_{GS}}-\hat{V_{TH}})^2}{\frac{1}{2}\mu_{n}C_{ox}\left( \frac{W}{L} \right)(V_{GS-V_{TH}})^2}
$$

$\hat{C_{ox}}=xC_{ox}$             $\hat{V_{GS}}=\frac{V_{GS}}{x}$


**Scaling on CMOS Gate Delay**


![[Impact of Scaling on MOSFET Performance - Gate Delay.png]]
- Propagation delay (assume MOSFET acts like a constant current source): $t_{d}=\frac{Q}{I_{D}}=\frac{C_{Load} \times V_{DD}}{I_{D}}$
- When scaled gates become faster and can be operated with higher frequency:
	- $\hat{C_{L}} \rightarrow \frac{1}{x}C_{L}$   $\hat{V_{DD}} \rightarrow \frac{1}{x}V_{DD}$    $\hat{I_{D}} \rightarrow \frac{1}{x}I_{D}$ 
$$
\frac{\hat{t_{d}}}{t_{d}} \approx \frac{\frac{1}{x}\times \frac{1}{x}}{\frac{1}{x}}=\frac{1}{x}
$$


**Scaling on CMOS Power Dissipation**

![[Impact of Scaling on MOSFET Performance - Power dissipation.png]]

- Energy dissipation during pull-up or pull-down phase:
	- $E_{\text{diss}}=\frac{1}{2}CV_{DD}^2$
- Total Energy Dissipation during pull-up *and* pull-down phase:
	- $E_{\text{diss}} /\text{cycle}= CV_{DD}^2$
- If the inverter is switched at a frequency of *f Hz* - Power dissipation:
	- $P_{\text{diss}}=fCV_{DD}^2$
- Power dissipation per MOSFET scales as:
	- $\frac{\hat{P_{\text{diss}}}}{P_{\text{diss}}}= x\times \frac{1}{x} \times \frac{1}{x^2}= \frac{1}{x^2}$
- Power density: 
	- $D_{P}=\frac{P_{\text{diss}}}{\text{Area}}$
	- $\hat{D_{P}}=D_{P}$
	- **Power per unit area of the chip remains constant**

- $\hat{C_{L}} \rightarrow \frac{1}{x}C_{L}$   $\hat{V_{DD}} \rightarrow \frac{1}{x}V_{DD}$    $\hat{f}=xf$
