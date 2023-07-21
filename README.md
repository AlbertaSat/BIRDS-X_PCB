# BIRDS-X_PCB
Repository for the PCB design for the BIRDS-X project.

## Features
1. Capable of APRS (Automated Packet Reporting System) digipeat and store-and-forward modes, for use by Amateur Radio enthusiasts.
2. Employs a RADFET-based radiation experiment, which compares the radiation shielding properties of shielding options.
3. Employs power safety systems to interface with the BIRDS-X satellite parent system.

## Release Notes

### Rev1.0
* Rev1.0 is a pre-release board that neared completion, but was never finished nor ordered. It includes several design flaws (inappropriate RF transceiver, lacked PIN Diode system, lacked concurrent reading circuitry for radfets), and was iterated on before a PCB was ordered.

### Rev2 Notes and Errata

1. Board outline is wrong.
2. C532 should be a 47pF cap. It was factory-populated as a 4.7pF cap.
3. Should have added SWITCH_CTRL to J502.
