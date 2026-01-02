# 🖥️ Smart Medicine Reminder System – Backend

## 📌 Overview
This folder contains the **backend server** for the **Smart Medicine Reminder System**.  
The backend acts as the **central controller** of the system, handling data processing, business logic, notifications, and communication between the web application and the ESP32 device.

It exposes APIs used by the frontend and manages real-time communication with the IoT device.

---

## 🎯 Backend Responsibilities
- Provide REST APIs for the frontend
- Manage medicine schedules and user data
- Handle authentication and authorization (planned)
- Communicate with the ESP32 device
- Trigger alerts and notifications
- Store and retrieve data from the database

---

## 🛠️ Tech Stack
- **Node.js**
- **Express.js**
- **JavaScript**
- **dotenv** – Environment variable management
- **CORS** – Cross-Origin Resource Sharing

(Additional libraries such as database drivers and MQTT will be integrated later.)

---

## 📁 Backend Folder Structure

backend/
│
├── src/
│ ├── routes/ # API route definitions
│ ├── controllers/ # Request handling & business logic
│ ├── models/ # Database models
│ ├── config/ # Database, MQTT, and app configurations
│ ├── services/ # Notification & communication logic
│ └── app.js # Express app configuration
│
├── server.js # Server entry point
├── .env # Environment variables (not committed)
├── package.json
├── package-lock.json
└── README.md # Backend documentation

---

## 🧠 File Description

### 🔹 `server.js`
- Entry point of the backend server
- Starts the Express application
- Listens on the configured port

---

### 🔹 `src/app.js`
- Configures Express middleware
- Registers routes
- Handles JSON parsing and CORS

---

### 🔹 `src/routes/`
- Defines REST API endpoints
- Maps URLs to controllers

Example:
PORT=5000
DB_URI=your_database_connection_string
MQTT_BROKER_URL=your_mqtt_broker_url

🔌 Communication Flow

Frontend sends API requests to backend

Backend processes logic and database operations

Backend sends commands or data to ESP32 device

ESP32 responds with status updates



🔀 Git Guidelines

Do not commit .env files

Use feature branches for development

Write clear commit messages

Avoid pushing directly to main




🔮 Future Enhancements

Authentication and role-based access

Database integration

MQTT-based real-time communication

Logging and monitoring

Security hardening