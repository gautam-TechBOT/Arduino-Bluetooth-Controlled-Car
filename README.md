# Arduino Bluetooth Controlled Robot Car

This project is an Arduino-based robot car that is controlled using a mobile Bluetooth app.  
You can control forward, backward, left, right, diagonal movement, speed levels, lights, and horn wirelessly.

Commands are received over Bluetooth (Serial) and used to drive motors through a motor driver module.

---

## 🔧 Hardware Used

- Arduino UNO 
- HC-05  Bluetooth Module
- L298N  Motor Driver
- 4 DC Motors + Wheels
- Robot Chassis
- Front LED
- Back LED
- Parking LED
- Buzzer / Horn
- Jumper Wires
- 12v Battery Pack

---

## 📦 Required Libraries

No external libraries required.  
Uses only built-in Arduino functions (Serial, digitalWrite, analogWrite).

---

## 🔌 Pin Connections (As per Code)

### 🎯 Motor Driver Pins

| Driver Pin | Arduino Pin |
|-------------|-------------|
| IN1 | D3 |
| IN2 | D5 |
| IN3 | D6 |
| IN4 | D11 |

---

### 💡 Lights & Horn

| Device | Arduino Pin |
|----------|-------------|
| Front LED | D9 |
| Back LED | D8 |
| Horn / Buzzer | D7 |
| Parking LED | D4 |

---

### 📡 Bluetooth Module (HC-05 / HC-06)

| Bluetooth | Arduino |
|------------|----------|
| TXD | Arduino RX (D0) |
| RXD | Arduino TX (D1) *(use voltage divider recommended)* |
| VCC | 5V |
| GND | GND |

> ⚠️ Disconnect Bluetooth TX/RX while uploading code, then reconnect.

---

## 🎮 App Command Controls

| Command | Action |
|-----------|---------|
| F | Forward |
| B | Backward |
| L | Left |
| R | Right |
| G | Forward Left |
| I | Forward Right |
| H | Back Left |
| J | Back Right |
| S | Stop + Brake |

---

### 💡 Light Controls

| Command | Function |
|-----------|-----------|
| W / w | Front LED ON / OFF |
| U / u | Back LED ON / OFF |
| X / x | Parking LED ON / OFF |

---

### 🔊 Horn

| Command | Function |
|-----------|-----------|
| V / v | Horn ON / OFF |

---

### ⚡ Speed Levels

| Command | Speed PWM |
|-----------|------------|
| 0–9 | Increasing speed |
| q | Max speed (255) |

---

## ⚙️ Features

- Bluetooth app control
- Variable speed control
- Direction + diagonal driving
- Electronic braking support
- Front / back / parking lights
- Horn control
- PWM motor speed control

---

## ▶️ How to Run

1. Connect hardware as per pin table
2. Upload Arduino code
3. Connect Bluetooth module
4. Pair mobile with HC-05/HC-06
5. Open Bluetooth car control app
6. Send commands to drive car

---

## 📷 Circuit Diagram

Circuit diagram image will be added soon. Pin wiring table is provided above.

---

## 🎥 Working Video

https://www.youtube.com/shorts/UmliJ263hkA

---

## ⚠️ Notes

- Remove Bluetooth TX/RX while uploading code
- Use motor battery separate from Arduino if possible
- Keep GND common between Arduino and motor driver
- Use proper driver — do not connect motors directly to Arduino
- Ensure PWM pins are used for speed control

---

## 👨‍💻 Author

Gautam — Robotics & Embedded Projects
