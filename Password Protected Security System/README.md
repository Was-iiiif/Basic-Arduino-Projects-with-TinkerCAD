# 🔐 Password Protected Security System (Arduino)

This is a beginner-friendly security system built with **Arduino UNO**, **4x4 Keypad**, **LEDs**, and a **Piezo Buzzer**. It allows you to enter a password using the keypad and get feedback through lights and sound.

## 🚀 Features

- Alphanumeric password entry via keypad
- Access granted and denied indicators (LEDs and buzzer)
- Reset/clear input with `*` key
- Password submission with `#` key
- Serial Monitor support for debugging

## 🔧 Components Used

| Component       | Quantity | Description                      |
|----------------|----------|----------------------------------|
| Arduino UNO     | 1        | Microcontroller board            |
| 4x4 Keypad      | 1        | Matrix-style input device        |
| Piezo Buzzer    | 1        | Audio output                     |
| Red LED (D1)    | 1        | Access denied indicator          |
| Green LED (D2)  | 1        | Access granted indicator         |
| 1kΩ Resistor    | 2        | For current limiting on LEDs     |
| Breadboard      | 1        | For circuit assembly             |
| Jumper Wires    | -        | For making connections           |

## 🧠 How It Works
Step	Action
	
	
Match	Green LED blinks, buzzer beeps once
Mismatch	Red LED lights, buzzer beeps thrice
Press * anytime	Clears input buffer

| Step      | Action                      |
|----------------|----------------------------------|
| User enters keys     | Keys stored in a buffer            |
| Presses #      | Compares input with stored password        |
| Match    | Green LED blinks, buzzer beeps once                     |
| Mismatch    | Red LED lights, buzzer beeps thrice          |
| Presses * anytime  | Clears input buffer         |

## 📦 Applications

This project can be used in a variety of entry-level or prototype security contexts:

- 🔐 **Electronic Door Locks** — Replacing physical keys with a keypad entry  
- 🧰 **Locker Systems** — Password-protected toolboxes, cabinets, or lockers    
- 📦 **Access Control** — Basic access to devices, drawers, or compartments  
- 🛠️ **DIY Automation** — Integrate into smart home or office automation systems  
