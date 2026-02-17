# 🏬 Retail Store Video Analytics System using YOLOv8

An AI-powered retail analytics system that performs **customer detection, tracking, path analysis, heatmap generation, and loitering detection** from surveillance video.

Built using **Ultralytics YOLOv8**, OpenCV, and NumPy.

---

## 📌 Project Overview

This project analyzes retail store CCTV footage to extract customer behavior insights.

The system:

* 👤 Detects customers (person class)
* 🆔 Assigns unique tracking IDs
* 🧭 Tracks movement paths
* 🌡 Generates real-time heatmaps
* ⏱ Detects loitering behavior
* 📊 Displays total customer count
* 🎥 Saves annotated output video

---

## 🎯 Key Features

### ✅ 1. Customer Detection

Detects people using YOLOv8 pre-trained COCO model.

### ✅ 2. Multi-Object Tracking

Tracks customers across frames using built-in tracking.

### ✅ 3. Path Visualization

Draws movement trails showing customer journey inside store.

### ✅ 4. Heatmap Generation

Highlights high-traffic areas inside store.

Hot zones indicate:

* Popular aisles
* Frequently visited shelves
* High engagement areas

### ✅ 5. Loitering Detection

If a customer remains in the store longer than a defined threshold (e.g., 5 seconds), the bounding box turns red.

Useful for:

* Theft prevention
* Suspicious behavior detection
* Security alerts

---

## ⚙️ System Architecture

```
Input Video
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
Annotated Output Video
```

---

## 🛠 Tech Stack

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

## ▶️ Usage

1. Place your retail surveillance video:

```
retail.mp4
```

2. Run the script:

```
python retail_analytics.py
```

3. Output will be saved as:

```
retail_output.mp4
```

---

## 📂 Input & Output

### Input

* Retail CCTV footage (fixed camera recommended)

### Output

Annotated video containing:

* 🟢 Customer bounding boxes
* 🔴 Loitering alerts
* 🔵 Movement trails
* 🌈 Heatmap overlay
* 📊 Customer count display

---

# 🌍 Real-World Applications

---

## 🛒 1. Store Layout Optimization

Identify:

* Most visited aisles
* High-traffic zones
* Underperforming areas

Helps improve product placement and store design.

---

## 💰 2. Sales & Marketing Insights

Analyze:

* Customer movement patterns
* Time spent near specific shelves
* Engagement behavior

Supports data-driven merchandising decisions.

---

## 🛡 3. Loss Prevention & Security

Detect:

* Loitering near high-value items
* Suspicious movement patterns

Enhances retail security automation.

---

## 🏬 4. Smart Retail Analytics

Enable:

* Customer flow analysis
* Peak-hour monitoring
* Staffing optimization

---

## 📊 5. Customer Behavior Research

Useful for:

* Shopping psychology studies
* Heatmap-based marketing analysis
* In-store engagement tracking

---

# 🔥 Why YOLOv8?

* Fast real-time detection
* Lightweight model options
* Easy tracking integration
* Production-ready architecture

---

# ⚠ Limitations

* Speed is not measured in real-world units
* Requires fixed camera for best results
* Does not identify individual customers (only tracks IDs)
* Performance depends on video quality

---

# 🚀 Future Improvements

* Zone-based aisle analytics
* CSV export of customer data
* Generate standalone heatmap image
* Suspicious behavior scoring
* Multi-camera integration
* Dashboard visualization
* Real-time alert system
* Cloud deployment

---

# 📊 Example Use Cases

| Industry           | Application                   |
| ------------------ | ----------------------------- |
| Supermarkets       | Customer flow tracking        |
| Shopping malls     | Crowd analytics               |
| Electronics stores | High-value product monitoring |
| Fashion retail     | Aisle engagement analysis     |

---

# 🏁 Project Highlights

✔ End-to-end retail analytics pipeline
✔ Real-time customer tracking
✔ Behavioral insight extraction
✔ Heatmap visualization
✔ Security monitoring capability
✔ Industry-relevant application

---

# 👨‍💻 Author

Developed as a Computer Vision & AI Retail Analytics project.

---


