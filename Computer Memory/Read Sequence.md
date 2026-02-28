
1) Pre-charge the bit lines
	- The pre-charge and equalization circuit is activated by raising the control signal $\Phi_{p}$
	- This will cause the $BL$ and $\overline{BL}$ lines to be at equal voltages - equal to $\frac{V_{DD}}{2}$ 
	- The clock $\Phi_{P}$ then goes low and the $BL$ and $\overline{BL}$ lines are left to float for a brief interval 

2) Word Line activated
	- The word line goes up, connecting the cell to the $BL$ and $\overline{BL}$ 
	- A voltage then develops between $BL$ and $\overline{BL}$ with $V_{BL}$ higher than $V_{\overline{BL}}$ if the accessed cell is storing a 1 or $V_{\overline{BL}}$ higher than $V_{BL}$ is the cell is storing a 0.
	- To keep the cell area small and to facilitate operation at higher speeds, the readout signal which the line is required to provide between $BL$ and $\overline{BL}$, is kept small (usually 20-500 mV)
3) Sense amplifier activated
	- Once an adequate difference voltage signal between B and B has been developed by the storage cell, the sense amplifier is turned on by connected it to ground and $V_{DD}$ through $Q_{5}$ and $Q_{6}$, activated by raising the sense control signal $\Phi_{s}$ 

![[Read Sequence.png]]
