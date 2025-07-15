# SAFEDrive
## Smart Automated Fatigue and Elevation Detection Drive System
SAFEDrive, developed by Team Sentinels — Chirag Gulati, Harsh Bansal, Mukul Sunda, and Harshit Bhatia — was the winning project at InnoHacks 3.0 (2024), hosted by KIET, Ghaziabad. 

## Overview
SAFEDrive is an advanced driver safety system that uses a multi-modal approach to detect driver drowsiness and fatigue. By combining computer vision technology with heart rate variability (HRV) analysis, the system provides a reliable method for preventing accidents caused by driver fatigue.

## Key Features
- **Dual-Detection System**
  - Computer Vision-based facial analysis
  - Heart Rate Variability (HRV) monitoring through PPG sensors
- **Real-time Processing**
- **Alert System** with buzzers and vibration feedback
- **Embedded System** implementation on Raspberry Pi and Arduino

## Technical Architecture

### 1. Vision-based Detection
- **Eye State Monitoring**
  - Tracks eye aspect ratio (EAR)
  - Detects eye closure duration
  - Uses facial landmarks for precise measurements
- **Head Position Analysis**
  - Monitors head roll index
  - Tracks facial orientation

### 2. Physiological Monitoring
- **PPG Sensor Integration** (MAX30102)
  - Heart rate measurement
  - HRV analysis
  - Breathing rate monitoring
- **Feature Extraction**
  - BPM (Beats Per Minute)
  - IBI (Inter-Beat Interval)
  - Breathing rate patterns

### 3. Alert System
- Triggers alerts when:
  - Extended eye closure is detected
  - Abnormal head position is identified
  - Irregular heart rate patterns are observed
- Alert mechanisms:
  - Audible buzzers
  - Vibration feedback
  - Visual warnings on display

## Hardware Requirements
- Raspberry Pi (Main processing unit)
- Arduino (Sensor interface)
- Camera module
- MAX30102 PPG sensor
- Buzzer module
- Vibration motor

## Software Components
1. **Eye Detection Module**
   - TensorFlow-based eye state classification
   - Custom trained model for robust detection

2. **Facial Landmark Detection**
   - dlib-based facial feature extraction
   - Real-time landmark tracking

3. **HRV Analysis System**
   - PPG signal processing
   - Machine learning-based fatigue prediction
   - Real-time heart rate monitoring