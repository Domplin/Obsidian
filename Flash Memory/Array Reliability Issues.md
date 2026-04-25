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
- Leakage currents in the row decoder can degrade the boosted wordline potential, resulting in a soft erase on the programmed cells in the unselected blocks
- Like in the [[Self-boosting]] program inhibit where the isolated NAND string is boosted by raising the word lines to high voltages, wordlines can be boosted to high voltages by the ramped potential of the shared p-well 
- The electrically isolated wordlines of the uns