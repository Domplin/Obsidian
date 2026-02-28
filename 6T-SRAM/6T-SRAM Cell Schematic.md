---
tags:
  - ECE_564
  - Lecture_5
---
![[6T-SRAM Cell Schematic.png]]
![[6T-SRAM Cell Schematic - access transistor.png]]

- **Access Transistors** facilitate Read/Write operation 
- Read/Write uses the same port - Need enough of a margin to prevent disturbances 
- One Word line (WL) to access cell
- Two bit lines ($BL$ and $\overline{BL}$) to carry data

*NOTE:* $C_{BL}$ and $C_{Q}$ are intrinsic capacitance and they are not physically connected separate capacitors - Bit line capacitance are significantly higher than the cell capacitance or $B_{BL}\gg C_{Q}$  