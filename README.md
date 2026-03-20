# 🚆 RailSafeBot – AI-Based Railway Track Crack Detection System

![Prototype image](https://github.com/user-attachments/assets/831acf3b-f971-45c8-a304-ec518dc6eba2)



## 📌 Overview

**RailSafeBot** is an AI-powered predictive maintenance robot designed to monitor railway tracks and detect cracks at an early stage. It integrates computer vision, sensor fusion, and edge AI to ensure railway safety and prevent major accidents.

The system uses:

* 📷 Camera module (ESP32-CAM)
* 📡 Ultrasonic sensor
* 📈 Vibration sensor

to detect structural anomalies in real-time.



## 🎯 Problem Statement

Railway inspection is traditionally:

* Manual
* Time-consuming
* Prone to human error

Delayed detection of cracks can lead to catastrophic failures.

👉 This project aims to:

* Automate railway inspection
* Detect cracks early
* Predict future failures
* Improve safety and efficiency



## 🧠 Key Features

* 🔍 AI-based crack detection using image classification
* 📡 Multi-sensor data fusion (Camera + Ultrasonic + Vibration)
* ⚡ Real-time anomaly detection
* 📊 Predictive maintenance analytics
* 🚨 Alert system (SMS / Alarm / Dashboard)
* 🌐 Edge computing using ESP32



## 🏗️ System Architecture

<img width="1011" height="644" alt="image" src="https://github.com/user-attachments/assets/0f21ae4e-2660-4bae-83b8-77377876855b" />


### 🔹 Modules Overview

#### 1. Data Ingestion

* ESP32-CAM captures railway track images
* Real-time transmission via Wi-Fi
* Optional SD card storage

#### 2. Image Processing

* Image classification using trained ML models
* Crack classification:

  * Normal
  * Minor Crack
  * Major Crack

#### 3. Multi-Sensor Data Fusion

* Combines:

  * Camera data
  * Ultrasonic readings
  * Vibration signals
* Improves detection accuracy

#### 4. Real-Time Processing

* Edge AI processing on ESP32
* Canny Edge Detection (~88.49% accuracy)
* Ultrasonic sensor measures crack depth

#### 5. Predictive Analytics

* Tracks crack progression
* Forecasts failures
* Suggests maintenance schedules

#### 6. Alert System

* Real-time alerts
* Emergency alarms
* SMS/Email notifications
* GPS-based location tracking


## 🛠️ Tech Stack

### 🔧 Software

* Arduino IDE / PlatformIO
* TensorFlow Lite / TensorFlow Lite Micro
* ESP-DL (Espressif DL Library)
* PyTorch / TensorFlow
* OpenCV

### ⚙️ Hardware

* ESP32-CAM (OV2640 Camera)
* Ultrasonic NDT Sensor
* Vibration Sensor
* GPS Module
* GSM Module
* FTDI Programmer
* 12V DC Motors + Motor Driver
* Power Supply (5V / 12V)


## 📂 Dataset

* Railway Track (Non-Crack) Images
* Railway Crack Dataset

Used for:

* Training classification models
* Testing crack detection accuracy



## 🚀 How It Works

1. Robot moves along railway track
2. Camera captures images continuously
3. Sensors collect vibration & depth data
4. AI model processes fused data
5. Crack is detected and classified
6. Alerts are triggered if required
7. Predictive model estimates future risks


## 📊 Results

* Accurate crack detection using AI + sensors
* Real-time monitoring capability
* Early-stage failure prediction
* Improved safety over manual inspection



## 📸 Sample Outputs
<img width="1216" height="645" alt="image" src="https://github.com/user-attachments/assets/43e7fda2-6904-440f-ac25-567179a80a15" />

<img width="2000" height="907" alt="image" src="https://github.com/user-attachments/assets/8d18cfcd-25ae-4ebd-b5cf-0b00aca9ec51" />


```
/images
  ├── crack_detected.jpg
  ├── normal_track.jpg
  └── dashboard.png
```



## 💻 Installation & Setup

### 1. Clone Repository

```bash
git clone https://github.com/your-username/railsafebot.git
cd railsafebot
```

### 2. Setup ESP32

* Install Arduino IDE
* Add ESP32 Board Support
* Upload CameraWebServer example

### 3. Install Dependencies

```bash
pip install opencv-python tensorflow torch numpy
```

### 4. Run Model

```bash
python detect_cracks.py
```
Youtube link:
https://youtu.be/4MqV2tyKS3M?si=F_sJnzSzP6MZdsBd 
---

## 🔮 Future Improvements

* 🚄 Integration with railway control systems
* ☁️ Cloud-based analytics dashboard
* 🤖 Autonomous navigation using AI
* 📡 5G-based real-time monitoring
* 🔍 Higher accuracy deep learning models



## 📜 License

This project is for academic and research purposes.


