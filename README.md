## AC-to-DC Converter — Circuit Design and PCB Layout

## Overview

This project involves the schematic design and PCB layout of an AC-to-DC converter circuit. The design uses a four-diode bridge rectifier to perform full-wave rectification, followed by capacitor filtering to produce a smoother DC output.

The project also includes component footprint assignment and two-layer PCB routing, with attention to component placement and power trace width.

## Objectives

- Design a bridge rectifier-based AC-to-DC conversion circuit.
- Implement capacitor filtering to reduce output voltage ripple.
- Include an LED indicator for the presence of DC output.
- Assign appropriate component footprints.
- Develop a routed two-layer PCB layout.

## Circuit Components

| Component | Function |
|---|---|
| D1–D4: 1N4007 diodes | Full-wave bridge rectification |
| C1: Filter capacitor | Reduces ripple in the rectified output |
| R1: 10 kΩ resistor | Bleeder resistor for capacitor discharge |
| D5: LED | DC power indication |
| R2: Series resistor | Limits LED current |
| J1 | Input screw terminal |
| J2 | DC output screw terminal |

## Working Principle

### 1. Bridge Rectification
Four 1N4007 diodes are arranged in a bridge configuration. The circuit rectifies the AC input so that both half-cycles contribute to a unidirectional, pulsating output.

### 2. Capacitor Filtering
The filter capacitor C1 smooths the rectified waveform by storing charge and supplying current between waveform peaks, reducing output ripple.

### 3. Bleeder Resistor
The 10 kΩ resistor R1 provides a discharge path for the filter capacitor after power is disconnected.

### 4. LED Power Indicator
The LED D5, connected with a current-limiting resistor R2, indicates the presence of DC output.

### 5. DC Output
The filtered output is available at the J2 screw terminal for connection to a suitable load.

## PCB Design

The PCB layout incorporates the following design considerations:

- **Two-layer routing:** Uses top and bottom copper layers to route circuit connections.
- **Power trace width:** Wider traces are used for power connections to help reduce resistance and voltage drop.
- **Component placement:** Input terminals, rectifier diodes, filter capacitor, indicator circuit, and output terminals are arranged according to circuit flow.
- **Bridge rectifier layout:** The four diodes are positioned to implement the full-wave rectifier circuit.

## Tools and Technologies

- Cadence schematic capture and PCB design tools
- Circuit schematic development
- Component footprint assignment
- Two-layer PCB routing
- Basic power electronics and rectifier design

## Project Files

- Circuit schematic
- Component footprint assignment screenshots
- Routed PCB layout
- Additional design documentation, where available

## Key Learning Outcomes

- Understanding full-wave bridge rectification
- Capacitor-based DC filtering
- Component selection and footprint assignment
- PCB component placement and routing
- Power trace width considerations in PCB design

## Future Improvements

- Simulate the rectifier output and quantify ripple voltage.
- Measure output voltage under different load conditions.
- Evaluate diode losses and capacitor requirements.
- Verify PCB trace widths against the intended current and temperature rise.
- Add input protection and appropriate regulation if required by the application.

