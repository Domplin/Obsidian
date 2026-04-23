---
tags:
  - ECE_564
  - lecture_10
---


**Question:** How many electrons need to be injection on FG to make $V_{T}$ (prog) = 1V
- Assume - $V_{T}$ (erase) = 0V, $t_{tox}$ = 8nm, $t_{box}$ = 16nm, Gate Area = 20mn x 20mn'
- *note*: $\epsilon_{Si 02}$ = $3.9 \epsilon_0=3.9 \times 8.8 \times 10^{-14}$ F/cm
	- Charge of an electron: $|q|=1.6 \times 10^{-19}$ C
	- 1 nm = $10^{-9}m=10^{-7}cm$ 



**Solution**:
##
$$
\Delta V_{T}= \frac{\Delta Q_{FG}}{C_{box}}
$$
$$
C_{box}=\frac{A\epsilon_{sio_{2}}}{t_{box}}= \frac{400 \times 10^{-14} \times 3.9 \times 8.8 \times 10^{-14}}{16 \times 10^{-7}}=8.6 \times 10^{-19}F
$$


$$
\Delta Q_{FG}= \Delta V_{T} \times C_{box} = 8.6 \times 10^{-19}C
$$

$$
\text{Number of Electrons = } \frac{8.6\times10^{-19}}{1.6\times10^{-19}}\approx 5

$$

###



[[Random Telegraph Noise (RTN)]]
**Question**: What is the $\Delta V_{T}$ for single electron de-trapping
- Assume - 20nm tech node, $t_{tox}=$ 7mn, Coupling ratio, $\alpha=0.65$ 
$$
\Delta V_{T} = \frac{|q|}{C_{box}} \propto \frac{1}{A}
$$
Gate area shrinks with technology scaling


**Solution**
##
$$
C_{ox}= \frac{A\epsilon_{sio_{2}}}{t_{ox}}= \frac{20^2 \times 10^{-14}\times 3.9 \times 8.8 \times 10^{-14}}{7 \times 10^{-7}}=19.6\times 10^{-19}F
$$

$$
C_{box}= C_{ox} \times \frac{\alpha}{1-\alpha}=19.6 \times 10^{-19} \times \frac{0.65}{0.35}=36.4 \times 10^{-19}F
$$
$$
\Delta V_{T}= \frac{1.6\times 10^{-19}}{36.4 \times 10^{-19}}=44mV
$$
