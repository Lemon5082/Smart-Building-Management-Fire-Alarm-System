# 🔥 Fire Detection System using IR Sensor and Arduino

## 📘 Project Overview

This project is a simple and effective **Fire Detection System** built using an **IR sensor**, **Arduino UNO**, **16x2 LCD display**, and a **buzzer**. It continuously monitors infrared radiation and alerts the user through visual (LCD) and audio (buzzer) signals when fire is detected.

---

## 🛠️ Features

- 🚨 Fire detection based on IR radiation levels.
- 📟 Real-time status display on a 16x2 LCD.
- 🔊 Audio alert via buzzer when fire is detected.
- ✅ Simple, low-cost, and beginner-friendly project.

---

## 🧰 Components Used

| Component         | Quantity | Description                                 |
|------------------|----------|---------------------------------------------|
| Arduino UNO       | 1        | Microcontroller                             |
| IR Flame Sensor   | 1        | Detects fire based on infrared radiation    |
| 16x2 LCD Display  | 1        | Displays system status                      |
| Buzzer            | 1        | Provides audio alert                        |
| Breadboard + Wires| As needed| For circuit connections                     |
| Resistor (optional)| 1        | For LCD contrast adjustment via potentiometer|

---

## 🔌 Circuit Connections

| Arduino Pin | Component         |
|-------------|-------------------|
| A0 (or change in code) | IR Sensor Output |
| 8, 9, 4, 5, 6, 7 | LCD RS, E, D4–D7 |
| 10          | Buzzer            |
| 5V, GND     | Power Supply      |

> ⚠️ **Note**: The IR sensor should be connected to an **analog pin**, e.g., `A0`, since `analogRead()` is used.

---

## 🧪 How It Works

1. The IR sensor detects infrared light from flames and outputs an analog signal.
2. If the IR value is **below a set threshold** (default `800`), the system identifies this as a potential fire.
3. In fire condition:
   - LCD shows `Fire detected`
   - Buzzer sounds
4. If no fire is detected:
   - LCD shows `Standby`
   - Buzzer remains silent

---
