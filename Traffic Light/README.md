# 🚦 Simple Traffic Light System with Pedestrian Button

This Arduino project simulates a basic traffic light system that includes a pedestrian crossing button. When the button is pressed, the system temporarily interrupts the green light, activates yellow and red signals to stop traffic, and then resumes the normal green light flow.

---

## 🔧 Components Used

| Component       | Quantity | Description                           |
|----------------|----------|---------------------------------------|
| Arduino UNO     | 1        | Microcontroller board                 |
| LED (Red)       | 1        | Represents STOP signal (pin 8)        |
| LED (Yellow)    | 1        | Represents WAIT signal (pin 9)        |
| LED (Green)     | 1        | Represents GO signal (pin 10)         |
| Push Button     | 1        | Pedestrian request button (pin 11)    |
| 220Ω Resistors  | 3        | Current limiting resistors for LEDs   |
| Breadboard      | 1        | For prototyping                       |
| Jumper Wires    | Several  | For connections                       |

---

## ⚙️ Circuit Diagram

| Arduino Pin | Connected To         |
|-------------|----------------------|
| D8          | Red LED (via resistor)     |
| D9          | Yellow LED (via resistor)  |
| D10         | Green LED (via resistor)   |
| D11         | One leg of push button     |
| GND         | Other side of LEDs + button|
| 5V          | Pull-up input for button  |


---

## 🧠 Code Behavior

- **When the button is not pressed:** Green LED stays on, indicating normal traffic flow.
- **When the button is pressed:**
  - Green LED turns off.
  - Yellow LED turns on for 2 seconds.
  - Then Red LED turns on for 5 seconds (indicating cars must stop).
  - After 5 seconds, the Red LED turns off and Green resumes.

---

