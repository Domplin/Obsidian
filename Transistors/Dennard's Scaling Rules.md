---
tags:
  - ECE_564
  - Lecture_1
aliases:
  - Dennard Scaling
---

**Problem with scaled MOSFET**
![[Dennard's Scaling Rules - Problem with scaled MOSFET.png]]

- If a transistor gate length is made for a factor of K (say $K=5$) times smaller, then the depletion regions around the source and the drain would touch
	- There would be no conduction channel and therefore no transistor operation
- Additionally - reducing the channel length by 5x increases the electric field by a factor of 5 
	- High electric fields cause the transistor and its associated semiconductor junctions to break down and get damaged 



![[Dennard's Scaling Rules.png|1525]]
**Scaling Rules**
1) *Dimensions*: Scale down all linear dimensions by a factor of *x* - When the gate length is reduced by *x*, the gate oxide thickness, implanted source/drain depth and transistor width should all be reduced by the same factor 
2) *Voltage*: Reduce the voltage applied to the device by a factor of *x* - If the voltage is reduced as the dimensions shrink, then the electric field can be kept constant. The threshold voltage also scales by a factor of *x* when the gate oxide thickness is scaled down so that the transistor operates at reduced drain voltages
3) *Doping*: Increase body doping concentration by a factor of *x*. By increasing the substrate doping, the depletion width can be reduced by the same factor which is important to keep them from touching the other 


**Summary**
Dennard's law, states that as transistors in a semiconductor chip get smaller, they get faster while power density remains constant 

- *Key points*
	- *Constant power density*: The core concept is that as transistors shrink their power density remains the same, enabling increased performance per unit area 
	- *Scaling voltage and current*: To maintain constant power density, both the operation voltage and current need to be scaled down proportionally with the transistor size
	- *Impact on chip design*: This law allowed chips designers to increase clock speed significantly without major power concerns, driving rapid advancements in processor performance.


- *Limitations and breakdowns of Dennard scaling*
	- *Physical limits*: As transistors became extremely small, physical effects like leakage current and short-channel effects started to increase power consumption - causing Dennard scaling to breakdown
	- *End of scaling era*: Around the mid-2000s, the industry reached a point where further scaling down voltage without significant performance penalties became difficult, leading to a shift towards multi-core architectures to maintain performance gains. 