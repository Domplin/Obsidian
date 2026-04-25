---
tags:
  - ECE_564
  - Lecture_15
---
- Flash-Cosmos enables
	- Computation on multiple operands with a single sensing operation
	- Accurate computation results by eliminated raw bit errors in stored data

**Multi-Wordline Sensing (MWS)**: Bitwise AND
- Intra-Block MWS
	- Simultaneously activates multiple WLs in the same block
		- Bitwise AND of the stored data in the WLs
![[In-FLASH bulk bitwise computing - MWS.png]]
- A bitline only reads as '1' when all the target cells store '1'
	- Equivalent to the bitwise AND of all the target cells

**Multi-Wordline Sensing (MWS)**: Bitwise OR
- Inter-Block MWS 
	- Simultaneously activates multiple WLs in different blocks
		- Bitwise OR of the stored data in the WLs
![[In-FLASH bulk bitwise computing - MWS OR.png]]
- A bitline reads as '0' only when all the target cells store '0'
	- Equivalent to the bitwise OR of all the target cells


**Bitwise AND operation** - With [[Multi-Level Cell]]s
![[In-FLASH bulk bitwise computing - MLC AND.png]]
*Result*: A AND B by LSB page read
Steps:
1) Operand A, B stored in LSB, MSB Page
2) Shift the $V_{ref1}$ with specific offset (Read  re)