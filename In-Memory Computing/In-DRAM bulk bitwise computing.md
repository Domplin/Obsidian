---
tags:
  - ECE_564
  - Lecture_15
---
Data movement from memory/storage to processor significantly bottlenecks performance and energy efficiency

![[In-DRAM bulk bitwise computing - State transitions.png]]

*Simplified DRAM read operations*:
1) Precharge: bitline (BL) and $\bar{BL}$ are set to $\frac{V_{DD}}{2}$ - wordline and sense amplifier are off
2) Activate: Wordline is raised, connecting the cell capacitor to the bitline
3) Charge Sharing: Charge flows from the capacitor to the bitline, slightly changing its voltage
4) Sensing: The sense amplifier detects and amplifies the sa