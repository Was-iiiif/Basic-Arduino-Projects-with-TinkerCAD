# 🌡️ Digital Thermometer

This project reads the ambient temperature using an analog temperature sensor (like LM35) and displays it on a 16x2 LCD in Fahrenheit.

---

## 🧰 Components Used

| Component              | Quantity |
|------------------------|----------|
| Arduino UNO            | 1        |
| TMP36 Temperature Sensor| 1        |
| 16x2 LCD Display       | 1        |
| 10kΩ Potentiometer     | 1        |
| Breadboard + Wires     | As needed|

---

## 🔌 Pin Connection Chart

| LCD Pin | Arduino Pin |
|---------|-------------|
| RS      | 12          |
| EN      | 11          |
| D4      | 10          |
| D5      | 9           |
| D6      | 8           |
| D7      | 7           |
| VSS     | GND         |
| VDD     | 5V          |
| V0      | Potentiometer center |
| RW      | GND         |
| A (LED+) | 5V (with resistor) |
| K (LED-) | GND        |

| LM35 Pin | Arduino Pin |
|----------|-------------|
| VCC      | 5V          |
| GND      | GND         |
| OUT      | A0          |

---

## 🧠 Features

- Live temperature display in **Fahrenheit**.
- User-friendly 16x2 LCD output.
- Modular and easy-to-modify code.

---

## 🔄 Conversions Used

- **Analog to Voltage**:  
  `voltage = analogRead(A0) / 1023.0 * 5000.0;`
  
- **Voltage to Celsius (LM35DZ)**:  
  `celsius = (voltage - 500) / 10.0;`
  
- **Celsius to Fahrenheit**:  
  `fahrenheit = (celsius * 9.0 / 5.0) + 32;`

---

## 🚀 How to Run

1. Connect all components as per the pin chart.
2. Upload the code to your Arduino using the Arduino IDE.
3. Power the Arduino and observe the temperature reading on the LCD.

---



