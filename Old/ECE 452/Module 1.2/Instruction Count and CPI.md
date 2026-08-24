**Recall:** [[CPU Time]]

$$
\begin{align}
\text{Clock Cycles}=\text{Instruction Count}*\text{Cycles Per Instruction} \\
\text{[[CPU Time]]}=\text{Instruction Count}*CPI*\text{Clock Cycle Time}  \\
= \frac{\text{Instruction Count}*\text{CPI}}{\text{Clock Rate}}
\end{align}
$$
- What Determines:
	- *Instruction Count for a program* 
		- Determined by program, ISA and compiler
	- *Average cycles per instruction (CPI)*
		- Determined by different CPU hardware
		- If different instruction have different CPI
			- Average CPI affected by instruction mix
	- *Clock Rate*
		- Determined by CPU hardware and process technology



**Performance is impacted by both HW and SW layers**



**CPI Example:** 
- CPU A: cycle time = 250ps, CPI = 2.0
- CPU B": cycle time = 500ps, CPI = 1.2
- Same ISA compiler
*which is faster and by how much*

$$
\text{CPU Time}_{A}=\text{Instruction Count}*\text{CPI}_{A}*\text{Cycle Time}_{A}
$$
$$
= I*2.0*250ps=I*500ps
$$


$$
\text{CPU Time}_{B}=\text{Instruction Count}*\text{CPI}_{B}*\text{Cycle Time}_{B}
$$
$$
=I*1.2*500ps = I*600ps
$$

$$
\frac{\text{CPU Time}_{B}}{\text{CPU Time}_{A}}= \frac{I*600ps}{I*500ps}=1.2
$$


*i.e.* → A is faster by 1.2 times 


**CPI in more detail**
- if different instruction classes (types) take different number of cycles 
$$
\text{Clock Cycles}= \sum^n_{i=1}(CPI_{i}*\text{Instruction Count})
$$
- Weighted average CPI
$$
\text{CPI}=\frac{\text{Clock Cycles}}{\text{Instruction Count}} = \sum^2_{i=1}\left( CPI_{i}*\frac{\text{Instruction Count}_{i}}{\text{Instruction Count}} \right)
$$



**CPI Example**
- Consider two different implementations, *M1* and *M2*, of the same instruction set. 
- There are three instructions (A, B, and C) in the instruction set.
- *M1* has a clock rate of 80 MHz 
- *M2* has a clock rate of 120 MHz

The average number of cycles for each instruction are as follows:
![[Pasted image 20250321163307.png]]

**(a)** calculate the average CPI for each machine, *M1* and *M2*

For *M1*
$$
\text{Clocks per instruction} = \left( \frac{50}{100} \right)*1+\left( \frac{30}{100} \right)*2+\left( \frac{20}{100} \right)*4 = 1.9
$$
For *M2*
$$
\text{Clocks per instruction}=\left( \frac{50}{100} \right)*2+\left( \frac{30}{100} \right)*3+\left( \frac{20}{100} \right)*4=2.7
$$


**(b)** Calculate the average MIPS ratings for each machine, *M1* and *M2* 

For *M1*
$$
\text{Average MIPS rating}= \frac{\text{Clock Rate}}{\text{CPI}*10^6}=\frac{80*10^6}{1.9*10^6}=42.10
$$
For *M2*
$$
\text{Average MIPS rating}=\frac{\text{clock Rate}}{\text{CPI}*10^6}=\frac{120*10^6}{2.7*10^6}=44.44
$$
**(c)** Which of the two (CPI or MIPS) is preferred for performance analysis and why?
	- CPI as MIPS is misleading and does not distinguish between instruction types, ISAs
	- MIPS is particularly misleading when used as a metric to compare different processors/implementations