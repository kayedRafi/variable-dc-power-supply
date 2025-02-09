# Variable DC Power Supply

## Project Overview
A versatile variable DC power supply designed and simulated in Proteus. This circuit converts AC input to a variable DC output with voltage regulation and protection features. The design includes LED indicators and a user-adjustable voltage control.

## Features
- Input Voltage: 240V AC
- Adjustable DC Output
- LED Status Indicators (Red/Green)
- Short Circuit Protection
- Voltage Regulation
- Current Monitoring
- Push Button Control

## Components List
### Active Components
- U5: LM317T (Voltage Regulator)
- U2: 7808 (Voltage Regulator)
- U3: 7815 (Voltage Regulator)
- U4: LM358 (Dual Op-Amp)
- Q6, Q7: 2N2222A (NPN Transistors)

### Passive Components
- BR2: Bridge Rectifier
- C1, C4: 1μF Capacitors
- C2: 2200μF Capacitor
- R1: 10k Resistor
- R2: 240Ω Resistor
- R5: 10k Resistor
- R6: 1k Resistor
- R7: 4.2k Resistor
- R8: 10k Resistor
- R9: 10k Resistor
- R10, R11: 1k Resistors
- R12: 1k Resistor
- R15, R16: Various Values
- RV1: 10k Potentiometer

### Indicators and Protection
- D1, D2: LED (Red/Green)
- D3, D4: 1N4735A Zener Diodes
- D6, D7: LED Indicators
- RL1, RL2: 5V Relays

### Connectors
- J1, J2: Terminal Blocks
- BUTTON: Push Button Switch

## Circuit Design
The circuit consists of several stages:
1. Input Stage: AC to DC conversion using bridge rectifier
2. Filtering Stage: Capacitive filtering
3. Regulation Stage: Multiple voltage regulators for stability
4. Control Stage: Op-amp based control circuit
5. Output Stage: Protected output with LED indicators

## Proteus Simulation Setup
1. Open Proteus ISIS Professional
2. Load the provided .DSN file
3. Configure simulation parameters:
   - Run Time: Continuous
   - Step Time: 0.1ms
   - Circuit Analysis: Transient



2. Open in Proteus ISIS Professional
3. Load the circuit file
4. Configure components as per specifications
5. Run simulation

## PCB Design Guidelines
The provided PCB layout (.LYT file) includes:
- 2-layer board design
- Ground plane on bottom layer
- Power traces: 20mil minimum
- Signal traces: 10mil minimum
- Component clearance: 0.3mm minimum

## Operation Instructions
1. Connect input power (240V AC)
2. Adjust RV1 for desired output voltage
3. Monitor LED indicators:
   - Green: Normal operation
   - Red: Fault condition
4. Use push button for output control

## Safety Precautions
- High voltage present in input stage
- Ensure proper isolation between high and low voltage sections
- Use appropriate heat sinking for regulators
- Follow proper PCB assembly guidelines

## Troubleshooting
Common issues and solutions:
1. No Output
   - Check input power
   - Verify bridge rectifier
   - Check voltage regulators

2. Unstable Output
   - Check filter capacitors
   - Verify regulator connections
   - Check feedback circuit

3. LED Indicators Not Working
   - Verify LED polarity
   - Check current limiting resistors
   - Test transistor drivers

## Future Enhancements
1. Digital voltage display
2. Current limiting feature
3. Temperature monitoring
4. Multiple output ranges
5. Digital control interface

