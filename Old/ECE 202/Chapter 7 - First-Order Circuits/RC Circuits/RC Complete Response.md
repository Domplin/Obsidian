The **complete response** or total response of the RC circuit to a sudden application of a dc voltage source

$Complete Response = Natural \mathrm{Re}sponse + Forced \mathrm{Re}sponse$
- Natural Response:
	- Stored energy
- Forced Response
	- independent source

Another way to look at the complete response is to break down the two components - one temporary and the other permanent

Complete Response = [[Old/ECE 202/Chapter 7 - First-Order Circuits/Transient Response]] + [[Steady-State Response]] 

The Complete Response can be written as:
$$
v(t)=v(\infty) + [v(0)-v(\infty)]e^{-t/\tau}
$$
where $v(0)$ is the initial voltage at $t=0^+$ and $v(\infty)$ is the final or steady-state value.

Parts of the equation are needed to be able to [[Find RC Step Response]] 