# Three Half Bridges
Three Half Bridges project is intended to be a universal(ish) module for use in larger power conversion and motor control systems.

This PCB aims to create a reasonably universal half bridge driver that can be used for medium to high power electrical systems, such as power converters (buck converter, forward converter, LC or LLC converter, etc) motor drivers, etc. As such, it is a bit over-engineered for most modest applications and allows direct control over all switches independently.

Gate drive topology uses a descrete design optimised for high gate drive currents and minimal propagation delay. End user is expected to design-in proper dead-time control as there are no safegaurds against shoot-through.

Input is intended to be RTZ (Return to Zero) encoded differential pulses into the inputs of the pulse transformers. Please respect the volt time ratings of the utilized pulse transformers if driving them with a low impedance high current capable source. A positive pulse that exceeds 2V should latch the gate driver HIGH. a negative going pulse of -2V or less should latch the gate driver LOW. If a pulse is missed then this circuit will explode. A shielded differential pair or shielded twinax is recommended for this, along with PLENTY of margin in the voltage thresholds!

Notes:
* The end-user is responsible for selecting the exact componts used for this PCB design. (i.e. MOSFET choice, bootstrap capacitor value)
* While the gate driver input is isolated, this isolation is only as good as the pulse transformer used and the allowable creapage/clearence of the PCB layout. This is a hobby project and not intended for commerical use so no effort has been put into getting any sort of safety certifications!

Licensed under the TAPR Open Hardware License (www.tapr.org/OHL)
