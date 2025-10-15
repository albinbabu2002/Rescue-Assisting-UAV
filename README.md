# Rescue-Assisting-UAV
Rescue Assisting UAV is capable of being operated in the air at certain altitudes as well as through the surface of water. A UAV with this capability can help to locate and assess the situation of trapped people.  In challenging environments such as tunnels, and confined spaces, and carrying out dangerous missions in hazardous environments.

## 🚁 Project Overview

The Rescue Assisting UAV is engineered to locate and assess trapped individuals in disaster-stricken areas. Its robust carbon fiber frame and advanced sensor suite enable real-time data acquisition in inaccessible or hazardous zones. The UAV features both aerial and aquatic mobility, supporting operations in flooded tunnels and confined spaces.

## ✨ Features

- **Dual Environment Operation**: Flies in air and floats and move on water.
- **Advanced Sensing**: BME680 environmental sensor (temperature, pressure, humidity, VOC, CO2).
- **Live Video/Imaging**: ESP32-CAM module for video streaming and object detection.
- **Wireless Telemetry**: Sensor data integration with Blynk IoT dashboard.
- **Manual and AI-Based Operation**: Edge Impulse platform for object/person recognition.
- **High Durability**: Carbon fiber frame and protective casing.
- **Bright Spotlights**: LED race wire spotlights for low-light rescue missions.

## ⚙️ Software Stack

- **Flight Controller**: Betaflight/Bluejay ESC firmware
- **Embedded Code**: Arduino IDE (C++, ESP8266, libraries)
    - bsec.h (BME680 sensor)
    - ESP8266WiFi.h
    - Blynk.h
- **IoT Platform**: Blynk App (for sensor telemetry)
- **Edge Impulse**: For custom object detection and AI

## 🖼️ System Architecture

```plaintext
    [RC Tx] -- [Flight Controller] -- [ESCs] -- [BLDC Motors]
                    |                |          (Propulsion)
                    |                |
             [Sensors]           [ESP32-CAM]
                    |                |
                [ESP8266 D1 Mini]    |
                    |________________|
                     |   WiFi/Blynk (IoT)
```

## 🚀 Getting Started

### Prerequisites

- Basic soldering and drone assembly skills
- Arduino IDE installed for firmware upload
- Blynk App account and authentication token

## 📦 Applications

- Disaster rescue in tunnels, collapsed structures
- Environmental quality monitoring in hazardous areas
- Search and surveillance in flooded zones or confined spaces

## ⚠️ Limitations

- Flight and float time depend on battery capacity and load.
- Water-resistant, not fully submersible.
- Communication range limited by RF and Esp8266 WiFi modules instea of 8266-wifi use LORA module for long range.

## 🧑‍💻 Contributing

Contributions and improvements are welcome! Please open issues, submit pull requests, or propose features/enhancements.

**Project Authors:**  
- ALBIN BABU 
