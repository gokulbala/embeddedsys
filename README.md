4.1 ALGORITHM:
•	The parameters are sensed through the sensors which are given as the input to the Port B of the transmitter.
•	The PIC 16F877A microcontroller transmits the eight packet data through a RS 485 chip which has a capacity of transmitting data up to 4Km.
•	 The data is received at the receiver through RS485.
•	This data is moved to Port B of the PIC 16F877A microcontroller of the receiver side.
•	The data from the port B is moved to a temporary register.
•	The data in the temporary register are checked bit by bit from bit 0 to bit 7 sequentially for logic high.
•	In case any bit is found logic high, then it calls the corresponding sub-routine and indicates the fault in the parameter through an LCD display and simultaneously a voice output through APR9600 chip.
•	Port B serves as an input to the LCD display.
•	PD4 and PD5 pins are used as the control lines for the LCD.
•	A port A and PE0 and PE1 pin of Port E serve as an input for the voice output.
•	  APR9600 is a voice recording and reproducing chip which has a capacity of 60 seconds which is divided equally into 7.5 seconds allotted to each of the eight channels.
•	We use a 16 Χ 2 LCD which displays the corresponding fault in the parameters.