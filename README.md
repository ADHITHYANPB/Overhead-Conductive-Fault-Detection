# Overhead-Conductive-Fault-Detection
# ESP32-CAM Analog-Triggered Camera

ESP32-CAM-based project that reads an analog sensor value, monitors it in real-time via a web interface, and automatically captures a photo when the value reaches a defined threshold (e.g., 3000). The captured image is displayed on the web page along with the current sensor reading. Ideal for IoT monitoring, smart detection systems, and sensor-triggered photography applications.

## Features
- Real-time analog sensor monitoring over WiFi.
- Automatic photo capture when sensor threshold is reached.
- Web interface displaying both sensor readings and captured images.
- Lightweight and easy-to-deploy ESP32-CAM project.

## Hardware Required
- ESP32-CAM (AI-Thinker module)
- Analog sensor (e.g., potentiometer, ACS sensor, etc.)
- WiFi network

## Software Required
- Arduino IDE with ESP32 board support
- ESP32-CAM libraries:
  - `esp_camera.h`
  - `WiFi.h`
  - `WebServer.h`

## Usage
1. Connect your analog sensor to an ADC pin of the ESP32-CAM (default in code: GPIO 34).
2. Update your WiFi credentials in the code:
   ```cpp
   const char* ssid = "YOUR_SSID";
   const char* password = "YOUR_PASSWORD";

