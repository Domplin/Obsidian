Using the **Dot Convention** a dot is placed in the circuit at one end of each of the two magnetically coupled coils to indicate the direction of the magnetic flux.

The dot convention is as follows:
![[Pasted image 20240404195651.png]]

If a current *enters* the dotted terminal of one coil the reference polarity of the mutual voltage in the second coil is *positive* at the dotted terminal of the second coil.

If a current *leaves* the dotted terminal of one coil, the reference polarity of the mutual voltage in the second coil is negative at the dotted terminal of the second coil.

The reference polarity of the mutual voltage depends on the reference direction of the inducting current and the dots on the coupled coils.

![[Pasted image 20240404195957.png]]


![[Pasted image 20240404200017.png]]

$$
\begin{align}
L=l_{1}+L_{2}+2M \text{ (Series-aiding connection)} \\
L=L_{1}+L_{2}-2M \text{ (Series-opposing connection)}
\end{align}
$$



Analyzing circuits with mutual inductance:

![[Pasted image 20240404200239.png]]
Applying KVL to coil 1:
$$
v_{1}=i_{1}R_{1}+L_{1} \frac{di_{1}}{dt} +M \frac{di_{2}}{dt}
$$

For coil 2 KVL gives:
$$
v_{2}=i_{2}R_{2}+L_{2} \frac{di_{2}}{dt} +M \frac{di_{2}}{dt}
$$
We can write it in them in the frequency domain as:
$$
V_{1}=(R_{1}+j\omega L_{1})I_{1}+j\omega MI_{2}
$$
$$
V_{2}=j\omega MI_{1}+(R_{2}+j\omega L_{2})I_{2}
$$
As a second example consider the circuit (b) WE analyze this in the frequency domain. Applying KVL to coil 1, we get 
$$
V=(Z_{1}+j\omega L_{1})I_{1}-j\omega MI_{2}
$$
For coil 2:
$$
0=-j\omega MI_{1}+(Z_{1}+j\omega L_{2})I_{2}
$$
