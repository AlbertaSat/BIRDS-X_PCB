# JASPER BIRDS-X_PCB
Repository for the PCB design for the JASPER BIRDS-X project.

JASPER is a joint organization between the University of Alberta's AlbertaSat and the University of Calgary's CalgaryToSpace cubesat teams.

## Features
1. Capable of APRS (Automated Packet Reporting System) digipeat and store-and-forward modes, for use by Amateur Radio enthusiasts.
2. Implements a radiation experiment, which compares the radiation shielding properties of shielding options.
	* Uses RADFET sensors and PIN diodes as radiation detection sensors.
3. Employs power safety systems (over-current protection, enable pins, etc.) to interface with the BIRDS-X satellite parent system.
4. Uses <300 mW on receive, and <1750 mW on transmit.
5. Stores data in flash memory.
6. Interfaces with the Mission Boss system via UART.
7. A test fixture board makes flashing and debugging the main payload board easier.

## Release Notes

### Rev1.0
* Rev1.0 is a pre-release board that neared completion, but was never finished nor ordered. It includes several design flaws (inappropriate RF transceiver, lacked PIN Diode system, lacked concurrent reading circuitry for radfets), and was iterated on before a PCB was ordered.

### Rev2.0
* SX1276-based board.


#### Rev2 Notes and Errata

1. Board outline is wrong.
2. C532 should be a 47pF cap. It was factory-populated as a 4.7pF cap.
3. Should have added SWITCH_CTRL to J502.

### Rev3.0
* DRA818V-based board, with 2 MCUs.
	* STM32G01K8
	* STM32L432
* Intended to run NucleoTNC, but was unsuccessful.

### Rev4.0
* DRA818V-based board, with 1 MCU.
* Semi-final release.
* Runs a fork of [vp-digi](https://github.com/sq8vps/vp-digi) on an STM32F103C8T6 MCU.
* Manufactured on 1.6mm PCB, with immpedance controlled `JLC04161H-7628` stackup from JLCPCB.

