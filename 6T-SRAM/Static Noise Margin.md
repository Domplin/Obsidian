---
tags:
  - ECE_564
  - Lecture_5
aliases:
  - SNM
---
![[Static Noise Margin.png]]

- Destructive read problem
- The size of the squares between the butterfly curves  = static noise margin



**Increasing Read Margin**:
- By increasing the size of the driver [[NMOS vs PMOS|NMOS]] improves the read margin
- Area is the number 1 constraint in memory design  
	- Increasing cell size is not a good trade off


- Boosted cell supply
	- Supply voltage of SRAM cell is higher than outside 
	- Makes driver stronger than access suppressing the rise in the low side
	- Effectively improves the beta ratio
	- Driver [[NMOS vs PMOS|NMOS]] can be downsized decreasing cell size 


- High $V_{t}$ transistors 
	- 