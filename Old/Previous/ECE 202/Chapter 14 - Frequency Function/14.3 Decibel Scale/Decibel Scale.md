Since Bode plots are based on logarithms, its important that we keep the [[Properties of Logarithms]] in mind

In communications systems, gain is measured in *bels*. Historically, the bel is used to measure the ratio of two level of power or power gain G; that is:
$$
G=Number Of Bells=\log_{10} \frac{P_{2}}{P_{1}}
$$
The *decibel* (dB) provides us with a unit of less magnitude. It is 1/10th of a bel and is given by:
$$
G_{dB}=10\log_{10} \frac{P_{2}}{P_{1}}
$$
when $P_{1} = P_{2}$ there is no change in power and the gain is 0 dB.

Another reason why logarithms are greatly used: The logarithm of the reciprocal of a quantity is simply negative the logarithm of that quantity:

if $P_{2} = 2P_{1}$ 
$$
G_{dB}=10\log_{10}2 \approx 3
$$
if $P_{2} = 0.5P_{1}$
$$
G_{dB}=10\log_{10}0.5 \approx  -3
$$

Alternatively the gain **G** can be expressed in terms of voltage or current ratio. To do so consider the network shown: 
![[Pasted image 20240328180219.png]]

If $P_{1}$ is the input power, $P_{2}$ is the output (load) power, $R_{1}$ is the input resistance. $R_{2}$ is the load resistance, then $P_{1}=\frac{0.5V_{1}^2}{R_{1}}$ and $P_{2}=\frac{0.5V_{2}^2}{R_{2}}$ 

$$
\begin{align}
G_{dB}=10\log_{10} \frac{P_{1}}{P_{2}}=10\log_{10} \frac{\frac{V_{2}^2}{R_{2}}}{\frac{V_{1}^2}{R1}} \\
=10\log_{10}\left( \frac{V_{2}}{V_{1}} \right)^2+10\log_{10} \frac{R_{1}}{R_{2}}  \\
G_{dB}=20\log_{10} \frac{V_{2}}{V_{1}}-10\log_{10} \frac{R_{1}}{R_{2}}
\end{align}
$$

For the case when $R_{2}=R_{1}$, a condition that is often assumed when comparing voltage levels, the equation becomes:
$$
G_{dB}=20log_{10} \frac{V_{2}}{V_{1}}
$$

Instead if $P_{1}=I_{1}^2R_{1}$ and $P_{2}=I_{2}^2R_{2}$, for $R_{1} = R_{2}$ the obtained equation is:
$$
G_{dB}=20\log_{10} \frac{I_{2}}{I_{1}}

$$
**Note:** [[Important Decibel Scale Notes]]
