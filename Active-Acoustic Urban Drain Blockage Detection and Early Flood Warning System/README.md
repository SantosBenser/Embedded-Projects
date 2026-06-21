# Active Acoustic Urban Drain Blockage Detection and Early Flood Warning System

## 📌 Title

Active Acoustic Urban Drain Blockage Detection and Early Flood Warning System Using ESP32

An intelligent IoT-based drainage monitoring system designed to detect drain blockages and predict flooding conditions before they become critical. The system combines ultrasonic sensing, flow monitoring, pressure analysis, acoustic inspection techniques, sensor fusion, and machine learning-based decision making to provide real-time alerts and early flood warnings through ESP32 connectivity.

---

## 🛠 Technologies

### Hardware
- ESP32 Development Board
- Ultrasonic Sensor
- Water Flow Sensor
- Pressure Sensor
- Buzzer
- LEDs
- Power Supply Module
- Breadboard
- Jumper Wires

### Software
- Arduino IDE
- Embedded C/C++
- Python
- MQTT Protocol
- Wi-Fi Communication

### Concepts
- Embedded Systems
- Internet of Things (IoT)
- Smart Drainage Monitoring
- Flood Prediction
- Sensor Fusion
- Machine Learning
- Predictive Maintenance
- Urban Infrastructure Monitoring
- Real-Time Alert Systems

---

## ✨ Features

- Real-time drain blockage detection
- Early flood warning system
- Water depth monitoring
- Flow rate analysis
- Pressure-based blockage identification
- Multi-sensor data fusion
- ESP32 Wi-Fi connectivity
- Mobile notifications
- Local LED and buzzer alerts
- Cloud integration using MQTT
- Machine Learning assisted verification
- Continuous monitoring system
- Historical event logging
- Smart urban drainage management

---

## ⌨️ System Controls

| Control | Function |
|----------|----------|
| Power ON | Activates monitoring system |
| ESP32 Reset | Restarts system |
| Wi-Fi Connection | Connects to monitoring network |
| Ultrasonic Sensor | Measures water depth |
| Flow Sensor | Measures water flow rate |
| Pressure Sensor | Detects pressure buildup |
| LED Indicators | Visual alert system |
| Buzzer | Audible warning system |
| MQTT Dashboard | Remote monitoring |
| Mobile Notification | Alert delivery |

---

## ⚙️ The Process

### 1. Sensor Data Acquisition

The system continuously collects:

- Water depth data
- Flow rate measurements
- Pipe pressure values

from multiple sensors installed in the drainage network.

---

### 2. Threshold Evaluation

The ESP32 analyzes incoming sensor data against predefined thresholds.

#### Pressure Threshold

When:

```text
Pressure > Threshold
```

the system suspects a blockage condition.

#### Flow Threshold

When:

```text
Flow Rate < Threshold
```

the system suspects restricted water movement.

Pressure buildup and reduced flow are strong indicators of drain obstruction. 

---

### 3. Sensor Fusion Analysis

The system combines:

- Water depth
- Flow rate
- Pressure

to improve reliability and reduce false alarms.

If multiple sensors indicate abnormal conditions, the likelihood of blockage increases.

---

### 4. Flood Detection

The ultrasonic sensor continuously monitors water depth.

If water depth exceeds the flood threshold:

```text
State = Critical Flood
```

Immediate action is triggered.

---

### 5. Blockage Classification

The decision engine evaluates:

#### Blockage Confirmed

```text
Flow ↓ AND Pressure ↑
```

#### Warning

```text
Flow ↓ OR Pressure ↑
```

#### Normal

```text
No abnormal sensor conditions
```

The system automatically classifies the drainage condition accordingly.

---

### 6. Machine Learning Verification

A Random Forest-based machine learning model verifies the rule-based classification using historical drainage behavior and real-time sensor data. This improves accuracy and minimizes false positives.

---

### 7. Alert Generation

Based on severity levels:

#### Critical Alert
- High flood risk
- Confirmed blockage
- Immediate maintenance required

#### Warning Alert
- Potential blockage
- Increased monitoring required

#### Normal
- Safe operation

The system automatically selects the appropriate response level.

---

### 8. Notification System

The ESP32 sends notifications through:

- Wi-Fi
- Mobile alerts
- MQTT cloud services

Alert messages contain:

- Alert severity
- Sensor readings
- Location information
- Timestamp

for rapid response.

---

### 9. Local Warning System

When abnormal conditions are detected:

- LEDs illuminate
- Buzzer activates
- Visual and audible alerts are generated

for immediate on-site awareness.

---

## 📚 What I Learned

- ESP32 programming
- IoT system development
- Sensor interfacing
- Real-time monitoring systems
- Urban drainage management
- Flood prediction concepts
- Multi-sensor fusion
- MQTT communication
- Wi-Fi-based notifications
- Machine learning integration
- Embedded system design
- Data analysis and classification
- Smart city infrastructure technologies

---

## 📈 Overall Growth

This project provided practical experience in designing a real-world smart infrastructure monitoring system. I gained hands-on exposure to embedded systems, IoT communication, sensor fusion, machine learning-assisted decision making, and predictive maintenance strategies.

The project strengthened my understanding of how modern technology can improve public safety, reduce flood risks, and support smart city development through continuous monitoring and intelligent alert systems.

---

## 🚀 How Can It Be Improved

- AI-based blockage prediction
- Computer vision for drain inspection
- Solar-powered operation
- LoRaWAN communication for long-range monitoring
- Cloud dashboard analytics
- Mobile application integration
- GIS mapping support
- Smart city platform integration
- Digital twin implementation
- Automated maintenance scheduling
- Multi-location monitoring network
- Real-time flood forecasting

---

## ▶️ Running the Project

### Hardware Requirements

- ESP32
- Ultrasonic Sensor
- Flow Sensor
- Pressure Sensor
- Buzzer
- LEDs
- Power Supply

### Software Requirements

- Arduino IDE
- ESP32 Board Package
- Required Libraries
- MQTT Broker (Optional)

### Steps

1. Assemble all hardware components.
2. Connect sensors to ESP32.
3. Install ESP32 board support in Arduino IDE.
4. Upload the source code.
5. Configure Wi-Fi credentials.
6. Configure MQTT settings (optional).
7. Power the system.
8. Monitor sensor readings.
9. Observe alerts and notifications.

---

## 📊 System States

| State | Description |
|---------|-------------|
| Normal | Drain operating correctly |
| Warning | Possible blockage developing |
| Blockage Confirmed | Obstruction detected |
| Critical Flood | Immediate flood risk |

---

## 🎯 Applications

- Smart Cities
- Urban Drainage Systems
- Flood Prevention Systems
- Municipal Infrastructure Monitoring
- Industrial Drainage Monitoring
- Smart Water Management
- Disaster Prevention Systems
- IoT Infrastructure Solutions

---

## 👨‍💻 Author

**Santos**

---

*"Transforming urban drainage systems into intelligent, self-monitoring infrastructure through IoT and machine learning."*
