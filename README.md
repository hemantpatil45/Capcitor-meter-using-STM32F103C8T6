# STM32F401RE Capacitor Meter

## Project Overview

This project aims to develop a simple and accurate capacitor meter utilizing the STM32F401RE microcontroller. The core principle involves measuring capacitance by analyzing the charging characteristics of an RC (Resistor-Capacitor) circuit. By precisely timing how long it takes for an unknown capacitor to charge to a specific voltage level using the microcontroller's ADC, its capacitance can be determined.

## Current Status

**Work in Progress (WIP)**. This repository currently contains initial circuit designs and simulation results. I am actively working on:
* Refining the circuit design.
* Developing the STM32F401RE firmware.
* Implementing ADC readings and time measurements.
* Calibrating the system for accuracy.

## Circuit Design (LTspice)

The primary circuit relies on a resistor-capacitor (RC) network.
* [cite_start]**Resistor:** 10 MOhms [cite: 4, 14, 48, 58]
* [cite_start]**Voltage Source:** 5V DC with a series resistance of 10 Ohms (Rser=10) [cite: 6, 7, 16, 17, 50, 52, 60, 62]
* [cite_start]**Capacitor:** Variable, with simulations demonstrating charging for values like 100pF [cite: 8][cite_start], 140pF [cite: 17][cite_start], 1nF [cite: 51][cite_start], and 2nF[cite: 61].
* [cite_start]The voltage at the "Microcontroller_Input_Pin" is observed for measurement[cite: 10, 19, 54, 64].

### Simulation Files

* [cite_start]`Draft2.asc` (LTspice schematic files, containing circuits for C=100p, C=140p, C=1n, C=2n examples) [cite: 20, 65]
* *(Optional: You might consider including screenshots of key simulation plots in an `images/` folder instead of large .raw files if they're not critical for others to re-run directly.)*

## Next Steps

* Complete firmware development for the STM32F401RE.
* Hardware prototyping (e.g., breadboard, custom PCB).
* Thorough testing and calibration.

## Contributions

Feel free to open issues or provide suggestions as I progress with the project!

## License

*(Choose an appropriate open-source license, e.g., MIT License, Apache 2.0 License. You'd typically include a separate `LICENSE` file in your repository.)*
