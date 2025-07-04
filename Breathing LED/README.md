# 🌬️ Breathing LED 

This Arduino project simulates the natural rhythm of human breathing by gradually increasing and decreasing the brightness of an LED — mimicking the "inhale" and "exhale" pattern. It's a calming light effect suitable for meditation aids, night lights, or aesthetic installations.

---

## 🔧 Components Used

| Component            | Quantity |
|----------------------|----------|
| Arduino Uno/Nano     | 1        |
| LED                  | 1        |
| 220Ω Resistor        | 1        |
| Breadboard & Wires   | As needed |
| USB Cable            | 1        |

---

## 🔌 Circuit Diagram

- Connect the **long leg (anode)** of the LED to **digital pin 9** through a **220Ω resistor**.
- Connect the **short leg (cathode)** of the LED to **GND**.


---

## 🧠 Breathing Pattern Logic

| Phase     | Duration (ms) | Description                     |
|-----------|----------------|---------------------------------|
| Inhale    | 2000           | LED gradually gets brighter     |
| Hold      | 500            | LED stays at max brightness     |
| Exhale    | 3000           | LED gradually dims              |
| Pause     | 500            | LED remains off (optional)      |

Total breathing cycle ≈ **6 seconds**, mimicking calm human breathing (~10 BPM).

---

## 📦 Applications
- Meditation & mindfulness lighting
- DIY sleep aid lamp
- Calming ambient room lighting
- Visual metronome for breathwork
