# 🌞 Digital Solar Tracker

This project demonstrates a **Dual-Axis Light Tracking System** using an Arduino, two servos, and four LDRs. The system detects the brightest light source (such as the sun) and automatically aligns itself to maximize light exposure. It's ideal for solar panel tracking or light-following robotics.

---

## ⚙️ Features

- Dual-axis movement (horizontal and vertical)
- Automatic adjustment to the strongest light direction
- Smooth and gradual servo motion
- Real-time light intensity feedback via Serial Monitor
- Adjustable sensitivity and movement step size

---

## 🔩 Components Used

| Component                     | Quantity | Pin Connections               |
|-------------------------------|----------|--------------------------------|
| Arduino Uno / Nano            | 1        | -                              |
| Servo Motor                   | 2        | 9 (Horizontal), 10 (Vertical)  |
| LDR (Light Dependent Resistor) | 4        | A0 (BR), A1 (TR), A2 (TL), A3 (BL) |
| 10kΩ Resistors                | 4        | Pull-down for each LDR         |
| Jumper Wires                  | Several  | -                              |
| Breadboard / Mount Base       | 1        | -                              |
| Power Supply (5V)             | 1        | -                              |


---

## 🛠️ How It Works

- Four LDR sensors are placed at the four corners of the panel.
- The Arduino reads analog values from the sensors.
- Calculates the **average light intensity** for top/bottom and left/right sides.
- If the difference exceeds a set threshold, it moves the respective servo to align the panel.
- Adjustable parameters:
  - **Threshold:** Prevents minor fluctuations from triggering motion.
  - **Step Size:** Controls how far the servos turn each time.

---

## 🚀 Setup Instructions

1. Wire the circuit according to the pin configuration.
2. Upload the provided Arduino sketch.
3. Open the Serial Monitor at **9600 baud** to observe real-time LDR readings.
4. Shine a flashlight or place under the sun to see the tracking in action.

---

## 🔧 Adjustable Parameters in Code

| Parameter   | Default | Description                             |
|-------------|---------|-----------------------------------------|
| threshold   | 50      | Minimum light difference to move servo |
| stepSize    | 5       | Angle to move per update (1–10 recommended) |

---

## 📈 Future Improvements

- Add PID control for smoother alignment
- Integrate real-time clock (RTC) for hybrid time-based tracking
- Add manual override using buttons
- Solar charging & battery management system




