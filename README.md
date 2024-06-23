
# Distance Measurement Using Basys 3 and HC-SR04 

This propsed system uses basys 3 FPGA and HCSR04 ultrasonic sensor to measure distance and display it on the seven segment display of Basys 3.

## Components Used

| Component             | Link                                                               |
| ----------------- | ------------------------------------------------------------------ |
| HC SR04 |https://robu.in/product/hc-sr04-ultrasonic-range-finder/?gad_source=4   |
| Breadboard | https://robu.in/product/mb102-830-points-solderless-prototype-pcb-breadboard-high-quality/|
| Logic level Converter | https://robu.in/product/level-converter-4-channel/?gad_source=4 |
| 5v DC Adapter | https://www.amazon.in/Generic-Power-Adapter-5V-1A/dp/B0D1CK9G8K?source=ps-sl-shoppingads-lpcontext&ref_=fplfs&psc=1&smid=A19IQ7FFZYA1ZN
|Male to Female Connector ||https://sharvielectronics.com/product/dc-power-jackfemale-adapter-pcb-mount/
|Jumper Wires||

HCSR04 has 4 pins: VCC,GND,ECHO,TRIGGER. It needs 5 volts to operate, so we have used an external power supply to power the sesnor. We have also used the logic level converter to step up and step down the incoming and outgoing voltages. The basys 3 can take maximum 3.3 volts of input and output, so the trigger pulse from basys 3 will be passed through the logic level converter and step up to 5 volts, and the echo pulse of 5 volts will step down to 3.3 volts as basys 3 can take maximum 3.3 volts from PMOD. Photos of the circuit have been added to the photos folder.

Add all the files in the source files and the XDC file to the XDC file location.

The Circuit was tested at Logic Design Workshop of Institute Of Technical Education And Research(ITER), SOA Deemed to be university
