# LCD Display with ATtiny85

This project demonstrates how to interface an **ATtiny85 microcontroller** with a **16x2 LCD display** using a breadboard setup. The circuit is powered by a 9V battery and displays data on the LCD screen.

---

## 🧾 Project Overview

The goal of this project is to display simple messages on an LCD using the ATtiny85 microcontroller. It's a compact and efficient solution for embedded systems or low-power applications.

---

## 🧰 Components Used

| Component           | Quantity | Description                                      |
|--------------------|----------|--------------------------------------------------|
| ATtiny85           | 1        | 8-pin microcontroller                            |
| LCD Display (16x2) | 1        | Alphanumeric LCD (HD44780-compatible)            |
| Resistors (220Ω)   | 2        | One for ATtiny85, one for LCD backlight          |
| Breadboard         | 1        | For prototyping                                  |
| Jumper Wires       | 15+      | Male-to-male jumper wires                        |
| 9V Battery         | 1        | Power source                                     |

---

## 🔌 Circuit Description

- ATtiny85 controls the LCD in **4-bit mode**.
- A potentiometer is used to adjust contrast via the V0 pin.
- Power is supplied via a 9V battery connected to the breadboard rails.
- LCD backlight is controlled with a current-limiting resistor.

---

## 📟 LCD Pin Connections

| LCD Pin | Function         | ATtiny Pin |
|---------|------------------|------------|
| VSS     | GND              | GND        |
| VDD     | +5V              | VCC        |
| V0      | Contrast Control | GND        |
| RS      | Register Select  | Pin 0      |
| EN      | Enable           | Pin 1      |
| D4      | Data Bit 4       | Pin 2      |
| D5      | Data Bit 5       | Pin 3      |
| D6      | Data Bit 6       | Pin 4      |
| D7      | Data Bit 7       | Pin 5      |
| LED+    | Backlight +      | +5V (with 1kΩ) |
| LED-    | Backlight -      | GND        |

---

