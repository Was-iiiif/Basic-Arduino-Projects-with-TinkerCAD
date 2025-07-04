# 🚗 Smart Parking System

This project demonstrates an **automated smart parking system** using an Arduino Uno. It detects the presence of vehicles in parking slots and controls entry and exit gates using servo motors. The parking status is displayed on a 16x2 LCD screen in real-time.

---

## 📋 Features

- Detects vehicle presence in parking slots using IR sensors.
- Displays parking slot availability on an LCD display.
- Automatically controls entry and exit gates with servo motors.
- Simple, efficient, and cost-effective solution.
- Real-time status updates.

---

## 🛠️ Components Used

| Component                     | Quantity | Purpose                                      |
|-------------------------------|----------|----------------------------------------------|
| Arduino Uno                    | 1        | Microcontroller                              |
| IR Sensors                     | 4        | Detect vehicle presence                      |
| Servo Motors                   | 2        | Control entry and exit barriers              |
| 16x2 LCD Display (Parallel)    | 1        | Display parking slot status                  |
| Potentiometer                  | 1        | Adjust LCD contrast                          |
| Jumper Wires                   | -        | Electrical connections                       |
| Breadboard                     | 2        | Circuit assembly                             |
| Resistor (for LCD)             | 1        | LCD backlight resistor                       |

---

## ⚙️ Working Principle

### 1. Slot Monitoring
- **IR Sensors on Pin 9 and 10** detect car presence in Slot 1 and Slot 2.
- If a slot is occupied, the LCD shows:
  
  `Slot 1 = NA` or `Slot 2 = NA`  *(NA: Not Available)*

- If a slot is vacant, the LCD shows:
  
  `Slot 1 = A` or `Slot 2 = A` *(A: Available)*

### 2. Gate Control
- **IR_ENTRY (Pin 8):** Detects cars approaching the entry gate. The entry servo opens to allow entry.
- **IR_EXIT (Pin 11):** Detects cars at the exit gate. The exit servo opens to allow departure.
- Gates return to the closed position when no car is detected.

---

## 🔌 Circuit Connections

| Arduino Pin | Connected To           |
|-------------|------------------------|
| 9           | IR Sensor (Slot 1)     |
| 10          | IR Sensor (Slot 2)     |
| 8           | IR Sensor (Entry Gate) |
| 11          | IR Sensor (Exit Gate)  |
| 12          | Servo Motor 1 (Entry)  |
| 13          | Servo Motor 2 (Exit)   |
| 7, 6, 5, 4, 3, 2 | LCD Control & Data Pins |

---

## ▶️ Usage Instructions

1. Upload the Arduino code to the Arduino Uno.
2. Power the Arduino with USB or external 5V power supply.
3. The LCD will display a welcome message and initial slot status.
4. Place an object in front of the IR sensors to simulate a vehicle.
5. Watch the slot availability change on the LCD and the gates operate automatically.

---

## 🚀 Future Enhancements

- Replace IR sensors with ultrasonic sensors for more precise detection.
- Increase the number of monitored slots.
- Add network connectivity for remote monitoring (using ESP32 or Wi-Fi module).
- Integrate with a smartphone app or web dashboard.
- Include automatic billing or ticketing.

---

## 📄 License

This project is licensed under the MIT License.

---

