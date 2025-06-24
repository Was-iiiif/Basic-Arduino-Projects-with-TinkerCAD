# NeoPixel Strip (4 LEDs) using Arduino

This is a beginner-friendly project that demonstrates how to control a 4-LED NeoPixel (WS2812) strip using an Arduino board. The NeoPixel LEDs are RGB addressable LEDs that can display millions of colors with precise control using a single digital pin. This project includes smooth rainbow animation to visualize color transitions and can be a great starting point for learning about addressable LEDs and animation effects.

---

## 🔧 Key Features

- Control of a NeoPixel strip (4 LEDs)
- Rainbow animation effect
- Adjustable brightness
- Uses Adafruit NeoPixel library
- Simple and expandable for larger strips

---

## 🧪 Components Used

| Serial No. | Component                          | Specification / Type            | Quantity |
|------------|------------------------------------|----------------------------------|----------|
| 1          | Arduino Board                      | UNO / Nano / Compatible          | 1        |
| 2          | NeoPixel LED Strip                 | WS2812 / WS2812B (4 LEDs)        | 1        |
| 3          | Resistor                           | 330Ω (for data line protection)  | 1        |
| 4          | Capacitor                          | 1000µF, 6.3V or higher           | 1        |
| 5          | Jumper Wires                       | Male-to-Male / Female-to-Male    | As needed |
| 6          | Breadboard                         | Standard mini or full-size       | 1        |
| 7          | External 5V Power Supply (optional)| 5V regulated adapter or battery  | 1        |
| 8          | USB Cable                          | For programming Arduino          | 1        |

---

## ⚙️ Circuit Connections

| NeoPixel Pin | Arduino Pin        |
|--------------|--------------------|
| DIN          | D6 (or other defined pin) |
| +5V          | 5V                 |
| GND          | GND                |

- Use a **330Ω resistor** between D6 and DIN
- Place a **1000µF capacitor** between 5V and GND (at LED power input)

---

## 📁 Library Required

Install the **Adafruit NeoPixel** library:
- Open Arduino IDE
- Go to **Sketch > Include Library > Manage Libraries**
- Search for **Adafruit NeoPixel** and click **Install**

---

## 📌 Applications
- LED decoration and art
- Mood lighting or ambient effects
- Learning embedded programming and timing
- Interactive Arduino-based light shows
