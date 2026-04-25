---
tags:
  - ECE_564
  - Lecture_13
---
**Logical Scaling**
- SLC - Single level cell
- MLC - Multi level cell
- TLC - Triple level cell



**Logical Page Structure in SLC Storage**
![[Multi-Level Cell.png|272]]
![[Multi-Level Cell-1.png|404]]
![[Multi-Level Cell-2.png|403]]

- Endurance: $100,000$ cycles
- Data Retention: 10 years
- Read Latency: 25 $\mu s$
- Program latency: $100-200\mu s$


**Multi-Level Cell**
- The read time depends on the bit being read from
	- The least significant bit (LSB) is the fastest - only one sense operation is required 
	- The most significant bit (MSB) is the slowest - two sense amps are needed 