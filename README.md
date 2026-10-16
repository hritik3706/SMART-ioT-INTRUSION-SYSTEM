# 🔐 IoT Based Security System

A smart **IoT-based security system** that detects intrusion using a **laser beam and PIR sensor**, triggers an alarm, and captures images using an **ESP32-CAM**.

---

## 📌 Overview

This project is designed to enhance security by combining **motion detection** and **laser interruption detection** to reduce false alarms. When an intrusion is detected:

- 🚨 Buzzer is activated  
- 📸 ESP32-CAM captures an image  
- 🌐 System can be extended for remote alerts  

---

## ⚙️ Features

- 🔦 Laser + LDR based intrusion detection  
- 🔥 PIR sensor for human detection (reduces false alarms)  
- 📸 Automatic image capture using ESP32-CAM  
- 🔊 Real-time buzzer alert  
- 🌐 IoT-ready (can be integrated with apps like Blynk)

---

## 🧠 Working Principle

1. A **laser beam** is continuously pointed at an LDR sensor  
2. If the beam is **broken**, it indicates possible intrusion  
3. The **PIR sensor** checks for human presence  
4. If both conditions are true:
   - Buzzer turns ON  
   - ESP32-CAM captures image  

---

## 🧰 Components Used

- NodeMCU (ESP8266)
- ESP32-CAM
- PIR Sensor
- Laser Module
- LDR (Light Dependent Resistor)
- Buzzer
- Breadboard
- Jumper Wires
- FTDI Programmer (for ESP32-CAM)
- Power Supply (5V / 3.3V)

---

## 🔌 Circuit Connections

### NodeMCU (ESP8266)
- PIR OUT → D1  
- LDR Module → A0  
- Buzzer → D2  
- VCC → 3.3V  
- GND → GND  

### ESP32-CAM
- Powered separately (5V)  
- Programmed using FTDI  
- Used only for image capture  

---

## 💻 Software & Tools

- Arduino IDE  
- ESP8266 Board Package  
- ESP32 Board Package  
- USB Drivers (CH340 / CP2102)

---

## 🚀 Getting Started

### 1️⃣ Install Arduino IDE  
Download and install Arduino IDE

### 2️⃣ Add Board URLs  
Go to Preferences and add:


http://arduino.esp8266.com/stable/package_esp8266com_index.json

https://dl.espressif.com/dl/package_esp32_index.json
