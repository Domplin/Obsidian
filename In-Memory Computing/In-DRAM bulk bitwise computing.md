---
tags:
  - ECE_564
  - Lecture_15
---
Data movement from memory/storage to processor significantly bottlenecks performance and energy efficiency

![[In-DRAM bulk bitwise computing - State transitions.png]]
$$
\delta=\frac{C_{s}}{C_{BL}+C_{s}}\left( \frac{V_{DD}}{2} \right)
$$
*Simplified [[DRAM]] read operations*:
1) Precharge: bitline (BL) and $\bar{BL}$ are set to $\frac{V_{DD}}{2}$ - wordline and sense amplifier are off
2) Activate: Wordline is raised, connecting the cell capacitor to the bitline
3) Charge Sharing: Charge flows from the capacitor to the bitline, slightly changing its voltage
4) Sensing: The sense amplifier detects and amplifies the small voltage difference 
5) Restore: The original charge is restored in the cell, completing the read operation



**AND/OR: Triple Row Activation**
![[In-DRAM bulk bitwise computing - ANDOR.png]]

Final State:
$$
AB+BC+AC=C(A+B)+\bar{C}(AB)
$$
- Bitwise AND: C = 0
- Bitwise OR: C = 1

Final state of the bitline to be $V_{DD}$ if at lease two of the three cells are initially fully charged, and the final state to be 0, if at two of the three cells are initially fully empty


**Charge Sharing Calculation**
![[In-DRAM bulk bitwise computing - charge sharing calculation.png]]

$$
\text{If } \delta > 0:BL \rightarrow V_{DD}
$$
$$
\text{If }\delta < 0: BL \rightarrow 0V
$$
Initial charge (before sensing) = Final charge (After sensing)
$$
\left( kC_{S}V_{DD}+C_{BL} \frac{V_{DD}}{2} \right)=(3C_{S}+C_{BL})\left( \frac{V_{DD}}{2}+\delta \right)
$$
$$
\delta= \frac{kC_{s}CV_{DD}+C_{BL}(V_{DD}/2)}{3C_{S}+C_{BL}}-\frac{V_{DD}}{2}=\frac{(2k-3)C_{s}}{6C_{s}+2C_{BL}}V_{DD}

$$
**Limitations of triple row activation (TRA)**
1) Weak sensing signal: Activating three cells reduces the voltage difference on the bitline, which can slow sensing or cause errors
2) Process variation: Real cells have unequal capacitance and non-ideal behavior, affecting reliability
3) Data destruction: TRA overwrites all three source cells, losing original data
4) Charge leakage: Partially leaked cells may lead to incorrect results
5) High hardware cost: requires simultaneous decoding of three rows, increasing controller and decoder complexity



**Ambit-AND-OR**
- Ambit reserves a set of designated rows in each subarray that are used to perform TRAs
	- These designated rows are chosen statically at design time
- To perform a bulk bitwise AND or OR operation on two arbitrary source rows, out mechanism first copies the data of the source rows into the designated rows and performs the required TRA on the designated rows

*As an example, to perform a bitwise AND/OR of two rows A and B, and store the result in row R, our mechanism performs the following steps*
1) Copy data of row A to designated row T0
2) Copy data of row B to designated row T1
3) Initialize designated row T2 to 0
4) Activate designated rows T0, T1, and T2 simultaneously 
5) Copy data of row T0 to row R