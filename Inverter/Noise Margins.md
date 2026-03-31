---
tags:
  - ECE_571
  - lecture_4
---
It is important to know the allowable voltage range on the input such that the output is not corrupted 

- Define NML as the LOW noise margin
	- Difference between maximum LOW input voltage and the maximum LOW output voltage produced by a driving gate 
	- $NML=VIL-VOL$

- Define NMH as the HIGH noise margin
	- Difference between minimum HIGH output voltage produced by a driving gate and the minimum HIGH input voltage 
	- $NMH=VOH-VIH$



![[Noise Margins.png]]


- Want noise margins as large as possible 
	- Want the forbidden zone to be small
	- Want the difference between VIL and VIH to be small
	- Want these centered on the midpoint between VOH and VOL
	- Want a high gain in the transition region between VOH and VOL

- Typically use unity gain points to define our logic levels 
	- Where slope of transfer curve is -1