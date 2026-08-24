To obtain a [[Transfer Function]] using [[Possible Transfer Functions]] we first obtain the frequency-domain equivalent of the circuit by replacing resistors, inductors, and capacitors with their [[Impedance|impedance]] values, $V , j\omega L, \frac{1}{j\omega C}$ 

We obtain the [[Frequency Response]] of the circuit by plotting the magnitude and phase of the [[Transfer Function|transfer function]] as the frequency varies. 

The transfer function $H(\omega)$ can be expressed in terms of its numerator polynomial $N(\omega)$ and denominator polynomial $D(\omega)$ as:
$$
H(\omega)= \frac{N(\omega)}{D(\omega)} 
	$$ Where $N(\omega)$ and $D(\omega)$ are not necessarily the same expressions for the input and output functions. The equation assumes that the common numerator and denominator in $H(\omega)$ have canceled, reducing the ratio down to the lowest terms, using [[Zeros and Poles]], the toots of $N(\omega)$ are called the *zeros*, The roots of $D(\omega)$ are called the *poles* of $H(\omega)$ 

To avoid Complex algebra it is easier to replace $j\omega$ with $s$ temporarily and replace them back at the end. 