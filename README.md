# 6T SRAM Cell Design and Simulation

## Overview
This repository contains the design and transient simulation of a standard 6-Transistor (6T) Static Random Access Memory (SRAM) cell. The design was implemented and verified using Cadence Virtuoso and the Spectre simulation environment.

## Technology Node
* **Process:** Generic Process Design Kit (GPDK) 45nm
* **Operating Voltage (VDD):** 1.1V

## Transistor Sizing
The cell is designed with specific Width/Length (W/L) ratios to ensure stable read and write margins.
* **Pull-Down (NMOS):** W = 120nm, L = 45nm
* **Pull-Up (PMOS):** W = 120nm, L = 45nm
* **Access (NMOS):** W = 120nm, L = 45nm


## Transient Analysis
The cell was subjected to transient analysis to verify its fundamental operations:
1.  **Write Operation:** Forcing the bitlines and asserting the Wordline (WL) to flip the internal storage nodes.
2.  **Hold State:** De-asserting WL to ensure the cross-coupled inverters retain the data indefinitely.
3.  **Read Operation:** Asserting WL and observing the bitline discharge without destroying the stored internal state.


## Tools Used
* Cadence Virtuoso Schematic Editor
* Analog Design Environment (ADE XL)
* Spectre Circuit Simulator
