
# 🔥 IoT-Based Fire & Gas Safety System using ESP32

## 📌 Overview

An IoT-based fire and gas safety system designed to detect smoke, harmful gases and fire using an ESP32 microcontroller. The system provides local audio alerts and remote notifications to improve emergency awareness.

## 🎯 Features

- 🔥 Flame detection using a flame sensor
- 💨 Smoke and gas detection using MQ-2 sensor
- 🔊 Audible buzzer alert
- 🗣️ Voice alerts using DFPlayer Mini
- 📱 Telegram emergency notifications
- 📊 Real-time monitoring using Blynk
- 🌐 Web dashboard for monitoring and control
- 📍 GPS location tracking integration
- 🔄 Online and offline alert functionality

## 🧰 Hardware Components

- ESP32 Dev Module
- MQ-2 Gas Sensor
- Flame Sensor
- DFPlayer Mini
- Speaker
- Buzzer
- 16x2 I2C LCD
- GPS Module (NEO-6M)
- Connecting wires
- Power supply

## ⚙️ Working Principle

1. The MQ-2 sensor monitors smoke and gas levels.
2. The flame sensor detects the presence of fire.
3. The ESP32 processes the sensor readings.
4. When a hazardous condition is detected, the buzzer and voice alert system activate.
5. Telegram sends emergency notifications when network connectivity is available.
6. Blynk and the web dashboard provide remote monitoring.
7. The system supports local alerts when internet connectivity is unavailable.

## 🧠 System Architecture

Sensors → ESP32 → Alert System

ESP32 → Telegram Notifications

ESP32 → Blynk IoT Platform

ESP32 → Web Dashboard

ESP32 → GPS Location Tracking

## 💻 Technologies Used

- C++
- ESP32
- Arduino IDE
- IoT
- Blynk
- Telegram Bot API
- GPS
- Embedded Systems

## 🚀 Project Goals

- Improve fire and gas hazard awareness
- Provide immediate local alerts
- Enable remote monitoring
- Support offline alert functionality

## 👨‍💻 Developer

Marella Radha Krishna

Electronics and Communication Engineering

Interested in Embedded Systems, IoT and Firmware Development.

## System Diagrams

### System Architecture
[View System Architecture](diagrams/system_architecture.md)

### System Flowchart
[View System Flowchart](diagrams/flowchart.md)

### State Machine Diagram
[View State Machine Diagram](diagrams/state_machine.md)
