# 🔢 Simple Calculator

This project is a simple calculator built with **Arduino Uno**, a **16x2 LCD (parallel)**, and a **4x4 matrix keypad**. It can perform basic arithmetic operations: addition, subtraction, multiplication, and division.

---
## ✅ Features

- 4 basic operations: `+`, `-`, `*`, `/`
- LCD-based interactive interface
- Real-time keypad input handling
- Input clearing (`C`)

## 🛠 Components Used

| Component            | Quantity |
|----------------------|----------|
| Arduino Uno          | 1        |
| 16x2 LCD Display     | 1        |
| 4x4 Matrix Keypad    | 1        |
| Jumper Wires         | Many     |
| Breadboard           | 1        |
| Resistor (1kΩ)  | 1        |

---

## 🔌 Circuit Connections

### LCD (16x2 Parallel Mode)
| LCD Pin | Arduino Pin |
|---------|-------------|
| RS      | 13          |
| EN      | 12          |
| D4      | 11           |
| D5      | 10          |
| D6      | 9          |
| D7      | 8           |
| GND     | GND         |
| VCC     | 5V          |
| VO      | GND |
| RW      | GND         |
| LED (Backlight +) | 5V  |
| LED (Backlight -) | GND with Resistor |

### Keypad
| Row/Col | Arduino Pin |
|---------|-------------|
| R1      | 7          |
| R2      | 6          |
| R3      | 5          |
| R4      | 4          |
| C1      | 3          |
| C2      | 2          |
| C3      | 1           |
| C4      | 0           |

---

## 🧠 How It Works

- User inputs a number using the keypad
- Presses an operator (`+`, `-`, `*`, `/`)
- Inputs the second number
- Presses `=` to view the result
- Press `C` to clear/reset



