# ESP32-Diode-Signal-Detector-
A simple ESP32-based diode signal detector that monitors voltage states (HIGH/LOW) and logs results via Serial.Ideal for basic polarity/voltage detection in DIY electronics projects
# ESP32 Diode Signal Detector

## Overview
This project uses an ESP32 to detect voltage states (HIGH/LOW) after a diode, printing results to the Serial Monitor. Useful for verifying signal polarity or basic voltage monitoring.

## Circuit Setup
- *Components*:
  - ESP32 (e.g., ESP32-WROOM)
  - Diode (e.g., 1N4148)
  - Pull-down resistor (10kΩ recommended)
- *Wiring*:
  - Diode anode → Signal source
  - Diode cathode → GPIO 25
  - Resistor between GPIO 25 and GND

## Code
- Reads digitalRead() on GPIO 25.
- Prints "High voltage detected!" or "No high voltage detected (safe)" to Serial (115200 baud).
