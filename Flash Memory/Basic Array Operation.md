---
tags:
  - ECE_564
  - Lecture_13
---
**How to update / erase a page** ([[NAND Array Structure]])
1) Copy valid page data
2) Block erase 
![[Basic Array Operation.png]]

*System level issues for page update*:
- Write only works on erased page
- [[In-place update]] of a page is not available 
- Erase operation cannot be don on a single page




**Read Operation**: Array biasing scheme
- Read 1 page at a time ([[NAND Array Structure]])
- Cell Bias Condition
	- conducting = 1
	- not conducting = 0
- All the cells connected to a given word line are read simultaneously
- Pass voltages need to be higher than the highest cell threshold voltage 



**Page program operation**
- All the cells connected to a given word line are programmed simultaneously 
- All unselected word lines are biased with $V_{pass}$ voltage
- High bit line voltage is used to pre-charge the NAND string to prevent programming (Self-boosting)
![[Basic Array Operation - Page program operation.png]]

- Challenges in programming:
	- Precise control of $V_{th}$ placement 
	- Avoid over-programming
	- Maintain tight distribution of MLC/TLC/QLC ([[Multi-Level Cell]])

		To address these challenges, NAND flash uses the [[Incremental Step Pulse Programming (ISPP)]] algorithm 