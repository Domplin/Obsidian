

**Write 0**

![[6T-SRAM Write Operation write 0.png]]

- Launch the write data on $BL$ and $\overline{BL}$ 
- Word line signal is turned on
- Low but line values flips cell data
- Access transistors mush be stronger than [[NMOS vs PMOS|PMOS]] pull-up transistor (or load)


*Pull-up Ratio*: $\frac{\left( \frac{W}{L} \right)_{pmos}}{\left( \frac{W}{L} \right)_{access}}$ - Typical Pull-up ratio $<1.5$ 

-  Note: for the same size, [[NMOS vs PMOS|PMOS]] is slightly weaker due to lower hole mobility: $\mu_{h} \approx \frac{1}{2} ,u_{e}$ 