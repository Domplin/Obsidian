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
![[Flash Memory/images/Multi-Level Cell.png|272]]
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
![[Multi-Level Cell.png]]

- Endurance: $5000-10,000$ cycles
- Data retention: $3-10$ years
- Read Latency: $25-37\mu s$
- Program Latency: $600-1800\mu s$

*MLC page read*
- LSB page read: 
	- The Data "1 1 0 0" (LSB page) is written, and a single sense amplifier read operation can verify if the cells are in one of two voltage ranges 
- MSB page read:
	- Decoding MSB page requires two sensing operations using two different read reference voltages.
	- During first sensing ($V_{ref{0}}$ ) only cell 0 is decoded as "1" (conducting)
	- During second sensing ($V_{ref 2}$) 
