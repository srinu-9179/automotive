# Atomotive Helmet-Detection-using-yoloV8
This project aims to develop an automated helmet detection system using Yolov8.

 Week 1 – Project Initialization & Planning
Objectives

*Decide project title and theme.

*Understand the problem domain (helmet detection).

*Explore existing research and tools for object detection.

*Set up GitHub repository and environment.

Tasks Completed:

#On Monday	Title Finalization	Selected project title: Helmet Detection using yolov8 (Automotive Theme)

#On Tuesday		GitHub Setup	Created and initialized GitHub repository

#On Wednesday	Problem Definition	Defined scope: Detect riders and identify helmet usage for road safety.

#On Thursday	Tool Selection	Finalized Python, YOLOv8, and OpenCV for implementation.

#On Friday	Studied about YOLOv5 and YOLOv8 architectures for object detection..

#On Saturday	collab setup and install Dependencies
Step 1 — Enable GPU

Menu → Runtime → Change runtime type → Hardware accelerator → GPU
Then Save.

Step 2 — Install dependencies
!pip install ultralytics opencv-python matplotlib pandas numpy


Check everything works:

from ultralytics import YOLO
import cv2, torch

print("✅ OpenCV:", cv2.__version__)
print("✅ Torch:", torch.__version__)
print("✅ CUDA available:", torch.cuda.is_available())
print("✅ YOLO ready!")

Step 3 — Run a sample detection (Week 1 goal)
from ultralytics import YOLO

# Load pretrained YOLOv8 small model
model = YOLO('yolov8n.pt')

# Run inference on sample image
results = model.predict(source='https://ultralytics.com/images/bus.jpg', save=True)

print("✅ Inference complete! Check /content/runs/predict for output.")


#On Sunday	Documentation	Wrote README.md with objectives and week summary.
