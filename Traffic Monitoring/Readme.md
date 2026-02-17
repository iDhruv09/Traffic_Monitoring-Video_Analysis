# 🚦 Highway Congestion Monitoring System using YOLOv8

An AI-powered **traffic monitoring system** that detects vehicles, tracks them across frames, estimates their speed, counts total vehicles, identifies slow-moving vehicles, and detects highway congestion from a video file.

Built using **Ultralytics YOLOv8**, OpenCV, and NumPy.

---

## 📌 Project Overview

This system processes a highway traffic video and provides:

* 🚗 Vehicle Detection (Car, Motorcycle, Bus, Truck)
* 🆔 Multi-object Tracking (unique ID per vehicle)
* 📏 Speed Estimation (pixels per second)
* 📊 Vehicle Counting
* 🐢 Slow Vehicle Detection
* 🚦 Automatic Congestion Detection
* 🎥 Output annotated monitoring video

The system is optimized for Google Colab and local execution.

---

## 🧠 How It Works

1. Load YOLOv8 pre-trained model (`yolov8n.pt`)

2. Detect and track vehicles using built-in ByteTrack

3. Assign unique IDs to each vehicle

4. Calculate vehicle speed:

   ```
   Speed = Distance between frames × FPS
   ```

5. Count:

   * Total vehicles
   * Slow-moving vehicles

6. Detect congestion if:

   * Total vehicles > threshold
   * Slow vehicles > threshold

7. Save processed output video

---

## 🎯 Vehicle Classes Used (COCO Dataset)

| Class      | ID |
| ---------- | -- |
| Car        | 2  |
| Motorcycle | 3  |
| Bus        | 5  |
| Truck      | 7  |

---

## ⚙️ Congestion Detection Logic

Congestion is detected when:

```
vehicle_count > MIN_VEHICLES
AND
slow_vehicle_count > MIN_LOW_SPEED
```

You can adjust:

```python
LOW_SPEED_THRESHOLD
MIN_VEHICLES
MIN_LOW_SPEED
```

---

## 🛠️ Tech Stack

* Python
* YOLOv8
* OpenCV
* NumPy
* COCO Pre-trained Model

---

## 🚀 Installation

```bash
pip install ultralytics opencv-python numpy
```

---

## ▶️ Run the Project

Place your traffic video:

```
traffic.mp4
```

Then run the script:

```bash
python traffic_monitor.py
```

Output:

```
output_video.mp4
```

---

## 📂 Input & Output

### Input:

* Highway traffic video file (`.mp4`)

### Output:

* Annotated video with:

  * Bounding boxes
  * Vehicle IDs
  * Speed values
  * Total vehicle count
  * Slow vehicle count
  * Congestion alert

---

# 🌍 Real-World Use Cases

This concept is widely used in intelligent transportation systems.

---

## 🚦 1. Smart Traffic Management

* Monitor congestion in real time
* Adjust traffic signal timings
* Reduce traffic bottlenecks

Problem Solved:

> Manual traffic monitoring is inefficient and reactive.

---

## 🏙️ 2. Smart City Infrastructure

* Collect traffic analytics
* Analyze peak hours
* Urban road planning

Problem Solved:

> Cities need data-driven road planning decisions.

---

## 🚨 3. Emergency Traffic Monitoring

* Detect unusual slowdowns
* Identify accident-prone areas
* Enable faster emergency response

Problem Solved:

> Traffic incidents often go unnoticed until congestion increases.

---

## 🚗 4. Highway Surveillance Automation

* Reduce human CCTV monitoring
* Automatically flag congestion
* Generate traffic reports

Problem Solved:

> Human monitoring is not scalable or accurate.

---

## 🚙 5. Autonomous Driving Research

* Study vehicle behavior patterns
* Model traffic flow dynamics

Problem Solved:

> Self-driving systems require traffic understanding.

---

# 📊 Output Features

✔ Real-time vehicle tracking
✔ Unique ID assignment
✔ Speed estimation
✔ Slow vehicle highlighting (Red boxes)
✔ Congestion alert display
✔ Vehicle & slow vehicle counters

---

# ⚠ Important Notes

* Speed is measured in **pixels per second**
* To convert to km/h:

  * Camera calibration required
  * Known real-world distance reference needed

---

# 🔥 Future Improvements

* Convert speed to km/h using perspective transform
* Lane-based congestion detection
* Vehicle counting line-crossing system
* Store analytics in CSV
* Generate congestion graphs
* Deploy as web dashboard
* Connect to live CCTV feed

---

# 🏁 Project Highlights

✔ End-to-end AI traffic monitoring system
✔ Real-time vehicle tracking
✔ Congestion detection logic
✔ Production-ready structure
✔ Smart city application ready

---

# 👨‍💻 Author

Developed as a Computer Vision & Deep Learning traffic analytics project.


