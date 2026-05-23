# CiS UV Project

## Mission Overview
This project is an autonomous 4cm cube data logger designed for stratospheric research below 23 miles. The mission compares the accuracy of low-cost analog and digital UV sensors against official NASA solar irradiance benchmarks. The device operates within a strictly unmodified Cubes in Space polycarbonate enclosure to evaluate sensor sensitivity to shielded radiation.

## Technical Specifications
*   **Microcontroller:** STM32L031K6T6 (Ultra-low-power ARM Cortex-M0+)
*   **Altitude Sensor:** Bosch BMP280 barometric pressure sensor
*   **Digital UV Sensor:** LTR390-UV (I2C interface)
*   **Analog UV Sensor:** GUVA-S12SD Phototransistor
*   **Storage:** Dual 24LC256 I2C EEPROMs for redundant data logging
  *These specs are not final*

## Operational Logic
The system is programmed for 100% autonomous operation. Upon initial power-up, the MCU enters a deep-sleep hibernation to preserve energy. Once the mission window begins, the altitude sensor triggers data collection at specific atmospheric pressure thresholds (10, 15, and 20 miles). Data is formatted into a text-based template and stored across two independent memory chips to prevent data loss from cosmic radiation or hardware failure.

## Experiment Variables
*   **Independent Variable:** UV sensor technology (Analog Phototransistor vs. Digital UV Detector)
*   **Dependent Variable:** Recorded solar UV radiation intensity (Watts per square meter)
*   **Control:** Identical altitude triggers and shielding environment

Contact me [here](vivaan.bobade@icloud.com)
