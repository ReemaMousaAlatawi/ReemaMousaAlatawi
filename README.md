# 🚦 Smart Traffic Management System

### Real-Time Object Detection & Multi-Object Tracking

**YOLOv5 + Deep SORT + OpenCV**

---

## 📖 Introduction

This project is a real-time traffic monitoring and object tracking system that combines **YOLOv5** for object detection with **Deep SORT** for multi-object tracking.

The system detects and tracks vehicles and other objects in traffic video streams while maintaining a unique ID for each detected object across frames.

This project demonstrates how **Computer Vision, Object Detection, and Multi-Object Tracking** can be combined to build intelligent traffic monitoring solutions.

---

## 🎥 Demo

### 🚗 Real-Time Object Tracking

![Traffic Tracking](MOT16_eval/track_all.gif)

### 👤 Pedestrian Tracking

![Pedestrian Tracking](MOT16_eval/track_pedestrians.gif)

---

## ✨ Features

- 🚗 Real-time vehicle and object detection
- 🎯 Multi-object tracking using Deep SORT
- 🆔 Unique ID assignment for tracked objects
- 📹 Video and webcam input support
- ⚡ Real-time processing
- 🧠 YOLOv5 object detection
- 🔍 Deep SORT appearance-based tracking
- 📊 MOT-compatible tracking results

---

## 🛠️ Technologies

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| PyTorch | Deep learning framework |
| YOLOv5 | Object detection |
| Deep SORT | Multi-object tracking |
| OpenCV | Video processing |
| NumPy | Numerical operations |
| Pandas | Data processing |

---

## 🏗️ System Architecture

```text
                    Input Video
                         │
                         ▼
                  ┌─────────────┐
                  │   YOLOv5    │
                  │  Detection  │
                  └──────┬──────┘
                         │
                  Detected Objects
                         │
                         ▼
                  ┌─────────────┐
                  │  Deep SORT  │
                  │   Tracker   │
                  └──────┬──────┘
                         │
                  Object IDs + Tracks
                         │
                         ▼
                Traffic Monitoring
```

---

## 📁 Project Structure

```text
Yolov5_DeepSort_Pytorch/
│
├── deep_sort/
│   ├── deep/
│   ├── sort/
│   └── utils/
│
├── yolov5/
│   ├── models/
│   ├── utils/
│   ├── data/
│   └── detect.py
│
├── MOT16_eval/
│   ├── track_all.gif
│   └── track_pedestrians.gif
│
├── videos/
│   └── Traffic.mp4
│
├── track.py
├── requirements.txt
├── yolov5n.pt
└── README.md
```

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/ReemaMousaAlatawi/ReemaMousaAlatawi.git
cd ReemaMousaAlatawi
```

### 2. Install the required dependencies

Make sure you have **Python 3.8 or later** installed.

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Tracker

### Run the included traffic video

```bash
python track.py --source videos/Traffic.mp4
```

### Run using a webcam

```bash
python track.py --source 0
```

### Run another video

```bash
python track.py --source path/to/video.mp4
```

---

## 📌 Notes

- The system uses YOLOv5 for object detection.
- Deep SORT is used to maintain unique IDs for tracked objects.
- The included `Traffic.mp4` video can be used to test the tracker.
- The tracker supports both video files and webcam input.

---

---

## 🎓 Training Program

**Samsung Innovation Campus – Immersive with Misk Skills**

Samsung Innovation Campus

---

## 👥 Team Members

This project was developed collaboratively as part of the **Samsung Innovation Campus – Immersive with Misk Skills** program.

- **Reema Mousa Alatawi**
- **Majed Alshnifi**
- **Taif Moied**
- **Rana Almohaimeed**
- **Gadah Alqahtani**
- **Meshal Alotaibi**

---

## 🤝 Collaboration

This project was developed as a collaborative team project.  
I contributed to the project, supported the team, and gained hands-on experience in **Computer Vision, Object Detection, and Multi-Object Tracking**.
