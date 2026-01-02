# 📟 Smart Medicine Reminder System – Device (ESP32)

## 📌 Overview
This folder contains the **embedded firmware and hardware-related code** for the **Smart Medicine Reminder System**.  
The device functions as a **smart pillbox** that reminds patients to take medicines on time and communicates with the backend server for monitoring and verification.

The device is built using an **ESP32 microcontroller**, enabling Wi-Fi connectivity, alert mechanisms, and real-time communication with the backend system.

---

## 🎯 Device Objectives
- Trigger medicine reminders at scheduled times
- Provide visual and audible alerts to the patient
- Verify medicine intake using a camera module
- Communicate device status and events to the backend server
- Support remote monitoring by caregivers and family members

---

## 🧰 Hardware Components (Planned)
- **ESP32 Development Board**
- **Camera Module (ESP32-CAM)**
- **Buzzer / Speaker**
- **LED Indicators**
- **Power Supply / Battery**

---

## 📁 Device Folder Structure
device/
│
├── esp32_main.ino # Main ESP32 firmware logic
├── mqtt_config.h # Wi-Fi and MQTT configuration
├── camera_module.ino # Camera initialization and capture logic
└── README.md # Device documentation


---

## 🧠 File Description

### 🔹 `esp32_main.ino`
- Entry point for the ESP32 firmware
- Handles:
  - Wi-Fi connection
  - Receiving medicine schedules
  - Triggering alarms and alerts
  - Communicating with backend server
  - Coordinating camera-based verification

---

### 🔹 `mqtt_config.h`
- Stores configuration details such as:
  - Wi-Fi credentials
  - MQTT broker address and port
  - Publish/subscribe topics
- Enables communication between the ESP32 device and backend server

📌 **Note:**  
Sensitive credentials should never be committed to GitHub.

---

### 🔹 `camera_module.ino`
- Responsible for:
  - Camera initialization
  - Capturing images during medicine intake
  - Sending images or verification data to backend
- Used to confirm whether the correct medicine is taken

---

## 🔌 Communication Flow
- Device connects to Wi-Fi
- Establishes communication with backend (via MQTT or HTTP)
- Receives medicine schedule data
- Triggers reminders at scheduled times
- Sends:
  - Medicine intake confirmation
  - Device status updates
  - Alert acknowledgements

---

## ⚙️ Development Setup

### Requirements
- Arduino IDE or PlatformIO
- ESP32 board support package installed
- Required libraries:
  - WiFi
  - PubSubClient (for MQTT)
  - ESP32 Camera libraries

---

## 🚀 Uploading Code to ESP32
1. Connect ESP32 to the system using USB
2. Open the `.ino` files in Arduino IDE
3. Select the correct ESP32 board and COM port
4. Upload the firmware
5. Monitor logs using Serial Monitor

---

## 🔒 Security Considerations
- Protect Wi-Fi credentials
- Use secure communication channels where possible
- Validate backend messages before execution

---


## 🔮 Future Enhancements
- Secure OTA firmware updates
- Power optimization for battery operation
- Advanced image verification
- Voice-based alerts

---

## 📜 License
This device firmware is developed for **educational and academic purposes**.

---

## 🙌 Contributors
SmartMedCoders – Embedded Systems Team
