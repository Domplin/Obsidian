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

**Multi-Wordlin**