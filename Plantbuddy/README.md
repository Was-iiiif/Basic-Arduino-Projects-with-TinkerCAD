# 🌿 PlantBuddy – Smart Garden Management System

**PlantBuddy** is a fully automatic Arduino-based system that rotates a plant toward sunlight and waters it based on soil moisture — all while displaying real-time plant status on an LCD screen.

---

## 🔥 Features

- 🔁 Dual-axis light tracking using 4 LDR sensors
- 💧 Automatic watering via soil moisture sensor
- 📟 LCD display showing real-time H/V sunlight angles and water status
- 💡 Clean, step-wise servo logic for smooth plant rotation
- 🧪 Fully simulated using TinkerCAD Circuits

---

## 🧠 Inspiration

Inspired by **heliotropism** (plants turning toward light), this project merges natural behavior with electronics and code to create an intelligent garden assistant.

---

## 🛠️ Components Used

| Component              | Description                     |
|------------------------|---------------------------------|
| Arduino Uno            | Main microcontroller            |
| 4x LDR Sensors         | Light detection from 4 directions |
| 2x Servo Motors        | Plant rotation (X and Y axes)   |
| Soil Moisture Sensor   | Triggers watering               |
| 16x2 LCD Display       | Status output                   |
| Resistors | Contrast & LDR circuits     |
| LED, DC Motor and Relay   | Indicates watering action       |

---


## 🧾 Code Summary

- LDRs calculate light intensity difference (left/right, top/bottom)
- Servos rotate plant in the direction of strongest light
- Moisture is continuously monitored and water pump LED activates when dry
- LCD prints sunlight angle and watering status

---

## 🌱 Future Upgrades

- Add DHT11 (temperature/humidity)
- Use real water pump with relay module
- WiFi (ESP8266) for mobile control
- RTC module for time-based watering
- Solar power integration
