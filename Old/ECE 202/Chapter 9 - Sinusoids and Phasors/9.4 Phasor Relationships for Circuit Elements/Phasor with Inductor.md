For the inductor L, let assume the current through it is $i=I_{m}\cos(\omega t+\phi)$
The voltage across the inductor is:
$$
v=L\frac{di}{dt}=-\omega LI_{m}\sin(\omega t+\phi)
$$
Given that $-\sin A=\cos(A+90^\circ)$ The voltage can be written as:
$$
v=\omega LI_{m}\cos(\omega t+\phi+90^\circ)
$$

Which then transforms the to the [[Phasor|phasor]]:
$$
V=\omega LI_{m}e^{j(\phi+90^\circ)}=\omega LI_{m}e^{j\phi}e^{j+90^\circ}=\omega LI_{m}\angle\phi+90^\circ
$$
Because $e^{j90^\circ} = j$ and $I_{m}\angle\phi = I$ the voltage can be written as:
$$
V=j\omega LI
$$
