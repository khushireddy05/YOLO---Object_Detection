# 🚀 YOLO Object Detection Using OpenCV and Python

A comprehensive guide to developing and deploying custom object detection models using **YOLOv8**, **OpenCV**, and **Python**.

---

## ✅ Project Overview

This project demonstrates how to perform **real-time object detection** using the powerful **YOLOv5 (You Only Look Once)** framework, integrated with **OpenCV** for image/video processing, and Python for automation.

### Key Features
- Train custom object detection models using your dataset
- Detect multiple objects in images and videos
- Save detection results and bounding boxes in YOLO format
- Simple integration with OpenCV for visualization and deployment

---

## ⚡ Prerequisites

Install required dependencies before running the project:

```bash
pip install -r requirements.txt
```

Alternatively, install key dependencies manually:

```bash
pip install opencv-python
pip install torch torchvision
pip install labelImg
```
---

🚧 How to Use
1️⃣ Annotate Images

Use LabelImg to annotate images and export annotations in YOLO format.

2️⃣ Train the YOLOv5 Model

Customize data.yaml and run the training script:
```bash
from ultralytics import YOLO

model = YOLO('yolov8m.pt')

model.train(data = '/kaggle/input/datayaml/data.yaml', epochs = 50)
```

3️⃣ Run Object Detection
```bash
python detect.py --source path/to/image_or/video --weights models/yolov8_custom_model.pt

```
Detected images and YOLO-format labels will be saved in the designated output folder.

---

📚 References

YOLOv5 Official GitHub Repository - https://github.com/ultralytics/yolov5

OpenCV Official Site - https://opencv.org/

LabelImg GitHub Repository - https://github.com/tzutalin/labelImg



