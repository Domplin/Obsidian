---
tags:
  - lecture_4
  - ECE_571
---
The concept of [[Beta Ratios]] can be applied to gates more complex than an inverters.

- To calculate the effective beta ratio, the gate needs to be transformed into an inverter
- For each input the worse case equivalent inverter by assuming a minimum  number of other inputs are set to sensitize the path 

This needs to be done for pull-up and pull-down paths separately 
- Remove all FETs of critical paths for the input
	- **NOTE**: Always select FETs with the lowest W when there is a choice
- Replace series FETs of $W_{1}$ and $W_{2}$ with a single FET of $W=\frac{1}{\frac{1}{W_{1}}+\frac{1}{W2}}$
- Replace parallel FETs of $W_{1}$ and $W_{2}$ with a single FET of $MIN(W_{1},W_{2})$ 



**Equivalent Inverter Example**
![[Skewed Logic Gates Example 1.png]]

- For path A $B_{p}$ and $C_{n}$ are ignored removing them
- Pull up network:
$$
A_{p}=\frac{1}{\frac{1}{4}+\frac{1}{4}}=2
$$
- Pull down  network:
$$
A_{}
$$