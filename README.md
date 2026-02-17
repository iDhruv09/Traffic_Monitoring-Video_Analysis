# Traffic_Monitoring-Video_Analysis



# 🚀 AI Video Analytics Projects using YOLOv8

This repository contains **two real-world AI-powered video analytics systems**:

1. 🚦 Highway Traffic Congestion Monitoring
2. 🏬 Retail Store Video Analytics

Built using **Ultralytics YOLOv8**, OpenCV, and NumPy.

---

# 📂 Repository Structure

```
Traffic Monitoring & Video-Analytics/
│
├── traffic_monitoring/
│   ├── traffic_circle.mp4
│   ├── output_video.mp4
│   ├── Readme.md
│   └── traffic_monitoring.ipynb
│
├── video_analysis/
│   ├── retail_store.mp4
│   ├── output_video.mp4
│   ├── README.md
│   └── video_analysis.ipynb
│
└── README.md
```

---

# 🚦 1️⃣ Traffic Monitoring System

📁 Folder: `traffic_monitoring/`
📓 Notebook: `traffic_monitoring.ipynb`
🎥 Video: `traffic_circle.mp4`

---

## 📌 Overview

An AI-powered highway monitoring system that:

* 🚗 Detects vehicles (Car, Motorcycle, Bus, Truck)
* 🆔 Tracks vehicles with unique IDs
* 📏 Estimates speed (pixels/sec)
* 📊 Counts total vehicles
* 🐢 Detects slow-moving vehicles
* 🚦 Identifies traffic congestion
* 🎥 Generates annotated output video

---

## 🧠 Congestion Detection Logic

Congestion is triggered when:

```
vehicle_count > MIN_VEHICLES
AND
slow_vehicle_count > MIN_LOW_SPEED
```

Speed is calculated as:

```
Speed = Distance between frames × FPS
```

---

## 🌍 Real-World Applications

* Smart traffic management systems
* Urban planning & infrastructure optimization
* Automated CCTV traffic analysis
* Emergency response systems
* Smart city solutions

---

# 🏬 2️⃣ Retail Store Video Analytics

📁 Folder: `video_analysis/`
📓 Notebook: `video_analysis.ipynb`
🎥 Video: `retail_store.mp4`

---

## 📌 Overview

A retail intelligence system that performs:

* 👤 Customer detection
* 🆔 Multi-object tracking
* 🧭 Path visualization
* 🌡 Heatmap generation
* ⏱ Loitering detection
* 📊 Customer counting
* 🎥 Annotated output video

---

## 🧠 Retail Analytics Pipeline

```
Input CCTV Video
      ↓
YOLOv8 Detection
      ↓
Multi-Object Tracking
      ↓
Path Storage
      ↓
Heatmap Accumulation
      ↓
Loitering Analysis
      ↓
Output Video
```

---

## 🌍 Real-World Applications

* Store layout optimization
* Customer behavior analysis
* Theft & suspicious behavior detection
* Retail marketing insights
* Smart surveillance systems

---

# 🛠 Tech Stack

* Python
* YOLOv8
* OpenCV
* NumPy
* COCO Pre-trained Model

---

# 🚀 Installation

```bash
pip install ultralytics opencv-python numpy
```

---

# ▶️ How to Run

Open notebooks in:

* Jupyter Notebook
* Google Colab
* VS Code

Then run:

### Traffic Monitoring:

```
traffic_monitoring/traffic_monitoring.ipynb
```

### Retail Analytics:

```
video_analysis/video_analysis.ipynb
```

---

# 📊 Key Features Across Both Projects

✔ Real-time object detection
✔ Multi-object tracking
✔ Behavior analysis
✔ Speed estimation
✔ Heatmap visualization
✔ Congestion detection
✔ Annotated video generation
✔ Industry-relevant AI applications

---

# ⚠ Important Notes

* Speed is measured in pixels per second
* Real-world speed (km/h) requires camera calibration
* Fixed camera angle recommended
* Performance depends on video resolution & lighting

---

# 🔥 Future Enhancements

* Convert speed to km/h
* Export analytics to CSV
* Dashboard visualization
* Multi-camera integration
* Real-time CCTV support
* Cloud deployment

---

# 🎯 Target Domains

| Domain         | Application                   |
| -------------- | ----------------------------- |
| Smart Cities   | Traffic analytics             |
| Retail         | Customer behavior tracking    |
| Surveillance   | Automated monitoring          |
| Transportation | Flow analysis                 |
| AI Research    | Multi-object tracking systems |

---

# 🏁 Project Highlights

✔ Two complete AI video analytics systems
✔ Industry-level use cases
✔ Modular folder structure
✔ Portfolio & resume-ready
✔ Real-world computer vision applications

---

# 👨‍💻 Author

Developed as a Computer Vision & Deep Learning AI Video Analytics Project.

---

If you want, I can now provide:

* ⭐ 4 strong resume bullet points (combined project)
* 💼 Internship-level description
* 🏢 Enterprise-grade version
* 🎯 Short powerful GitHub profile description
* 🔥 LinkedIn project description

Tell me your goal (internship / job / production).
