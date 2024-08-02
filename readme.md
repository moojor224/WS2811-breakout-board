# WS2811 Breakout Board

## v1 (failed design)

![v1 pcb](./images/v1%20pcb.png)
![v1 photo](./images/v1%20photo.jpg)

unfortunately, I decided that I was too good at making pcbs to take any measurements before ordering the boards, so I found the following issues after they arrived:

 - the 4 pin header at the top of the board had the wrong spacing (too close together)
 - the sop-8 footprint was the wrong size (too small)
 - the through-holes for the terminal blocks were too small for the terminal block pins
 - the smd resistor pads for low-speed enable are too small to realisically solder
 - the100 ohm resistor from 3.3VIN to VDD was not necessary and could be removed to save space

## v2

This time around, I actually measured the components I had and adjusted the incorrect components like so.
 - replace the 4-pin footprint with 4 individual through-holes
 - increase the inner diameter of all terminal block through holes to 1mm
 - double the width of all traces

Additionally, the board shrunk by 0.1 inches horizontally due to taking out the 100 ohm resistor

while checking if I soldered the IC to the pcb correctly, I found that the in/out GND pins at the left/right side of the pcb were not connected. This is temporarily fixable by simply connecting the screw terminals with a short length of wire, but is fixed in V2.5


![v2 pcb](./images/v2%20pcb.png)
![v2 photo](./images/v2%20photo.jpg)

## v2.5

this version is just a re-route of v2 to put the traces on one side
also fixes the gnd disconnect mistake from V2


![v2.5 pcb](./images/v2.5%20pcb.png)
![v2.5 photo pending](./images/v2.5%20photo.jpg)