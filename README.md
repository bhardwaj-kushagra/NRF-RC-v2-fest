# NRF24L01 Arduino RC Car 🚗💨

A wireless RC car controlled using **NRF24L01** transceivers and an **Arduino-based joystick controller**. The setup enables smooth and responsive remote driving with a **2.4GHz communication** link.

## 🎯 Features
- **Wireless control** using NRF24L01+ module 📡
- **Joystick-based movement** for intuitive handling 🎮
- **Dual Arduino setup** – one for controller, one for car 🛠️
- **L298N motor driver** for smooth motor control ⚙️
- **Reliable communication at 2.4GHz**

## 🛠️ Components
- **2× Arduino Uno**
- **2× NRF24L01+ (with antenna)**
- **L298N motor driver**
- **2-axis joystick module**
- **Power source (batteries)**
- **Chassis & motors**

## ⚡ Wiring Guide
### 🎮 **Joystick Controller (Transmitter)**
| Component | Arduino Pin |
|-----------|------------|
| CE        | D7         |
| CSN       | D8         |
| SCK       | D13        |
| MOSI      | D11        |
| MISO      | D12        |
| GND       | GND        |
| VCC       | 3.3V       |
| VRX       | A0         |
| VRY       | A1         |
| VCC (5V)  | 5V         |

### 🚗 **Car Module (Receiver)**
| Component | Arduino Pin |
|-----------|------------|
| CE        | D7         |
| CSN       | D8         |
| SCK       | D13        |
| MOSI      | D11        |
| MISO      | D12        |
| GND       | GND        |
| VCC       | 3.3V       |

#### 🏎️ **Motor Driver (L298N) Connections**
| L298N Pin | Arduino Pin |
|-----------|------------|
| IN1       | D5         |
| IN2       | D6         |
| IN3       | D7         |
| IN4       | D8         |
| GND       | GND        |

## 🔧 How It Works
1. The **joystick module** sends movement data via **NRF24L01** to the car.
2. The car receives signals and processes movement commands using the **L298N motor driver**.
3. You can control **forward, backward, left, and right movement** smoothly.

## 📌 Notes
- **Ensure NRF24L01 modules receive stable 3.3V power**.
- **L298N requires a separate power source for motors**.
- **Check wiring properly to avoid miscommunication**.

🚀 Get ready to **build & race** your own wireless RC car! Let me know if you have any questions. 😎
