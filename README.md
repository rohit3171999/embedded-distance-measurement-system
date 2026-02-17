# 📏 Embedded Distance Measurement System – Ultrasonic Sensor

![License](https://img.shields.io/badge/license-MIT-blue)
![Platform](https://img.shields.io/badge/platform-Arduino-orange)
![Language](https://img.shields.io/badge/language-C++-blue)

An embedded distance measurement system using an ultrasonic sensor (HC-SR04) for real-time range detection and structured event-driven control logic.

---

## Table of Contents

- Project Overview
- Hardware Requirements
- Software Requirements
- Wiring Connections
- Working Principle
- Code Structure
- Documentation Requirement
- Submission Requirements
- Future Improvements
- License

---

## Project Overview

This project demonstrates distance measurement using an HC-SR04 ultrasonic sensor and Arduino (Uno R4 recommended).

The system:

- Sends ultrasonic pulse
- Measures echo time
- Calculates distance
- Displays structured serial output
- Follows Doxygen documentation standards
- Enforces Git-based development discipline

This project introduces:

- Time-of-flight measurement
- Pulse signal generation
- Distance calculation logic
- Embedded system structuring

---

## Hardware Requirements

- Arduino Uno R4
- HC-SR04 Ultrasonic Sensor
- Breadboard
- Jumper wires
- USB cable

---

## Software Requirements

- Arduino IDE
- Git
- GitHub Account

---

## Wiring Connections

| HC-SR04 Pin | Arduino |
|-------------|----------|
| VCC         | 5V       |
| GND         | GND      |
| TRIG        | Pin 9    |
| ECHO        | Pin 10   |

---

## ⚙ Working Principle

- TRIG pin sends a 10µs ultrasonic pulse.
- Sound wave travels and reflects from object.
- ECHO pin stays HIGH for duration of return time.
- Distance is calculated using time-of-flight formula:

Distance (cm) = (Duration × 0.0343) / 2

---

## Code Structure

The system:

1. Initializes Serial communication
2. Configures TRIG and ECHO pins
3. Sends ultrasonic pulse
4. Measures echo duration
5. Calculates distance
6. Prints structured output

---

## 📚 Documentation Requirement

Students must include:

- File-level Doxygen documentation block
- Function documentation for:
  - `setup()`
  - `loop()`
- Required tags:
  - `@file`
  - `@brief`
  - `@author`
  - `@date`

---

## Submission Requirements

- Minimum 5 meaningful commits
- Proper commit message format
- All TODO tasks completed
- Doxygen documentation included
- Code must compile successfully

---

## Future Improvements

- Add buzzer alert for close object
- Integrate with servo for radar scanning
- Build obstacle-avoiding robot
- Add LCD display
- IoT-based distance monitoring

---

## 📜 License

This project is licensed under the MIT License.
