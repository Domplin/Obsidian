Self boosting is a technique used in NAND flash memory to prevent program disturb on unselected cells sharing the same bit line or word line during a program operation 

During programming, a high voltage (15-20V) is applied to the selected wordline. All cells in the same NAND string ([[NAND Array Structure]]) share this bitline. Unselected cells on inhabited bitlines (those not being programmed) are at risk of being unintentionally programmed by this high field 


**How self Boosting Works**
The core Idea is to float the channel of unselected strings so the channel potential rises along with the wordline voltage, reducing the net voltage across the tunnel oxide of unselected cells

1) Select gate source (SGS) is turned off - isolating the channel from the soruce line
2) Select gate drain (SGD) is turned off - isolating the channel from the bitline
3) The wordline voltage turns up ($V_{pgm}$)
4) Because the channel is floating, capacitive  coupling between the wordlines and the channel boosts the channel potential - typically ~8-10V
5) The net voltage across the tunnel oxide of the unselected cells becomes $V_{tunnel}=V_{pgm}-V_{channel-boost}$ 



**Boosting Efficiency**
Boosting efficiency is given by:
$$
\frac{\Delta V_{ch}}{V_{ppass}}=\frac{C_{cell}}{C_{cell}+C_{dep}}*\left[ \frac{N-1}{N}+\frac{1}{N} \frac{V_{pp}}{V_{ppass}}\right]= \frac{C_{cell}}{C_{cell}+C_{dep}}\left[ 1+\frac{1}{N}\left( \frac{V_{pp}}{V_{ppass}}-1 \right) \right]
$$

- The boosted channel potential can