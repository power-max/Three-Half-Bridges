# Three Half Bridges
Three Half Bridges project is intended to be a universal(ish) module for use in larger power conversion and motor control systems. This PCB aims to create a reasonably universal half bridge driver that can be used for medium to high power (100W to 1kW) electrical systems, such as power converters (buck converter, forward converter, LC or LLC converter, etc) motor drivers, etc. As such it is fairly bare-bones and additional components may need to be added external to this PCB for a particular system.

Digital isolator ICs are used for providing isolated gate drive signals and pretty much any generic low-side gate driver can be used for the actual gate driver ICs. I found some cheapies on LCSC for less than a dollar that claim 4A source and sink per channel, and each channel is paralell so in theory 8A source and sink is acheivable. Note that there is no logic to prevent shoot-through, as the user inputs each high and low switch independently. Use a TL494 style flip flop based pulse steering network or my Dead Time Insertion PCB to implement this logic from a single ended square wave.

Notes:
The end-user is responsible for selecting the exact componts used for this PCB design. (i.e. MOSFET or IGBT choice, choice of gate driver IC, value of capcitors, etc)

Licensed under the MIT License (https://mit-license.org/)

I was really drunk when I wrote this. Please consider buyin gm e more beerrs so I caan contune edevelopment thnaks!
