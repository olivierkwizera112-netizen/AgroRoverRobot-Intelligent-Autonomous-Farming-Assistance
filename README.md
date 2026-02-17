# AgroRover 🤖 – Intelligent Autonomous Farming Assistant

[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

---

## Project Vision
Agriculture is the backbone of Rwanda’s economy. However, many farmers still rely on **manual inspection** to monitor crop health, soil conditions, and irrigation needs. This leads to:

- Over-irrigation or under-irrigation
- Late disease detection
- Reduced crop yield
- Wasted resources

**AgroRover** is an autonomous robotic system designed to **monitor crop health, analyze soil conditions, and provide real-time intelligent recommendations** through an advanced web dashboard.  
We are combining **Robotics, AI, IoT, and full-stack web development** to modernize small and medium-scale farming.

---

## System Overview
AgroRover consists of **four major subsystems**:

1. **Autonomous Ground Rover (Hardware + Robotics)**
2. **Sensor & Data Acquisition System**
3. **AI Processing & Decision Engine**
4. **Advanced Web Monitoring Platform (React + Node + Express)**

---

### 1️⃣ Autonomous Robotic Rover

The rover is a **4-wheel smart robotic vehicle** capable of navigating between crop rows.

#### Movement System
- DC motors with motor driver (L298N or similar)
- Ultrasonic sensors for obstacle detection
- Line-following capability (optional)
- GPS module for open-field navigation (advanced version)

#### Intelligence
- ESP32 or Arduino for real-time control
- Raspberry Pi for AI image processing
- Autonomous navigation algorithm:
  - Obstacle avoidance
  - Row-based movement logic
  - Pre-programmed path execution

> The rover moves through farmland, stops at intervals, collects environmental data, and sends it to the cloud server.

---

### 2️⃣ Sensor & Data Collection System

The rover collects multiple environmental parameters:

**Environmental Sensors:**
- Soil Moisture Sensor
- DHT22 (Temperature & Humidity)
- Light Intensity Sensor
- pH Sensor (advanced)
- Water Level Sensor (irrigation monitoring)

**Camera Module:**
- Captures crop leaf images
- Used for disease detection
- Raspberry Pi Camera or ESP32-CAM

> All collected data is transmitted via WiFi or GSM to the backend server.

---

### 3️⃣ AI & Smart Decision Engine

#### AI Plant Disease Detection
- Machine learning model trained using plant disease dataset
- Image classification (Healthy vs Diseased)
- Basic CNN model using Python + TensorFlow

**Example Flow:**
1. Leaf image captured
2. AI detects early blight disease
3. System sends alert before disease spreads

#### Smart Irrigation Recommendation
Uses:
- Soil moisture levels
- Weather forecast API
- Historical crop data

The system:
- Predicts irrigation needs
- Suggests optimal watering time
- Prevents water waste

#### Yield Prediction Model (Advanced)
Uses:
- Seasonal data
- Temperature trends
- Soil conditions
- Past production data

> Regression-based prediction system estimates expected crop yield. Judges love this predictive intelligence!

---

### 4️⃣ Advanced Web Dashboard (Modern Tech Stack)

We are building a **professional agricultural monitoring platform** using:

- **Frontend:** React.js
- **Backend:** Node.js + Express.js
- **Database:** MongoDB or MySQL
- **Authentication:** JWT
- **Real-time updates:** Socket.io

#### Dashboard Features
- **Real-Time Monitoring**
  - Live soil moisture levels
  - Temperature & humidity
  - Rover battery level
  - GPS location map
- **Interactive Farm Map**
  - Visual map of field
  - Rover position tracking
  - Highlighted problem zones
- **AI Alerts Panel**
  - “Leaf disease detected in Zone 3”
  - “Low moisture in Sector A”
  - “Irrigation recommended”
- **Data Analytics & Graphs**
  - Historical moisture trends
  - Crop health statistics
  - Yield prediction charts
  - Water usage analytics
- **SMS & Notification System**
  - SMS alerts using Twilio API
  - Push notifications for mobile users
  - Email alert system

---

### Solar Charging System
To make the project sustainable:
- Solar panel mounted on rover
- Smart battery management system
- Power-efficient movement algorithm

> Ensures long operation hours, eco-friendly design, and suitability for rural areas.

---

### Security & Scalability
- Secure API endpoints
- Role-based access (Admin / Farmer / Researcher)
- Cloud hosting ready
- Expandable to multiple farms

---

### System Architecture
