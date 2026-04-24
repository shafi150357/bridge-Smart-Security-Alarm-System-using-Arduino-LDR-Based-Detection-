# bridge-Smart-Security-Alarm-System-using-Arduino-LDR-Based-Detection-
# 🔐 Smart Security Alarm System (Arduino)

## 📌 Project Overview
This project is a simple home security alarm system built using an Arduino.  
It detects environmental changes using a Light Dependent Resistor (LDR) and triggers an alarm when an intrusion is suspected.

The system is designed for low-cost, practical use in residential environments and can be simulated using Tinkercad.

---

## 🎯 Objectives
- Detect intrusion using light changes (LDR sensor)
- Trigger alarm (buzzer + red LED)
- Display system status using LEDs
- Implement automatic night mode

---

## ⚙️ Components Used
- Arduino (Uno / Mega 2560)
- Breadboard
- LDR (Photoresistor)
- Red LED (Alarm indicator)
- Green LED (System status)
- Buzzer
- Resistors (470Ω, 10kΩ)
- Jumper wires

---

## 🔌 System Behavior

### 🌙 Night Mode (Dark Environment)
- Activated when LDR value is high (e.g. > 600)
- Green LED blinks slowly
- System is actively monitoring

### ☀️ Normal Mode (Light)
- Green LED stays ON
- System is idle and monitoring

### 🚨 Intruder Detection
- Triggered when sudden bright light is detected (LDR < 300)
- Red LED flashes rapidly then stays ON
- Buzzer sounds continuously

### 🔁 Auto Reset
- System resets automatically when environment returns to dark

---

## 🧠 How It Works
The LDR reads light intensity and sends analog values (0–1023) to the Arduino.

- High values → Dark environment  
- Low values → Bright environment  

Threshold values are used to determine system states:
- `> 600` → Night mode  
- `< 300` → Intrusion detected  

---

## 💻 Arduino Code
> Upload the provided `.ino` file to your Arduino or run it in Tinkercad simulation.

---

## 🛠️ Simulation (Tinkercad)
You can simulate this project using Tinkercad:
- Adjust the LDR light level using the slider
- Observe LED and buzzer behavior

---

## 🚀 Future Improvements
- Add motion sensor (PIR) for better detection
- Add GSM module for SMS alerts
- Add mobile app monitoring
- Implement dynamic threshold calibration

---

## 📚 Learning Outcomes
- Understanding of analog sensors (LDR)
- Arduino programming and logic design
- Circuit design using breadboard
- Real-world application of embedded systems

---

## 👤 Author
**Ineza Shafi**  
Computer Systems and Architecture (CSA) Student  

---

## 📅 Date
April 2026
