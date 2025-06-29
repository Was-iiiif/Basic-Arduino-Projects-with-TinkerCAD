# 🌓 Analog Input Dimmer Circuit using Arduino

## 🔧 Project Overview

This project demonstrates a **simple analog dimmer circuit** using an Arduino. It reads analog input from a potentiometer (or any analog sensor) and adjusts the brightness of an LED or the speed of a motor using **PWM (Pulse Width Modulation)**. The project is ideal for beginners learning analog-digital interfacing and PWM control.

---

## ⚙️ Features

- Reads analog input voltage (0–5V) from pin `A0`
- Scales analog input (0–1023) to PWM output range (0–255)
- Outputs PWM signal on digital pin `9`
- Real-time serial output of PWM values for monitoring

---

## 🔩 Components Used

| Component          | Quantity | Description                                |
|-------------------|----------|--------------------------------------------|
| Arduino Uno/Nano  | 1        | Microcontroller board                      |
| Potentiometer     | 1        | Variable resistor for analog input         |
| LED / Motor       | 1        | Output device for dimming/speed control    |
| Resistor (220Ω)   | 1        | Protects LED from overcurrent              |
| Breadboard        | 1        | For assembling the circuit                 |
| Jumper Wires      | As needed| For making connections                     |

---

## 🔌 Circuit Connections

| Arduino Pin | Connected To                 |
|-------------|------------------------------|
| A0          | Middle pin of potentiometer  |
| GND         | Potentiometer GND / LED –    |
| 5V          | Potentiometer VCC            |
| D9 (PWM)    | LED + / Motor input (via resistor if LED) |

---

## 📌 Applications

Light dimmers

Fan/motor speed controllers

Analog sensor data visualization

PWM-based control systems
