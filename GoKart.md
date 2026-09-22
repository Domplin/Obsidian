- USB-to-CAN adapter using candleLight firmware

- SPI Click can drop frames on high CPU load - overflow the clicks internal buffer 
	- forcibly allocate more memory to the click in the Pi's memory
	- reduce the status rate in VESC tool