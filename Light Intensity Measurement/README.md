# 🌞 Light Intensity Measurement with Arduino

This project demonstrates how to measure ambient light using an LDR (Light Dependent Resistor) and an Arduino, and dynamically adjust the brightness of an LED based on the light level. Real-time sensor data is displayed through the Serial Monitor.

---

## 🧰 Components Used

| Component         | Quantity | Purpose                            |
|------------------|----------|------------------------------------|
| Arduino Uno       | 1        | Microcontroller board              |
| LDR (Photoresistor)| 1       | Light sensing                      |
| 10kΩ Resistor     | 1        | Forms voltage divider with LDR     |
| LED               | 1        | Light output (brightness control)  |
| Breadboard        | 1        | Circuit assembly                   |
| Jumper Wires      | As Needed        | Connections                        |
| USB Cable         | 1        | Uploading code & power supply      |

---

## 🔌 Pin Configuration

| Arduino Pin | Connected To              |
|-------------|---------------------------|
| A5          | Middle node of LDR + 10kΩ |
| 5V          | One end of LDR            |
| GND         | One end of 10kΩ resistor  |
| 9 (PWM)     | Positive leg of LED       |
| GND         | Negative leg of LED (via resistor) |

---

## 🔧 Circuit Description

The LDR and a 10kΩ resistor form a **voltage divider**. The Arduino reads the analog voltage at pin **A5**, which varies based on light intensity. This value is mapped to PWM output and used to adjust the brightness of an LED connected to **pin 9**.

## 🎯 Applications

Light-sensitive streetlights

Smart home lighting systems

Light data logging

Ambient mood lighting
