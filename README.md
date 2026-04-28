# 🧴 Automatic Bottle Filling Machine using Arduino

**Arduino Code for Automatic Bottle Filling Project**

An Arduino-based automation project designed to streamline the bottle filling process using IR sensors, motor control, and timed operations. This system simulates an industrial conveyor-based filling setup with high accuracy and efficiency.

---

## 📌 Project Overview

This project implements an automatic bottle filling mechanism where:

- A conveyor belt (Motor 1) moves bottles forward  
- IR sensors detect bottle positions  
- A filling mechanism (Motor 2 / pump simulation) activates at the right time  
- The system ensures controlled and repeatable filling cycles  

The goal is to demonstrate industrial automation concepts such as **sequencing, sensing, and actuator control using Arduino**.

---

## ⚙️ Features

* 🚀 Fully automated bottle detection and filling process  
* 🎯 Filling accuracy up to **±5 ml (simulated)**  
* 🔄 Continuous operation with automatic reset  
* ⏱️ Timed motor control for precise filling  
* 📡 Dual IR sensor integration for position tracking  

---

## 🧠 Working Principle

1. **Motor 1 (Conveyor)** starts and moves bottles forward  
2. When **IR Sensor 1** detects a bottle:  
   - Conveyor stops  
   - Waits for 2 seconds  
3. **Motor 2 (Filling Pump)** runs for 7 seconds  
4. After filling:  
   - Conveyor resumes after 1 second  
5. When **IR Sensor 2** detects the bottle:  
   - Conveyor stops  
6. Once the bottle is removed:  
   - System resets and restarts automatically  

---

## 🛠️ Hardware Components

- Arduino (Uno / Mega)  
- Adafruit Motor Shield (v1)  
- DC Motors (Conveyor + Pump)  
- IR Sensors (2 units)  
- Power Supply  
- Conveyor setup (prototype)  

---

## 💻 Software Requirements

- Arduino IDE  
- AFMotor Library (Adafruit Motor Shield v1)

---

## 🔌 Pin Configuration

| Component     | Pin        |
|--------------|-----------|
| IR Sensor 1  | A1        |
| IR Sensor 2  | A2        |
| Motor 1      | M1 Shield |
| Motor 2      | M2 Shield |

---

## ▶️ How to Run

- Connect all hardware components
- Install AFMotor Library in Arduino IDE
- Upload the code to Arduino
- Power the system
- Place a bottle on the conveyor

---

## 📊 Applications
- 🥤 Beverage Industry
- 💊 Pharmaceutical Filling Systems
- 💄 Cosmetic Packaging
- 🏭 Small-scale Industrial Automation

---

## 📈 Future Improvements
- Replace delay() with millis() (non-blocking logic)
- Add LCD display for monitoring
- Integrate flow sensor for real-time volume measurement
- Implement PID control for higher precision
- Add IoT monitoring (WiFi/Bluetooth)

---

## 👨‍💻 Author

Aditya Sonje
B.Tech – Automation & Robotics
