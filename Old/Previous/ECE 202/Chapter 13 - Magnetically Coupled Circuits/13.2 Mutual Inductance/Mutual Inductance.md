
**Mutual Inductance** is the ability of one inductor to induce a voltage across a neighboring inductor measured in Henrys (H)

When two inductors are close in close proximity to each other, the magnetic flux caused by current in one coil links with the other coil, inducing voltage in the other. This is known as **Mutual Inductance** 


Using Faraday’s law the voltage *v* induced in the coil is proportional to the number of turns **N** and the time rate of change of the magnetic flux $\phi$

$$
v=N \frac{d\phi}{dt}
$$
The flux $\phi$ is produced by current $i$ so that any change in $\phi$ is caused by a change in the current:
$$
v=N \frac{d\phi}{di} \frac{di}{dt}
$$
or 
$$
v=L \frac{di}{dt}
$$
which is the same voltage-current relationship for the inductor. The inductance $L$ of the inductor is given as 
$$
L=N \frac{d\phi}{dt}
$$
Consider two coils with self-inductance $L_{1}$ and $L_{2}$ that are in close proximity to one another. Coil 1 has $N_{1}$ turns and coil two has $N_{2}$ turns. The magnetic flux $\phi_{1}$ emanating from coil 1 has two components: one component $\phi_{11}$ links only coil 1 and another component $\phi_{12}$ links both coils.
![[Pasted image 20240404194453.png]]

$\phi_{1}=\phi_{11}+\phi_{12}$

Although the two coils are physically separated, they are said to be **Magnetically coupled**. Since the entire flux $\phi_{1}$ links coil 1, the voltage induced in coil 1 is:
$$
v_{1}=N_{1} \frac{d\phi_{1}}{dt}
$$
Only flux $\phi_{12}$ links coil 2 so the voltage induced in coil 2 is 
$$
v_{2}=N_{2} \frac{d\phi_{12}}{dt}
$$
The fluxes are caused by current $i_{1}$ flowing in coil 1 and can be written as:
$$
v_{1}=N_{1} \frac{d\phi_{1}}{di_{1}} \frac{di_{1}}{dt} = M_{21} \frac{di_{1}}{dt}
$$

Where $L_{1}=N_{1} \frac{d\phi_{1}}{di_{1}}$ is the self inductance of coil 1. The voltage induced in coil 2 can also be written as
$$
v_{2}=N_{2} \frac{d\phi_{1}}{di_{1}} \frac{di_{1}}{dt} = L_{1} \frac{di_{1}}{dt}
$$
where
$$
M_{21}=N_{2} \frac{d\phi_{12}}{di_{1}}
$$
$M_{21}$ is known as the **Mutual Inductance** of coil 2 with respect to coil 1. The subscript *21* indicates that the inductance $M_{21}$ relates the voltage in coil 2 by coil 1. The open-circuit *mutual voltage* (or induced voltage) across coil 2 is
$$
v_{2}=M_{21} \frac{di_{1}}{dt}
$$

