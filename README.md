📡 Electrostatic Detector with Arduino

A simple and cost-effective Arduino-based system to detect electrostatic charges in real-time. This project uses a capacitive sensor (antenna + RC circuit) to sense static electricity and provides visual and audible alerts using an LED, buzzer, and LCD display. It is useful for ESD prevention, educational demonstrations, and electronics safety.

---

🔬 Introduction

Static electricity is an ever-present phenomenon that can damage sensitive electronic components, cause malfunctions, or even create safety hazards.
This project aims to provide a low-cost, real-time detection system using Arduino Uno and basic components. The detector alerts users about electrostatic charge buildup with a buzzer, LED, and LCD readout.


---


📦 Components Required

Component	Quantity	Description

Arduino Uno	1	Microcontroller board
Copper Wire (antenna)	1	Acts as electrostatic probe
Resistors	2–3	Used in RC detection circuit
LCD (I2C, 16x2)	1	Displays sensor values
LED	1	Visual alert
Buzzer	1	Audible alert
1N4007 Diode	1	Protection from spikes
Rechargeable Battery	1	Power supply
Jumper Wires	As needed	Connections
PCB/ Breadboard	1	Circuit assembly



---

⚡ Circuit Diagram

<img width="706" height="579" alt="Screenshot 2025-09-20 230845" src="https://github.com/user-attachments/assets/ccaf04d2-5b1f-4b11-b527-d9a8633e1252" />



---

⚙ How It Works

1. The copper wire antenna picks up nearby electrostatic fields.


2. The RC circuit converts capacitance changes into a voltage signal.


3. Arduino reads the analog signal from the sensor on pin A0.


4. If the value crosses the threshold, the LED and buzzer turn ON, and LCD displays "DETECTING".


5. Otherwise, the LED and buzzer remain OFF, and LCD shows "OFF".



💯Final Circuit 

![WhatsApp Image 2025-09-20 at 23 16 31_58b49862](https://github.com/user-attachments/assets/15c06b42-dd68-4b9a-96a3-9db3bcf6af0f)

![WhatsApp Image 2025-09-20 at 23 18 03_fdfc87d9](https://github.com/user-attachments/assets/43b081b2-ed35-47ac-9b12-2ef853632f9f)

---
✨ Features

⚡ Electrostatic field detection using a copper wire antenna

📟 LCD display for real-time monitoring

🔊 LED + buzzer alerts when charge is detected

🔧 Adjustable detection threshold via Arduino code

💡 Beginner-friendly and suitable for educational labs



---

🛠 Applications

Electrostatic Discharge (ESD) prevention in electronics labs

Educational tool for learning about electrostatics

Static electricity experiments

Dust and particle detection

Lightning prediction research

Quality control in manufacturing environments

DIY and hobbyist electronics projects



---
✅ Advantages & ❌ Limitations

Advantages

Non-contact detection

Real-time alerts

Low-cost, simple design

Beginner-friendly project


Limitations

Limited sensitivity range

Prone to interference from nearby electronics

Requires calibration for accuracy

Single-purpose (electrostatics only)



---

🚀 Future Improvements

Add OLED display for compact design

Implement wireless data logging (ESP8266/ESP32)

Display electrostatic field strength in volts/meter

Use AI/ML models to classify static sources

Improve sensitivity using better antennas
