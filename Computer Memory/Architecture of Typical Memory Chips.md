---
tags:
  - ECE_564
  - lecture_4
---
- **Data Lines**: 
	- $m$-bits in parallel - typically $m=8,16$ 
- **Address Lines**: 
	- $L$ address lines $\rightarrow N=2^L$ addresses
- **Control Lines**: 
	- Write enable (WE): When activated values on data lines are written to the specified addresses
	- Output enable (OE): data at a specified memory location is placed on the I/O pins
	- Chip select (CS): Selects a specific chip in an array of memory chips 
![[Architecture of Typical Memory Chips.png]]