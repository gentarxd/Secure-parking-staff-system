# Secure-parking-staff-system
Collection of IoT and Automation systems built using ESP32, Arduino, n8n, Supabase, and PostgreSQL — including Smart Parking and Smart Attendance ; Payroll solutions with real-time monitoring and workflow automation.
🚗 Smart Safety Parking & Employee Management System

An integrated IoT-based smart parking and employee management system built using Arduino, ESP32, RFID technology, cloud databases, and real-time monitoring systems.

The project combines:

- Smart parking automation
- RFID vehicle access control
- Emergency safety systems
- Gas leak and earthquake detection
- Employee attendance tracking
- Web dashboard monitoring
- Payroll and attendance analytics
- Cloud database integration

---

📌 System Overview

This project is divided into two main subsystems:

1️⃣ Smart Safety Parking System

An Arduino-based intelligent parking system that controls vehicle access using RFID authentication and provides advanced emergency safety features.

2️⃣ Smart Employee Attendance System

An ESP32-based employee management and attendance system connected to a live web dashboard and cloud database.

---

🚘 Smart Parking System Features

✅ RFID Vehicle Authentication

- Uses MFRC522 RFID Reader
- Allows only authorized RFID cards
- Supports entry/exit detection

✅ Automatic Gate Control

- SG90 Servo Motor controls the main parking gate
- Automatically opens/closes after authentication

✅ Parking Slot Management

- Separate parking states for vehicles
- LED indicators for parking activity

✅ Parking Duration & Cost Calculation

- Calculates parking duration using "millis()"
- Calculates parking cost automatically

✅ Gas Leak Detection

- MQ-2 Gas Sensor continuously monitors gas levels
- Activates:
  - Buzzer alarm
  - Warning LED
  - Emergency exit system

✅ Earthquake / Vibration Detection

- SW-420 Vibration Sensor detects abnormal vibration
- Activates emergency procedures automatically

✅ Emergency Exit System

- MG995 Continuous Rotation Servo Motor
- Opens emergency exit during dangerous situations
- Automatically closes after alert completion

✅ Real-Time Serial Monitoring

Displays:

- Vehicle entry
- Exit duration
- Parking cost
- Gas alerts
- Earthquake alerts

---

👨‍💼 Employee Attendance System Features

✅ Employee Authentication

- 4x4 Keypad-based employee login system
- Individual secure employee codes

✅ Attendance Tracking

- Check-in / Check-out system
- Calculates attendance duration

✅ ESP32 Web Dashboard

Real-time dashboard includes:

- Live employee status
- Attendance records
- Payroll analysis
- Admin panel
- Dark/Light theme

✅ Payroll Management

Automatically calculates:

- Attendance days
- Working hours
- Late penalties
- Net salary

✅ Supabase Database Integration

Stores:

- Attendance logs
- Check-in/out records
- Durations
- Payroll data

✅ N8N Automation Integration

Sends attendance events to:

- CRM system(Google sheets) 
- Notification(Telegram)

✅ WiFi Connectivity

ESP32 hosts:

- Live web server
- Interactive dashboard

---

🛠 Hardware Components

Parking System

- Arduino UNO
- MFRC522 RFID Reader
- SG90 Servo Motor
- MG995 Continuous Rotation Servo
- MQ-2 Gas Sensor
- SW-420 Vibration Sensor
- Buzzer
- LEDs
- RFID Cards
- Breadboard & Jumper Wires

Employee System

- ESP32
- 4x4 Keypad
- WiFi Connection

---

💻 Software & Technologies

Embedded Systems

- Arduino IDE
- C/C++

Communication Protocols

- SPI Communication
- Serial Communication
- HTTP Requests

Cloud & Web

- Supabase
- N8N
- REST APIs
- Web Dashboard

Frontend

- HTML
- CSS
- JavaScript

---

🔌 Communication Architecture

RFID Communication

The RFID module communicates with Arduino using:

- SPI Protocol

Pins:

- MOSI
- MISO
- SCK
- SS

Arduino acts as:

- SPI Master

RFID Reader acts as:

- SPI Slave

---

🚨 Emergency Safety Logic

If:

- Gas leak is detected
  OR
- Earthquake/vibration is detected

The system automatically:

1. Activates buzzer alarm
2. Turns on warning LED
3. Opens emergency exit
4. Alerts users through serial monitoring

---

🌐 Web Dashboard Features

Dashboard Includes

- Live employee monitoring
- Attendance history
- Payroll reports
- Admin management system

Admin Capabilities

- Add employees
- Remove employees
- Monitor attendance
- Manage payroll system

---

📊 Payroll System

The payroll module automatically calculates:

- Total attendance days
- Total working hours
- Delay penalties
- Final salary

---

🔐 Security Features

- RFID-based access control
- Secure employee authentication
- Admin password protection
- Cloud-based attendance logging

---

🚀 Future Improvements

- Mobile Application Integration
- Camera-based Plate Recognition
- IoT Notifications
- Cloud Analytics Dashboard
- AI-based Parking Prediction
- Fire Suppression System

---

📷 Project Preview

Smart Parking System

- RFID access gate
- Emergency exit system
- Gas detection
- Earthquake alert system

Employee Management Dashboard

- Real-time attendance monitoring
- Payroll analytics
- Cloud synchronization

---

👨‍💻 Developed By

**Mahmoud Abdelnasser**
**Youssef Mohammed**

---
