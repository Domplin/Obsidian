---
tags:
  - ECE_564
  - lecture_10
  - Equations
---
**Cell Design Rules**
- Thin tunnel oxide: $t_{tox}\approx 6-8nm$
- Thick blocking oxide: $t_{box} \approx 12-18nm$
- For data retention: $t_{ox} > 4.5nm$


**Memory cell at Retention state**
![[Design Rules.png]]


*What is the voltage of the floating gate when $V_{CG}=0V$* 
$$
V_{FG}=\frac{Q_{FG}}{C_{box}+C_{tox}}
$$
$$
\approx \left( \frac{Q_{FG}}{C_{box}} \right) \frac{C_{box}}{C_{box}+C_{tox}}\approx \alpha V_{T}
$$

*In general, when $V_{CG}\neq 0$:*
$$
V_{FG}=V_{CG}\left( \frac{C_{box}}{C_{box}+C_{tox}} \right)+\frac{Q_{FG}}{C_{box}+C_{tox}}\approx \alpha(V_{CG}+V_{T})
$$
Coupling Ratio: $\alpha=\left( \frac{C_{box}}{C_{box}+C_{tox}} \right)$



**Summary**:
![[Design Rules - Gate stack.png]]

*Metal Gate*: 
- High work function metal gate
	- To prevent electron back-tunneling (Barrier height)
- [[High-K Dielectric]] material 
	- To prevent electron back-tunneling (electric field) high CBO* necessary for retention
- Charge Trapping Material or FG
	- (Stoichiometric: deep trap, si-rich: shallow trap)
- Tunnel Oxide
	- Thin to enable FN tunneling (PGM & Erase)
	- Thick to prevent direct tunneling (Retention)


**CBO** - (Conduction Band Offset)