# Real-Time Vision Monitoring System

A Python-based computer vision application designed to analyze live video streams, detect objects, and track their movement in real time. The system combines deep learning with video-processing tools to provide an extensible foundation for intelligent monitoring applications.

## 🚀 Features

* Real-time object detection from webcam or video streams
* Object tracking with persistent IDs
* Live bounding-box and confidence-score visualization
* Video and image input support
* Configurable detection thresholds
* Real-time FPS monitoring
* Modular Python architecture
* REST API support for integrating vision capabilities with other applications

## 🛠️ Technology Stack

* **Python**
* **PyTorch**
* **YOLO**
* **OpenCV**
* **FastAPI**
* **NumPy**

## 📁 Project Structure

```text
vision-monitoring/
│
├── models/              # Detection and tracking models
├── src/
│   ├── detection/      # Object detection logic
│   ├── tracking/       # Object tracking
│   ├── api/            # REST API endpoints
│   └── utils/          # Helper functions
│
├── tests/               # Automated tests
├── requirements.txt     # Python dependencies
├── config.yaml          # Application configuration
└── README.md
```

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/your-username/vision-monitoring.git
cd vision-monitoring
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate it:

**Windows**

```bash
venv\Scripts\activate
```

**Linux/macOS**

```bash
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## ▶️ Running the Application

Run the vision pipeline:

```bash
python main.py
```

For webcam input, configure the camera source in the application configuration.

For a video file:

```bash
python main.py --source videos/sample.mp4
```

Start the REST API:

```bash
uvicorn src.api.main:app --reload
```

The API can then be used to connect the vision engine with external applications.

## 🔍 How It Works

```text
Camera / Video
      │
      ▼
  OpenCV Input
      │
      ▼
 Object Detection
      │
      ▼
 Object Tracking
      │
      ▼
 Video Analytics
      │
      ├── Detection Results
      ├── Object IDs
      ├── Confidence Scores
      └── FPS Metrics
      │
      ▼
Visualization / REST API
```

## 📊 Possible Applications

The system can serve as a foundation for:

* CCTV monitoring
* Traffic analysis
* People and vehicle counting
* Restricted-area monitoring
* Industrial safety monitoring
* Smart-camera applications
* Retail analytics
* Robotics and autonomous systems

## 🔮 Future Improvements

* Multi-camera support
* Event-based notifications
* Database integration for detection history
* Web-based m
