---
tags:
  - ECE_571
  - Lecture_5
---
**Pitch and Wavelength**
- We define pitch as the width + spacing of a feature = 2b
$$
2b=k_{1}  \frac{\lambda}{NA}
$$
$$
NA=n\sin(\alpha)
$$
**Phase Shift Masks**
- Uses interference caused by phase differences to improve resolution and contrast
- Goal is to allow features smaller than wavelength of light to be printed 
- Two Types:
	- Alternating - caused by phase shift and interference pattern 
	- Attenuated - Partially opaque, still causes desirable interference patterns


**Silicon Dioxide**
- Oxide is formed by heating Si in an oxidizing atmosphere
	- Wet oxidation - water vapor + 900-100$\degree$C - For thick field oxides
	- Dry oxidation - Pure oxygen + 1200$\degree$C - For thin field oxides
	- Atomic layer deposition (ALD) - Built up layer by layer 
- First two approaches consume Si wafer
- SiO2 has 2x volume of Si


**Wet Etching**
- Wafers are immersed in a tank of etchant (usually sulfuric acid and hydrogen peroxide) for a specific amount of time, transferred to a rinse station for acid removal and transferred to a station for final rinse and a spin dry
- Wet etching is limited to a pattern sizes of 3 microns
- Wet etching is isotropic, resulting a sloped sidewalls 

**Dry Etching**
- Uses gases and plasma energy to cause chemical reaction
- Wafers are loaded into a chamber and the pressure inside is reduced by a vacuum system
- After the vacuum is established, the chamber is filled with reactive gas
- A power supply creates a radio frequency (RF) field through electrodes in the chamber 
- The field energizes the gas mixture to a plasma state to attack the layers (often Si02) in the pattern openings, converting it to volatile components that are removed by the vacuum system

**Creating Diffusion**
- Two approaches: CVD and Ion Implantation - Diffusion occurs in both
- Chemical Vapor Deposition - heated gasses react next to wafer and product is deposited on surface. High temperatures cause diffusion into wafer
- Ion Implantation - Bombards wafer with highly energized dopants. Atoms will travel below surface. High temperatures (>800$\degree$C) even out concentrations but too much will cause over diffusion - rest of fabrication needs to limit temperatures 
- Arsenic and Phosphorus are frequently used to form n-type diffusion
- Boron is frequently used for p-type
