# 🩺 Smart Medicine Reminder System

## 📌 Project Overview
The **Smart Medicine Reminder System** is an end-to-end IoT-based healthcare solution designed to help patients take their medicines on time and in the correct dosage. The system reduces missed doses, wrong medication intake, and caregiver burden by combining a web application, backend server, and a smart IoT device.

This project is developed as a team-based system with clear separation between frontend, backend, and device-level development.

---

## 🎯 Objectives
- Improve medication adherence
- Reduce missed or incorrect doses
- Provide automated reminders and alerts
- Enable remote monitoring by caregivers and family members
- Integrate IoT hardware with a web-based system

---

## 🏗️ High-Level System Architecture
Patient / Caregiver
│
▼
Web Application (Frontend)
│
▼
Backend Server (APIs, Database, Notifications)
│
▼
Smart Device (ESP32-based Pillbox)

---

## 📁 Project Folder Structure

SMARTMEDCODERS/
│
├── frontend/                         # React + Vite Web App
│   ├── public/
│   │   └── index.html
│   │
│   ├── src/
│   │   ├── assets/                   # Images, icons
│   │   ├── components/               # Reusable UI components
│   │   │   ├── Navbar.jsx
│   │   │   └── ReminderCard.jsx
│   │   │
│   │   ├── pages/                    # App pages/screens
│   │   │   ├── Login.jsx
│   │   │   ├── Dashboard.jsx
│   │   │   └── Schedule.jsx
│   │   │
│   │   ├── services/                 # API calls
│   │   │   └── api.js
│   │   │
│   │   ├── App.jsx                   # Root component
│   │   ├── main.jsx                  # Entry point
│   │   └── index.css
│   │
│   ├── .gitignore
│   ├── eslint.config.js
│   ├── vite.config.js
│   ├── package.json
│   ├── package-lock.json
│   └── README.md
│
├── backend/                          # Node.js + Express API
│   ├── src/
│   │   ├── routes/                   # API routes
│   │   │   └── reminderRoutes.js
│   │   │
│   │   ├── controllers/              # Business logic
│   │   │   └── reminderController.js
│   │   │
│   │   ├── models/                   # Database models
│   │   │   └── Reminder.js
│   │   │
│   │   ├── config/                   # DB, MQTT, Firebase configs
│   │   │   ├── db.js
│   │   │   └── mqtt.js
│   │   │
│   │   ├── services/                 # SMS, notifications, MQTT logic
│   │   │   └── notificationService.js
│   │   │
│   │   └── app.js                    # Express app
│   │
│   ├── server.js                     # Server entry point
│   ├── .env                          # Environment variables
│   ├── package.json
│   ├── package-lock.json
│   └── README.md
│
├── device/                           # ESP32 / IoT code
│   ├── esp32_main.ino                # Main ESP32 logic
│   ├── mqtt_config.h                 # MQTT broker config
│   ├── camera_module.ino             # Camera handling
│   └── README.md
│
├── docs/                             # Documentation
│   ├── architecture.png
│   ├── api_docs.md
│   ├── flowcharts/
│   │   ├── system_flow.png
│   │   └── device_flow.png
│
├── .gitignore
└── README.md                         # Main project overview


---

## 📂 Folder Description

### 🔹 frontend/
Contains the **web application** used by patients, caregivers, and doctors.

Responsibilities:
- User authentication
- Medicine schedule management
- Alerts and notifications
- Dashboard and reports

Tech Stack:
- Vite
- React
- HTML, CSS, JavaScript

🔹 backend/

Contains the server-side logic.


Responsibilities:

REST API development

Database management

Notification handling (SMS / app alerts)

Communication with IoT device


Planned Tech Stack:

Node.js

Express.js

Database (Firebase / MongoDB)

MQTT / HTTP APIs


🔹 device/

Contains embedded firmware for the smart pillbox.


Responsibilities:

ESP32 firmware

Alarm and reminder control

Sensor / camera integration

Communication with backend server



Hardware (planned):

ESP32

Camera module

Buzzer / LEDs

Sensors



🔹 docs/

Contains all project documentation, including:

Architecture diagrams

Flowcharts

API documentation

Design references

🔮 Future Enhancements

Mobile application support

AI-based pill recognition

Voice-based reminders

Advanced analytics and reporting
