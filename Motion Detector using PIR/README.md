# 🚨 Motion-Controlled RGB LED Siren using Arduino

This project is a motion-activated RGB lighting system with a high-frequency siren sound using an Arduino, a PIR motion sensor, a piezo buzzer, and RGB LEDs.

When motion is detected:
- A **siren sound** plays through the buzzer.
- All RGB LEDs turn **blue**.
- When idle, RGB LEDs glow **purple**.

---

## 📷 Project Overview

![Circuit Diagram](<insert your image link here>)

---

## 📦 Components Used

| Component             | Quantity | Description                                      |
|-----------------------|----------|--------------------------------------------------|
| Arduino Uno           | 1        | Microcontroller board                            |
| PIR Motion Sensor     | 1        | Detects motion, triggers LEDs & buzzer          |
| RGB LEDs (Common Cathode) | 3    | Displays different colors                        |
| Piezo Buzzer          | 1        | Emits siren sound                                |
| 220Ω Resistors        | 9        | For limiting current to RGB LED pins            |
| Breadboard            | 1        | For assembling components                        |
| Jumper Wires          | ~15      | To connect components on the breadboard          |
| USB Cable             | 1        | For uploading code and powering Arduino          |

---

## 🔌 Circuit Connections

| Arduino Pin | Connected To        | Component     |
|-------------|---------------------|---------------|
| 13           | PIR OUT             | PIR Sensor    |
| 9           | RGB LED 1 RED       | LED #1        |
| 10           | RGB LED 1 GREEN     | LED #1        |
| 11           | RGB LED 1 BLUE      | LED #1        |
| 9           | RGB LED 2 RED       | LED #2        |
| 10          | RGB LED 2 GREEN     | LED #2        |
| 11          | RGB LED 2 BLUE      | LED #2        |
| 9          | RGB LED 3 RED       | LED #3        |
| 10          | RGB LED 3 GREEN     | LED #3        |
| 11          | RGB LED 3 BLUE      | LED #3        |
| 12          | Positive leg of buzzer | Buzzer   |
| GND         | Common ground rail  | All           |
| 5V          | VCC for PIR + LEDs  | All           |

---

## 💡 Features

- Motion detection via PIR sensor.
- Siren effect using piezo buzzer.
- RGB LED color change based on motion state.
- Visual + sound alert system.

---

## 🧠 How It Works

1. **PIR detects motion** → Digital HIGH on pin 2.
2. Triggers `sirenEffect()` → A sweeping frequency sound.
3. RGB LEDs display a **blue alert** color.
4. When **no motion** → LEDs revert to **purple**.

---
