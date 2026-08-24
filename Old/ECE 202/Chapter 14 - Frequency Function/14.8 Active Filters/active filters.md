There are 3 major limitations to the [[Passive Filters|passive filters]].
1) they cannot generate gain greater than 1
	- Passive elements cannot add energy to the network
2) they may require bulky and expensive inductors
3) they perform poorly at frequencies below the audio frequencies range $300Hz<f<3000Hz$ 
	- They are still useful at high frequencies 

Active filters consist of combinations of resistors, capacitors, and op-amps.

They offer advantages over [[Passive Filters]]
1) they are often smaller and less expensive because they do not require inductors
2) they can provide amplifier gain in addition to providing the same [[Frequency Response|frequency response]] as [[Passive Filters]]
3) active filters can be combined with buffer amplifiers (voltage followers) to isolate each stage of the filter from source and load [[Impedance|impedance]] effects
	- This isolation allows designing the stages independently and then cascading them to realize the desired [[Transfer Function|transfer function]]
	- However, active filters are less reliable and less stable

The limit of most active filters is about $100kHz$ - most active filters operate well below that frequency