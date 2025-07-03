# Flowing LED Lights with Arduino

This Arduino project demonstrates a simple flowing LED light effect using multiple LEDs connected to digital output pins. The LEDs turn on one after another in sequence and then turn off in reverse order, creating a wave-like flow of light.

## 🔧 Project Description

This project simulates a "flowing" or "chasing" light effect, often used in decorative lighting or to visualize sequence timing. It's a great beginner project to understand basic digital output control, `for` loops, and timing in Arduino programming.

## 🧰 Components Used

| Component              | Quantity | Description                      |
|------------------------|----------|----------------------------------|
| Arduino Uno/Nano       | 1        | Microcontroller board            |
| LED (Any color)        | 6        | Standard 5mm LEDs                |
| Resistor (220Ω)        | 6        | Current-limiting resistor        |
| Breadboard             | 1        | For circuit prototyping          |
| Jumper Wires           | As needed | For electrical connections       |

## 🔌 Circuit Diagram

Each LED is connected to a digital pin (from pin 2 to pin 7). A 220Ω resistor is connected in series with each LED to prevent overcurrent. The negative (shorter) leg of each LED is connected to the ground rail.


## 🧠 Learning Outcomes
- Use of pinMode() and digitalWrite()
- Loop control using for
- Simple LED wiring and circuit safety
- Timing control using delay()
