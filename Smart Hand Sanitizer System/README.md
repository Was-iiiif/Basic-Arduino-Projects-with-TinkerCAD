# 🤖 Smart Hand Sanitizer Dispenser using Arduino

This project is a contactless hand sanitizer dispenser built with an Arduino, ultrasonic sensor, and servo motor. It detects your hand under the sanitizer nozzle and automatically presses the pump using a servo — perfect for hygiene in public or home spaces.

---

## 🚀 Features

- ✅ Contactless operation
- ✅ Automatically dispenses sanitizer when hand is detected
- ✅ Adjustable detection range
- ✅ Low-cost, easy to build
- ✅ Compact and Arduino-compatible

---

## 🧰 Components Required

| Component             | Quantity |
|-----------------------|----------|
| Arduino Uno/Nano      | 1        |
| Ultrasonic Sensor (HC-SR04) | 1        |
| Servo Motor (e.g., SG90)     | 1        |
| Breadboard + Jumper Wires   | As needed |
| Sanitizer Bottle with Pump  | 1        |
| External 5V Power Source (optional for servo) | 1 |
| (Optional) 3D-printed/DIY frame | 1 |

---

## 🔌 Wiring Diagram

| Component        | Arduino Pin | Notes                         |
|------------------|-------------|-------------------------------|
| HC-SR04 Trigger  | D8          | Output pin to trigger signal |
| HC-SR04 Echo     | D9          | Input pin to read distance   |
| Servo Signal     | D6          | PWM pin for servo control    |
| VCC (All modules)| 5V          | Use external power for servo if needed |
| GND (All modules)| GND         | Common ground                 |

---

## 🧠 How It Works

1. The **ultrasonic sensor** continuously measures the distance below the nozzle.
2. If a hand is detected within **10 cm**, the **servo rotates to press the sanitizer pump**.
3. After dispensing, the servo returns to its original position.
4. A cooldown delay ensures it doesn’t trigger multiple times rapidly.

---


