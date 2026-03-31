# IoT-Based-Tunnel-Inspection-Rover-using-esp32

overview : 

This project implements an IoT-based tunnel inspection rover designed to monitor hazardous environments where human inspection is difficult or dangerous. The rover is controlled through a Blynk IoT mobile application and provides live environmental monitoring and video streaming.

The system uses two microcontrollers:

ESP32 – main rover controller (sensors, motors, IoT communication)
ESP32-CAM – live video streaming
The rover continuously monitors gas concentration, temperature, humidity, and obstacles, while transmitting the data to the Blynk cloud platform.

Features : 

Remote rover control through Blynk mobile app
Live camera streaming using ESP32-CAM
Gas detection using MQ sensors
Temperature and humidity monitoring
Obstacle detection using ultrasonic sensor
Motor speed control
Real-time alerts for dangerous gas levels
Hardware Components
ESP32 Development Board
ESP32-CAM Module
L298N Motor Driver
MQ2 Gas Sensor
MQ135 Gas Sensor
DHT11 Temperature and Humidity Sensor
HC-SR04 Ultrasonic Sensor
DC Motors
Robot Chassis
Battery Pack
Software & Technologies
Arduino IDE
ESP32 WiFi Library
Blynk IoT Platform
ESP32 Camera Library
Serial Communication (UART)
System Architecture
The rover system is divided into two main modules:

1. Rover Controller (ESP32)
Handles:

Motor control
Sensor data acquisition
Blynk communication
Obstacle detection
Gas monitoring

2. Camera Controller (ESP32-CAM)
Handles:

Camera initialization
Video streaming server
Sending camera stream link to the main ESP32
