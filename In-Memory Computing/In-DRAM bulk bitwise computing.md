---
tags:
  - ECE_564
  - Lecture_15
---
Data movement from memory/storage to processor significantly bottlenecks performance and energy efficiency

![[In-DRAM bulk bitwise computing - State transitions.png]]
$$
\delta=\frac{C_{s}}{C_{BL}+C_{s}}\left( \frac{V_{DD}}{2} \right)
$$
*Simplified DRAM read operations*:
1) Precharge: bitline (BL) and $\bar{BL}$ are set to $\frac{V_{DD}}{2}$ - wordline and sense amplifier are off
2) Activate: Wordline is raised, connecting the cell capacitor to the bitline
3) Charge Sharing: Charge flows from the capacitor to the bitline, slightly changing its voltage
4) Sensing: The sense amplifier detects and amplifies the small voltage difference 
5) Restore: The original charge is restored in the cell, completing the read operation



**AND/OR: Triple Row Activation**
![[In-DRAM bulk bitwise computing - ANDOR.png]]

Final State:
$$
AB+BC+AC=C(A+B)+\bar{C}(AB)
$$
- Bitwise AND: C = 0
- Bitwise OR: C = 1

Final state of the bitline to be $V_{DD}$ if at lease two of the three cells are initially fully charged, and the final state to be 0, if at two of the three cells are initially fully empty


**Charge Sharing Ca**