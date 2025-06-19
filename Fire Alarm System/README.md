# 🔥 Fire Alarm System using Arduino

This project is a simple fire and gas detection system built using an Arduino UNO, temperature and gas sensors, LEDs, and a buzzer. It monitors environmental conditions and alerts users when dangerous levels of heat or gas are detected.

## 🚀 Features

- Detects high temperature using an TMP36 sensor
- Detects harmful gas levels using a gas sensor (e.g., MQ-2)
- Activates LEDs and buzzer for visual and audible alerts
- Displays real-time temperature and gas levels via Serial Monitor

## 🧰 Components Required

| Component                  | Quantity |
|---------------------------|----------|
| Arduino UNO               | 1        |
| TMP36 Temperature Sensor   | 1        |
| Gas Sensor (e.g., MQ-2)   | 1        |
| Buzzer                    | 1        |
| LEDs                      | 1        |
| Resistors (220Ω)          | 2        |
| Breadboard and Jumper Wires | As needed |

## 🔌 Circuit Connections

| Arduino Pin | Component               |
|-------------|-------------------------|
| A0          | Gas Sensor Output       |
| A1          | TMP36 Sensor Output      |
| D13         | Temperature Alert LED   |
| D7          | Buzzer (+ve)            |
| GND         | All sensor and buzzer GND |
| 5V          | All sensor and buzzer VCC |

**##📜 How It Works**

- Temperature is read from TMP36 (A1), converted to Celsius. The TMP36 is a temperature sensor that outputs an analog voltage proportional to the temperature in Celsius. It produces:<br>
10 millivolts (mV) per 1°C.<br> The analogRead() function reads the voltage from the LM35 as a value from 0 to 1023, representing 0V to 5V.<br>
So each unit ≈ 4.88 mV (5000 mV ÷ 1023 steps)<br>
- Gas level is read from the analog gas sensor (A0).<br>
- If:<br>
Temperature ≥ 80°C → LED (D13) ON<br>
Gas level ≥ 1000 → Buzzer (D7) ON<br>
- Serial Monitor prints real-time values every second.<br>
