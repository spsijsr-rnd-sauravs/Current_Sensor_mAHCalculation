Aim: To measure current and voltage and also calculate the total power consumed when the battery gets drained.

Materials required: Resistor (10.8, 20 W), Arduino UNO, Relay 5V, Li-Po battery ( 12V, 3S battery), Current Sensor ( ACS712 30A), bread-board, jumper wires, 2 resistors ( R1=1762  and R2=976) which we used for the voltage divider ( because the Arduino can sense only up to 5V, so we have to divide the voltage, which means to create a voltage divider in the circuit).

Procedure: 

At first what I do is like measure the resistance of the resistor, or better we say load, using multimeter and which comes out to be 10.8 whose power is 20 W. 

And after making the circuit using the load, relay, current sensor, jumper wires, the two resistors for voltage divider, battery, and the Arduino UNO. 

We first took the readings as per mentioned below:
		R( load)=10.8 
		V (supply/battery)=11.9V
		VR=10.3V (voltage drop across the load which is R)
So from ohm’s law: current flow through the load
		IR=10.310.8=0.953A  		(verified using multimeter)

Also we have measured the off-set voltage ( in the context of electronics and electrical engineering, refers to a small voltage that is present at the output of a circuit when ideally, it should be zero) , How: when load is not connected to the battery we can measure the off-set voltage using the multimeter and ACS712 ( 30A), and it comes out to be:
		Voff=2.51V                                                  ...(1)

Also, we had measured the output voltage as mentioned in the case of Voff, here we connect load with the battery ( supply), and it comes out to be:
		Vout=2.58V                                                    ...(2)

So we can measure the sensitivity of the current sensor ACS712 30 A ( although it’s been mentioned in the datasheet, but it's the typical value not the exact value), and sensitivity can be calculated as follows: 
		S=(Vout-Voff)/I=(2.58-2.5)/10.97 V/A=0.0721649485 V/A
