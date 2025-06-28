# Thermometer Using ATTiny85 

This project uses an ATTiny85 microcontroller and a TMP36 temperature sensor to control an LED. The LED blinks at different rates based on the surrounding temperature.

## 📌 Features

- Reads ambient temperature using a TMP36 sensor
- Converts analog input into degrees Celsius
- Blinks an LED at different speeds depending on the temperature range:
  - 🔹 Fast blink (100ms) for temperatures between **-40°C and 69°C**
  - 🔸 Medium blink (500ms) for **70°C to 116°C**
  - 🔴 Slow blink (1000ms) for **117°C to 238°C**

---

## ⚙️ Components Used

| Component          | Quantity |
|-------------------|----------|
| ATTiny85           | 1        |
| TMP36 Temperature Sensor | 1        |
| LED (Red)          | 1        |
| Resistor (220Ω)    | 1        |
| AA Battery (1.5V)  | 3        |
| Battery Holder     | 1        |
| Breadboard & Wires | As needed |

---


## 🧠 How It Works

1. The TMP36 outputs a voltage proportional to the ambient temperature.
2. The ATTiny85 reads this voltage using its analog input (A1).
3. The code converts this voltage to temperature in Celsius.
4. Based on the temperature range, the LED blinks at a specific rate.

---

## 🧪 Applications

1. Temperature alert system
2. Smart cooling fans
3. Educational microcontroller projects



