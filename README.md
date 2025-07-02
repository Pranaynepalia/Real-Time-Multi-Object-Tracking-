# ** Real-Time Multi-Object Tracking with Speed Estimation **
This project implements a real-time multi-object tracking system enhanced with speed estimation using computer vision techniques. It is designed to assist in emergency or rescue operations by detecting, tracking, and calculating the speed of multiple objects (e.g., vehicles, people) from live video streams or recorded footage.

# ** Features **
✅ Real-time object detection using YOLOv8
✅ Multi-object tracking using Deep SORT / Custom SORT
✅ Speed estimation for each tracked object (in km/h)
✅ Kalman Filter for robust tracking
✅ OpenCV-based visualization of bounding boxes, IDs, and speed
✅ Modular design for easy extension (e.g., counting, alerts)

# ** Use Cases **
🛣️ Monitoring vehicles for over-speeding
🧑‍🚒 Tracking individuals in rescue missions
🚁 Surveillance via drones
🚨 Emergency scene analysis

# ** Requirements **
Python 3.8+
OpenCV
NumPy
torch
ultralytics (for YOLOv8)
filterpy

# ** 🚀 How It Works **
YOLOv8 detects objects frame-by-frame.
Tracker assigns consistent IDs to objects across frames.
Speed is calculated using:
    Displacement between object centroids
    Frame rate (FPS)
    Pixel-to-meter conversion (PPM)