---
tags:
  - ECE_571
  - lecture_4
---
- Already seen that for an unskewed inverter ([[Skewed Logic Gates]]) the [[Beta Ratios]] is 1
- Therefore the $\beta$ for both P and N devices are the same 
- Recall: $\beta= \frac{\mu \epsilon_{ox}}{t_{ox}}$ 
- Recall: $\mu_{n}>\mu_{p}$
- If drawing minimum length FETs, this implies the widths of the nFET and pFET of the inverter must not be the same
$$
\frac{W_{p}}{W_{n}}=\frac{\mu_{n}}{\mu_{p}}
$$
- For example $\mu_{n}=2\mu_{p}$, $W_{p}=2W_{n}$ for an unskewed inverter
	- This is where the 2:1 ratio between pFET and nFET sizes that have been illustrated come from 



**NAND FET Sizes**
- The process used to find [[Equivalent Inverter]]s is essentially reversed to size the FETs in more complex gates
- Assume there is a 2-input NAND gate that needs the same drive strength as the "2-over-1" inverter.
- The nFET needs to be 2 X-wide to pull down the output, Q, with the same strength as the 1-wide nFET in the inverter 
	- Two X-wide saturated FETs of length L in series are equivalent to a single FET of width X and length 2L
	- Two X-wide FETs in series are equivalent to single X/2-wide FET
	- In general, n X-wide FETs in series are equivalent to a single X/n-wide FET
- Since the pull-down chain needs to have the same drive strength of the 1-wide nFET of the inverter: X=2