# Water Level Indicator

A simple electronic circuit designed to monitor and indicate the water level inside a tank, preventing overflow and dry running.

## Features / Functions
* **Real-Time Level Monitoring:** Displays low, medium, and full water levels using visual indicators (LEDs).
* **Overflow Alert:** Triggers a buzzer alarm when the tank reaches maximum capacity.
* **Low-Power Operation:** Consumes minimal power while continuously sensing water levels.

## Components Required
* **Sensor / Probes:** Copper wires or stainless steel probes (placed at different tank depths)
* **Transistors / IC:** 4x BC547 NPN Transistors *(or ULN2003 IC)*
* **Indicators:** 3x LEDs (Red, Yellow, Green)
* **Alarm:** 1x Piezo Buzzer
* **Resistors:** 4x 220Ω resistors, 4x 1kΩ resistors
* **Power Supply:** 9V DC Battery with battery clip
* **Miscellaneous:** Breadboard or PCB, connecting jumper wires

## How It Works
1. **Common Ground/Supply:** One wire connected to the positive terminal is placed at the bottom of the tank.
2. **Level Detection:** As water rises, it completes the circuit between the bottom wire and the probes placed at different heights.
3. **Signal Amplification:** Each probe sends a small current to the base of its respective transistor, turning it ON.
4. **Output Indication:** The activated transistor powers the corresponding LED, and the top-level probe activates the buzzer when the tank is full.
