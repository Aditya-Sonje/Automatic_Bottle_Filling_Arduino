# Automatic_Bottle_Filling_Arduino
Arduino Code for Automatic Bottle Filling Project

🧴 Automatic Bottle Filling Machine using Arduino

An Arduino-based automation project designed to streamline the bottle filling process using IR sensors, motor control, and timed operations. This system simulates an industrial conveyor-based filling setup with high accuracy and efficiency.

📌 Project Overview

This project implements an automatic bottle filling mechanism where:

A conveyor belt (Motor 1) moves bottles forward
IR sensors detect bottle positions
A filling mechanism (Motor 2 / pump simulation) activates at the right time
The system ensures controlled and repeatable filling cycles

The goal is to demonstrate industrial automation concepts such as sequencing, sensing, and actuator control using Arduino.

⚙️ Features
🚀 Fully automated bottle detection and filling process
🎯 Filling accuracy up to ±5 ml (simulated)
🔄 Continuous operation with automatic reset
⏱️ Timed motor control for precise filling
📡 Dual IR sensor integration for position tracking
🧠 Working Principle
Motor 1 (Conveyor) starts and moves bottles forward
When IR Sensor 1 detects a bottle:
Conveyor stops
System waits for 2 seconds
Motor 2 (Filling Pump) runs for 7 seconds to fill the bottle
After filling:
Conveyor resumes after 1 second
When IR Sensor 2 detects the bottle at the end:
Conveyor stops
Once the bottle is removed:
System resets and restarts automatically
🛠️ Hardware Components
Arduino (Uno / Mega)
Adafruit Motor Shield (v1)
DC Motors (for conveyor and pump)
IR Sensors (2 units)
Power Supply
Conveyor setup (prototype)
💻 Software Requirements
Arduino IDE
AFMotor Library (Adafruit Motor Shield v1)
📂 Code Structure
Motor control using AFMotor.h
Sensor readings using analog inputs
State-based logic using flags
Delay-based timing for sequencing
🔌 Pin Configuration
Component	Arduino Pin
IR Sensor 1	A1
IR Sensor 2	A2
Motor 1	M1 (Shield)
Motor 2	M2 (Shield)
▶️ How to Run
Connect all hardware components properly
Install AFMotor Library in Arduino IDE
Upload the code to Arduino
Power the system
Place a bottle on the conveyor to start automation
📊 Applications
🥤 Beverage Industry
💊 Pharmaceutical Filling Systems
💄 Cosmetic Packaging
🏭 Small-scale Industrial Automation
📈 Future Improvements
Replace delay-based logic with non-blocking (millis())
Add LCD/Display for status monitoring
Integrate flow sensor for real-time volume measurement
Use PID control for higher precision
IoT monitoring using WiFi/Bluetooth
👨‍💻 Author

Aditya Sonje
B.Tech – Automation & Robotics
Passionate about Robotics, Automation, and Intelligent Systems

⭐ Project Highlights
Real-world inspired automation system
Strong foundation in embedded systems and control logic
Demonstrates industrial workflow simulation using Arduino
