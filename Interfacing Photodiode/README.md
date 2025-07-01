# 📸 Interfacing Photodiode

This project demonstrates how to use a **photodiode** with an Arduino UNO to detect ambient light intensity. The sensor reads analog voltage changes based on light exposure and displays the values in the Serial Monitor.

## 📷 Project Overview

A **photodiode** is a semiconductor device that generates a voltage or current when exposed to light. In this project, the photodiode is connected in a **voltage divider** configuration with a resistor. The Arduino reads the analog voltage at the junction and interprets the light level.

## 🔧 Components Used

| Component       | Quantity | Description                            |
|----------------|----------|----------------------------------------|
| Arduino UNO     | 1        | Microcontroller board                  |
| Photodiode      | 1        | Light sensor                           |
| 10kΩ Resistor   | 1        | Used in voltage divider with photodiode|
| Jumper Wires    | 3+       | For circuit connections                |

## 🔌 Circuit Diagram

- The photodiode is used in a reverse-biased configuration with a resistor to form a voltage divider.
- One end of the photodiode is connected to **5V**
- The other end is connected to:
- Analog pin **A0**
- One end of a **10kΩ resistor**, whose other end is connected to **GND**

## 💡 How It Works

- In bright light, the photodiode allows more current to pass.
- This changes the voltage at the analog pin.
- The Arduino reads this voltage (0–5V) as an integer (0–1023).
- The Serial Monitor displays the corresponding value in real time.

## 🧠 Applications
- Light-based security systems
- Optical communication
- Infrared detection
- Object sensing and counters
