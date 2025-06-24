# 🔌 Arduino Digital Voltmeter

This project demonstrates how to build a simple **digital voltmeter** using an Arduino Uno, a 16x2 LCD (non-I2C), and a voltage divider circuit to measure higher voltages safely.

---

## 📷 Project Overview

The system reads an analog voltage from a voltage divider connected to an external source and displays the corresponding voltage on a 16x2 LCD screen. This is useful for monitoring voltages above 5V by scaling them down within Arduino's readable range.

---

## ⚙️ Features

- Displays measured voltage in real-time on an LCD
- Serial output for debugging or logging
- Customizable resistor values for different voltage ranges
- Contrast-adjustable LCD via potentiometer

---

## 🛠️ Components Used

| Component              | Quantity |
|------------------------|----------|
| Arduino Uno            | 1        |
| 16x2 LCD (standard)    | 1        |
| 10kΩ Potentiometer     | 1        |
| Resistors (e.g., 90.9k & 10k) | 2        |
| Breadboard             | 1        |
| Jumper wires           | —        |
| External power source (e.g. variable power supply) | 1        |

---


### LCD Pin Connection (Using LiquidCrystal)
| LCD Pin | Arduino Pin |
|---------|-------------|
| RS      | 13           |
| E       | 12           |
| D4      | 11          |
| D5      | 10          |
| D6      | 9          |
| D7      | 8          |
| VSS     | GND         |
| VDD     | 5V          |
| V0      | Potentiometer middle pin |
| RW      | GND         |

---



