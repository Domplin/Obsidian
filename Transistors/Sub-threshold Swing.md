---
tags:
  - ECE_564
  - Lecture_2
---

- Sub-threshold swing measures how efficiently a MOSFET switches from *on* to *off* 
- Defined as the gate voltage change (mV) required to alter the drain current by one order of magnitude is the sub-threshold region
- A lower sub-threshold swing (ideally 60mV/dec @ 300K) indicates a sharper faster, and more power efficient switch
![[Sub-threshold Swing.png]]


$$
I_{sub}=I_{0}e^{q(V_{GS}-V_{T})/mk_{B}T}
$$
$$
\ln(I_{sub})=\text{constant} + \frac{V_{GS}}{m(k_{B}T)/q}
$$
$$
\log_{10}(I_{sub})=\text{constant}+\frac{V_{GS}}{2.3m(k_{B}T/q)}
$$
$$
S=\left[ \frac{\Delta(\log_{10}(I_{sub}))}{\Delta V_{GS}} \right]^{-1}=2.3m(k_{B}T/q)  \frac{mV}{dec}
$$
