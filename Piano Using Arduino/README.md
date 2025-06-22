# 🎹 Arduino Piano 

This project demonstrates how to create a simple piano using an Arduino board, a piezo buzzer, and push buttons. Each button corresponds to a musical note from the C major scale.

---


## 🔧 Components Used

| Component             | Quantity |
|-----------------------|----------|
| Arduino Uno/Nano      | 1        |
| Piezo Buzzer          | 1        |
| Push Buttons          | 8        |
| 10kΩ Resistors        | 8        |
| Breadboard & Jumper Wires | 1 set    |

---

## 🎼 Notes & Frequencies

| Note | Frequency (Hz) |
|------|----------------|
| C4   | 262            |
| D4   | 294            |
| E4   | 330            |
| F4   | 349            |
| G4   | 392            |
| A4   | 440            |
| B4   | 494            |
| C5   | 523            |

---

## 🧪 Working Principle

- Each button triggers a specific frequency corresponding to a musical note.

- The tone() function sends a PWM signal to the buzzer to generate that frequency.

- Delay ensures notes are audible without overlapping.

- noTone() stops the sound after the delay.

