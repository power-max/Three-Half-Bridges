# Three Half Bridges
Three Half Bridges project is intended to be a universal(ish) module for use in larger power conversion and motor control systems.

This PCB aims to create a reasonably universal half bridge driver that can be used for medium to high power (100W to 1kW) electrical systems, such as power converters (buck converter, forward converter, LC or LLC converter, etc) motor drivers, etc. As such it is fairly bare-bones and additional components may need to be added external to this PCB for a particular system.

Half bridge power is provided via the bananna jack VCC and GND, the center terminal is the output of the half bridge.

An IRS2186 is used for its high current drive capability and flexabiility in driving the FETs independantly. End user is expected to design in proper dead-time control as there are no safegaurds against shoot-through.

Notes:
There is currently NO electrical isolation between the signal in and the high power connections. This may be a future consideration.
The end-user is responsible for selecting the exact componts used for this PCB design. (i.e. MOSFET choice, bootstrap capacitor value)

Licensed under the MIT License (https://mit-license.org/)
