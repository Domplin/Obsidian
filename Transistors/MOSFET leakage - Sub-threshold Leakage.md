---
tags:
  - ECE_564
  - Lecture_2
aliases:
  - sub-threshold leakage
---
	
Sub-threshold leakage (or conduction) is the unwanted, exponential current ($I_{sub}$) flowing between source and drain when a MOSFET is "off" ($V_{GS}<V_{th}$) primarily due to carrier diffusion rather than drift. It is a major component of static power dissipation.


![[MOSFET leakage - Sub-threshold Leakage.png]]
- *Key factors being*:
	- **[[Sub-threshold Swing]] (or Leakage)**: $I_{sub}$ - Current flowing from drain to source due to carrier diffusion when the gate voltage is below threshold 
	- **[[Junction Leakage]]**: $I_{j}$ - Reverse-bias PN junction current between the source/drain and the substrate (minority carrier diffusion/drift)
	- **[[Gate Leakage]]**: $I_{\text{gate}}$ - Current tunneling through the thin gate oxide (increases exponentially as oxide get thinner)
	- **[[Drain Induced Barrier Lowering]]**: $I_{DIBL}$ - High drain voltage reduced the  source-channel potential barrier
	- **[[Gate-Induced Drain Leakage]]**: $I_{GIDL}$ - Current created by high fields in the drain-gate overlap region.
	- **[[Punch Through Leakage]]**: $I_{punch}$ - Current created by high fields in the drain-gate overlap region


**There are ways to stop leakage**: [[Countering Leakage]]


**Linear Scale**
![[MOSFET leakage - Sub-threshold Leakage - Linear Scale.png]]


**Log-scale**
![[MOSFET leakage - Sub-threshold Leakage - Log scale.png]]


At sub-threshold - oxide capacitor ($C_{ox}$) comes in series with channel depletion capacitor ($C_{D}$) 

$$
I_{\text{sub}}=I_{0}e^{\frac{q(V_{GS}-V_{th})}{mk_{b}T}}
$$
$$
V_{GS}=\psi_{s}+V_{ox}
$$
- $\psi_{s}$ = surface potential 
$$
\psi_{s}=V_{GS} \times \frac{C_{ox}}{C_{ox}+C_{D}}= \frac{V_{GS}}{m}
$$
$$
m=1+\frac{C_{D}}{C_{ox}}=1+ \frac{\frac{\epsilon_{Si}}{W_{D}}}{\frac{\epsilon_{ox}}{t_{ox}}}=1+\frac{3t_{ox}}{W_{D}}
$$
- It can be noted from the preceding expression that $m$ can be made smaller by using a thinner oxide (insulator) layer to reduce or a lower substrate doping concentration (resulting in larger $W_{D}$)
- 