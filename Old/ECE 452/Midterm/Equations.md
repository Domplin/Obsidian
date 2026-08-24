
**Performance & Timing Equations**

*Execution Time*
- $\text{[[CPU Time]]} = \frac{\text{Instructions}*\text{CPI}}{\text{Clock Rate}}$
- $\text{CPU Time} = \text{Clock Cycles}*\text{Cycle Time}$

*Performance*
- $\text{Performance}=\frac{1}{\text{CPU Time}}$
	- Larger number is better

*Clock Cycles*
- $\text{Clock Cycles}=\sum(\text{Instruction Count}*\text{CPI})$

*Global CPI*
- $\text{Global CPI}=\frac{\text{Total Clock Cycles}}{\text{Total Instruction Time}}$
- $\text{CPI}=\frac{\text{Execution Time}}{\text{Instruction Count}*\text{Cycle Time}}$

*MIPS*
- $\text{MIPS}=\frac{\text{Clock Rate}}{\text{CPI}*10^6}$

*MFLOPS*
- $\text{MFLOPS}=\frac{\text{Floating Point Instructions}}{\text{Execution Time}*10^6}$
- $\text{Floating Point Instructions}=\text{Total Instructions}*\text{FP Instruction Ratio}$


**Multi [[Processor Performance]]**
*Ideal Time per Processor*
- $t_{p}=\frac{t}{p}$

*total time with constant overhead*
- $T_{total}=\frac{t}{p}+t_{0}$

*speedup*
- $S=\frac{T_{1}}{T_{p}}$

*Efficiency (Ratio of actual speedup to idea speedup)*
- $R=\frac{\text{Actual Speedup}}{\text{Ideal Speedup}}$

*Overhead Growing with processors*
- $t_{0}=2p$


**Power & Energy Equations**
*Dynamic Power*
- $p_{\text{dynamic}}= \frac{1}{2}*C*V^2*f$
	- rearrange equation to solve for specific variables 

*Static Power*
- $P_{\text{Static}}=V*I$

*Total Power Reduction Constraint*
- $P_{\text{new total}}=0.8*P_{\text{Old Total}}=P_{\text{static, new}}+P_{\text{Dynaic, new}}$


**Wafer & Die Cost / Defect**
*Wafer area*
- $A=\pi*r^2$

*Die Area*
- $\text{Die Area}=\frac{\text{wafer area}}{\text{Number of Dies}}$

*Yield* 
- $\text{Yield}=\frac{1}{\left( 1+\left( \text{Defects per area}*\frac{\text{Die Area}}{2} \right) \right)^2}$

*Cost Per Die*
- $\text{Cost Per Die}= \frac{\text{Wafer Cost}}{\text{Dies per wafer}*\text{Yield}}$


**Compiler & Speedup**
*Speedup*
- $\text{Speedup}=\frac{T_{old}}{T_{new}}$

*Clock Rate Ratio(if same execution time)*
- $\frac{\text{Clock Rate}_{A}}{\text{Clock Rate}_{B}}=\frac{\text{Instrution}_{A}*\text{CPI}_{A}}{\text{Instruction}_{B}*\text{CPI}_{B}}$

*Execution Time From MIPS*
- $T=\frac{\text{Instruction Count}}{\text{MIPS}*10^6}$


**Pipelining & CPI Impact**
*Extra CPI form Mis-predicted Branches*
- $\text{Extra CPI}=\text{Penalty}*(1-\text{Accuracy})*\text{Branch Frequency}$
	- penalty usually being 2-3

*Total CPI (with stalls or hazards)*
- $\text{Total CPI}=\text{Base CPI}+\text{Stall cycles per instruction}$

*Speedup (from pipelining, ISA changes, etc.)*
- $\text{Speedup}=\frac{\text{Old execution Time}}{\text{New Execution Time}}=\frac{\text{Old CPI}}{\text{New CPI}}$
	- If clock Rate Constant

*Pipeline Speedup*
- $\text{Speedup}_{\text{ideal}}=\text{Number of pipeline stages}$
- $\text{Speedup}_{\text{real}}=\frac{\text{Execution time}_{\text{Non-Pipelined}}}{\text{Execution Time}_{\text{pipelined}}}$


*Pipeline Clock Cycle Time*
- $\text{Cycle Time}_{\text{Pipeline}}=\text{max}(\text{Stage Delay})+\text{Pipeline Register Overhead}$

**Branch Conversion Impact**
*if a fraction of branches are replaced*
- New instruction count:
	- $\text{New Instructions}=\text{Original}+\text{Extra from replacement}$

- Speedup or slowdown comes from:
	- $\text{Execution Time}∝\text{Instruction Count}*\text{CPI}$

**Cache Miss Penalty Impact**
*Average Memory Access Time*
- $\text{Average Memory Access Time (AMAT)}=\text{Hit Time}+\text{Miss rate}*\text{Miss Penalty}$
-
