# 🧪 Capacitance Measurement Using Arduino

This project allows you to **measure the capacitance** of an unknown capacitor using an Arduino UNO by timing how long it takes to charge through a known resistor.

---

## 🔧 Components Used

| Component           | Quantity | Notes                           |
|--------------------|----------|---------------------------------|
| Arduino UNO        | 1        | Microprocessor                               |
| Breadboard         | 1        | Establish connection                                |
| Resistor           | 2        | 10kΩ used for charge timing     |
| Capacitor          | 1        | Unknown capacitor to be measured |
| Jumper Wires       | Several  | For connections                 |

---

## ⚙️ Circuit Connections

| Arduino Pin | Connected To           |
|-------------|------------------------|
| A0          | Between resistor and capacitor |
| D8          | Resistor (Charge Pin)  |
| D9          | Capacitor (Discharge Pin) |
| GND         | Breadboard Ground      |
| 5V          | Positive rail (Resistor end) |

---

## 🧠 How It Works

- The capacitor is charged through a 10kΩ resistor by setting D8 HIGH.
- Arduino monitors voltage at A0 until it reaches about 63% of 5V (≈3.15V or analogRead ≈ 610).
- The time taken to reach this threshold is used to calculate the capacitance based on the RC charging formula:
  \[
  C = t/R
  \]

- After measurement, the capacitor is discharged by setting D9 LOW.

---

