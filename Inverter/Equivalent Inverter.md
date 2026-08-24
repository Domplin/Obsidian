
The concept of [[Beta Ratios|beta ratios]] can be applied to gets more complex than inverters. To calculate the effective beta ratio, we need to transform a gate into an inverter. 

For each input we can find the worst case equivalent inverter by assuming a minimum number of other inputs are set to set to sensitize the path

This needs to be done for pull up and pull down paths separately 
- Remove all FETs of $W_{1}$ and $W_{2}$ with a single FET of $W=\frac{1}{\frac{1}{W_{1}}+\frac{1}{W_{2}}}$ 
- Replace parallel FETs of $W_{1}$ and $W_{2}$ with a single FET of $W=MIN(W_{1},W_{2})$ 


![[Equivalent Inverter - Example 1.png]]


![[Equivalent Inverter - Example 2.png]]