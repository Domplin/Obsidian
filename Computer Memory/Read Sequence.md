
1) Pre-charge the bit lines
	- The pre-charge and equalization circuit is activated by raising the control signal $\Phi_{p}$
	- This will cause the $BL$ and $\overline{BL}$ lines to be at equal voltages - equal to $\frac{V_{DD}}{2}$ 
	- The clock $\Phi_{P}$ then goes low and the $BL$ and $\overline{BL}$ lines are left to float for a brief interval 

2) Word Line activated
	- The word line goes up, connecting the cell to the $BL$ and $\overline{BL}$ 
	- A voltage then develops between $BL$ and $\overline{BL}$ with $V_{BL}$ higher than $V_{\overline{}}$