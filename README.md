# LDR Automatic Light Switch

Automatic light-sensing circuit using an LDR (Light Dependent Resistor) and a BC547 NPN transistor as a switch — LEDs turn **ON** in darkness and **OFF** in light. The project includes a Tinkercad circuit simulation and a physical breadboard prototype housed in a cardboard diorama demonstrating dusk-to-dawn automatic lighting.

## Overview

This project simulates a real-world automatic streetlight / garden light system. The LDR continuously senses ambient light levels. When light falls below a certain threshold (dusk/night), the resistance of the LDR increases, which changes the voltage at the base of the transistor — turning it ON and lighting the LEDs. When ambient light increases again (dawn/day), the transistor switches OFF and the LEDs turn off automatically.

## Components Used

| Component | Quantity |
|---|---|
| LDR (Light Dependent Resistor) | 1 |
| BC547 NPN Transistor | 1 |
| LEDs (Green / Blue / Red) | 2–3 |
| Resistors (current limiting & biasing) | 2–3 |
| 9V Battery | 1 |
| Breadboard | 1 |
| Jumper Wires | As required |
| Cardboard, straws, artificial flowers (diorama model) | For enclosure/demo setup |

## Working Principle

1. The LDR and a fixed resistor form a **voltage divider**.
2. In bright light, the LDR's resistance is low, keeping the transistor's base voltage below the threshold — transistor stays OFF, LEDs stay OFF.
3. In darkness, the LDR's resistance rises sharply, raising the base voltage enough to turn the transistor ON.
4. Once ON, the transistor allows current to flow through the LED branch, lighting up the LEDs.
5. This creates an automatic, sensor-driven ON/OFF switching behavior with no manual intervention.

## Circuit Diagram

The circuit was designed and simulated in **Tinkercad** before physical assembly.
- 9V battery → breadboard power rails
- LDR + resistor → voltage divider feeding transistor base
- Transistor (BC547) → switches LED branch
- LED + current-limiting resistor → output indicator

Add circuit 
## Prototype / Demo

A physical prototype was built on a breadboard and mounted inside a cardboard diorama (styled as a garden with artificial flowers and lamp posts) to visually demonstrate how the light would activate automatically in low-light conditions, mimicking a real streetlight setup.

Add circuit image
## How to Build

1. Place the LDR and a fixed resistor in series on the breadboard to form a voltage divider.
2. Connect the junction of the LDR and resistor to the base of the BC547 transistor (through a resistor if needed).
3. Connect the collector to the LED (with a current-limiting resistor) and the emitter to ground.
4. Power the circuit using a 9V battery.
5. Test by covering the LDR with your hand — the LED should turn ON; uncover it — the LED should turn OFF.

## Future Improvements

- Replace LEDs with a relay-driven AC bulb for real-world street/garden lighting.
- Add a microcontroller (Arduino/micro:bit) for adjustable sensitivity and logging.
- Include a potentiometer for manual threshold calibration.
- Add solar charging for an off-grid, sustainable lighting solution.

## Author

Shamini — Electronics and Communication Engineering (ECE) Student
