---
tags:
  - ECE_564
  - Lecture_1
  - Equations
---
- Operation of the enhancement NMOS transistor as $V_{DS}$ is increases
	- The induced channel acquires a *tapered shape* and its resistance increases as $V_{DS}$ is increased while $V_{GS}$ is kept fixed at $V_{GS}= V_{th}+V_{OV}$ [[Threshold and Overdrive Voltage]]

- Note that $V_{DS}$ appears as a voltage drop across the length of the channel
	- The voltage between the gate and points along the channel decreases from $V_{GS}=V_{th}+V_{OV}$ at the source end to $V_{GB}=V_{th}+V_{OV}-V_{DS}$ at the drain end
- Since the channel depth or charge depends on this effective voltage, we find that the channel is no longer uniform, rather taking the tapered shape 
![[Current Voltage For high V.png]]
![[Current Voltage For high V Graph.png]]

$$
I = Q(x) \times v(x)
$$

$Q(x)$ = Charge per length (C/cm)
	$Q(x)=C_{ox}(W)(V_{OV}-V_{ch}(x))$
$v(x)$ = Carrier Velocity (cm/s)
	$v(x)=\mu_{n}E_{\text{field}}(x)=\mu_{n} \frac{V_{DS}}{L}$
$$
I=\mu _n C_{ox}\left( \frac{W}{L} \right)\left( V_{OV}-\frac{1}{2}V_{OV}  \right)V_{OV}
$$

**What Happens when $V_{DS}=V_{OV}$**
$I=\mu _n C_{ox}\left( \frac{W}{L} \right)\left( V_{OV}-\frac{1}{2}V_{OV}  \right)V_{OV}= \mu_{n}C_{ox}\left( \frac{W}{2L} \right)V_{OV}^2$
