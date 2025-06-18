# Ultrasonic Sensor with Arduino 🧠📏

This project demonstrates how to use an **ultrasonic sensor (HC-SR04)** with an **Arduino Uno** to measure distance and display it on an **I2C LCD** screen. It was developed and simulated using **TinkerCAD Circuits**.

## 📌 Project Overview

- **Platform:** Arduino Uno (Simulated on TinkerCAD)
- **Component:** HC-SR04 Ultrasonic Distance Sensor
- **Purpose:** Real-time distance measurement in centimeters (cm)

## 🔧 Components Used

| Component             | Quantity |
|-----------------------|----------|
| Arduino Uno R3        | 1        |
| HC-SR04 Ultrasonic Sensor | 1    |
| Jumper Wires          | As needed |

## ⚙️ Circuit Diagram
<a href="https://www.tinkercad.com/things/g3ARDLLDci6-ultrasonic-sensor-with-arduino"></a>

##🧠 <b>How It Works</b>

<ol type="i"><li>The trig pin sends out an ultrasonic pulse.</li>
<li>The echo pin receives the reflected wave.</li>
<li>The Arduino calculates the time taken and converts it to distance.</li>
<li>The result is shown on the I2C LCD in centimeters.</li></ol>

## ✅ Applications

<ul><li>Obstacle detection</li>
<li>Smart parking systems</li>
<li>Liquid level measurement</li>
<li>Robotics and automation</li>
