# ESP32-Based WiFi Controlled Robotic Car with Motor Control

## Overview
This project demonstrates the design and implementation of a WiFi-controlled
robotic car using an ESP32 microcontroller, DC motors, a motor driver module,
and IR sensors. The system focuses on embedded motor control, real-time command
processing, and sensor-based decision logic.

The robotic car supports directional movement, speed control, rotation, and
sensor-driven navigation through embedded firmware executed on the ESP32.

---

## Objective
To develop a microcontroller-based robotic system capable of:
- Wireless motor control using WiFi
- Speed variation and directional movement
- Integration of sensors for navigation logic
- Reliable hardware–software coordination

---

## Hardware Components
- ESP32 development board
- L298N motor driver module
- DC motors with wheels
- IR sensors (left and right)
- Battery power supply (7–12V)
- Robot chassis and wiring

---

## System Architecture
The ESP32 acts as the central controller, receiving WiFi-based control commands
and processing sensor inputs. Based on the received commands and sensor data,
the ESP32 generates appropriate control signals for the L298N motor driver,
which drives the DC motors accordingly.

Two IR sensors provide input for navigation logic, enabling the system to
adjust movement based on surface detection.

---

## Functional Capabilities
- Forward, backward, left, and right motion control
- Speed variation using PWM-based motor control
- Rotation and smooth directional turning
- IR-sensor-based navigation logic implemented in firmware
- WiFi-based command handling through an embedded web server

---

## Communication
- WiFi communication using an embedded HTTP server
- Commands are sent as control parameters and interpreted by the ESP32
- UART used for debugging and monitoring during development

---

## Workflow
1. System powers on and initializes ESP32 and motor driver
2. ESP32 establishes WiFi communication
3. Control commands are received wirelessly
4. Sensor inputs are read and processed
5. Motor control signals are generated
6. L298N driver actuates motors based on logic decisions

---

## Implementation Notes
- Embedded firmware is written in C/C++ using Arduino-compatible ESP libraries
- Motor speed is controlled using PWM signals
- The repository focuses on embedded logic, system integration, and control flow
- A demonstration video is included to show real-world operation

---

## Demo
A working demonstration of the robotic car showing motion control and speed
variation is included directly in this repository.
