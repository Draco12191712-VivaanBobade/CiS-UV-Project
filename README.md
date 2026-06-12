# CiS UV Project

## Mission Overview
This project is an autonomous 4cm CiS cube data logger designed for stratospheric research below 23 miles. The mission compares the accuracy of low-cost analog and digital UV sensors against official NASA solar irradiance benchmarks.

## Technical Specifications
*   **Microcontroller:** Adafruit QT Py ESP32-S3
*   **Altitude Sensor:** Bosch BMP388 barometric pressure sensor
*   **Digital UV Sensor:** LTR390-UV (I2C interface)
*   **Analog UV Sensor:** GUV-S12SD Phototransistor

## Operational Logic
The system is programmed for 100% autonomous operation. Upon initial power-up, the MCU enters a deep-sleep hibernation to preserve energy. Once the mission window begins, the altitude sensor triggers data collection at specific atmospheric pressure thresholds (10, 15, and 20 miles). Data is formatted into a text-based template and stored in the 8MB flash of the MCU. It is stored as a .csv or .txt file.

## Experiment Variables
*   **Independent Variable:** UV sensor technology (Analog Phototransistor vs. Digital UV Detector)
*   **Dependent Variable:** Recorded solar UV radiation intensity (Watts per square meter)
*   **Control:** Identical altitude triggers and shielding environment

Contact me [here](https://mail.google.com/mail/u/0/#inbox?compose=CllgCJlKnPFPVLQjcsljjzhmlWcqJcHHqMGgTwCpJXrgkwkLzLtTHTZzZfDFtzpMlHJpBmxJPVV)
