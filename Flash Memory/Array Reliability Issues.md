---
tags:
  - ECE_564
  - Lecture_14
---
**Read Disturb**
- Increasing Vread $\rightarrow$ soft program occurs in the unselected cell of selected string
- Unselected wordlines have Vread applied to CG
- Selected wordline has Vref applied to CG
- Applied voltages cause unintended tunneling of charge
- Since Vref < Vpass, unselected wordlines are most severely affected 

	*Read Disturb - Signatures*:
	- Large number of reads (> 1 million) are required to cause disturb 
	- Most of the read disturb effects are observed on the erased memory cells
	- Program states not affected much

**Erase Disturb**
- Erase disturb, unlike the program disturb, is not usually a large issue in NAND flash.
- Since the erase operation affects all cells located in one block at the same time, there is no relevant intra-block interference 
- Leakage 