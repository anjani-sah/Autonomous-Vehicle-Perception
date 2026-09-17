# Autonomous Vehicle Perception

An end-to-end computer vision project for autonomous vehicle perception, integrating object detection, lane segmentation, and multi-object tracking into a unified pipeline.

## Project Overview

This project explores a vision-based perception pipeline for autonomous vehicles. The system combines YOLOv8 for object detection, lane segmentation for road understanding, and DeepSORT for multi-object tracking.

The project is implemented in a Jupyter Notebook and is supported by the corresponding research paper included in this repository.

## Main Project

### Integrated Object Detection, Lane Segmentation, and Tracking for Autonomous Vehicles Using YOLOv8 and DeepSORT

The core project integrates three important perception tasks:

1. Object Detection
2. Lane Segmentation
3. Multi-Object Tracking

The objective is to provide a unified perception pipeline that can identify road objects, understand lane structure, and maintain object identities across video frames.

## Object Detection

YOLOv8 is used for detecting objects in road scenes.

The detection pipeline is designed to identify objects relevant to autonomous driving scenarios and produce bounding boxes and class predictions.

Key components:
- YOLOv8
- Bounding box detection
- Object classification
- Confidence scores
- Road scene analysis

## Lane Segmentation

The project includes lane segmentation to identify lane boundaries and road structure from visual input.

Lane information can be used together with object detection and tracking to provide richer scene understanding for autonomous vehicle applications.

Key components:
- Lane detection
- Pixel-level road structure analysis
- Lane boundary identification
- Visual road scene understanding

## Multi-Object Tracking

DeepSORT is used to track detected objects across frames.

Tracking helps maintain consistent identities for objects as they move through the scene.

Key components:
- DeepSORT
- Object identity tracking
- Bounding box association
- Frame-to-frame tracking

## Integrated Pipeline

The overall perception workflow follows this structure:

```text
Input Road Image / Video
          |
          v
     YOLOv8 Detection
          |
          +-------------------+
          |                   |
          v                   v
   Detected Objects     Lane Segmentation
          |                   |
          +---------+---------+
                    |
                    v
             DeepSORT Tracking
                    |
                    v
        Integrated Scene Understanding
```

## Dataset

The project uses the KITTI dataset for autonomous driving perception experiments.

A smaller working dataset was prepared for model development and experimentation to make training and testing more manageable.

The dataset supports road-scene analysis involving vehicles and other objects commonly encountered in autonomous driving environments.

## Technologies Used

- Python
- Jupyter Notebook
- YOLOv8
- DeepSORT
- OpenCV
- Computer Vision
- Deep Learning
- KITTI Dataset

## Repository Contents

```text
Autonomous-Vehicle-Perception/
|
├── Autonomous_Vehicle_Perception.ipynb
│   Main implementation notebook containing the perception pipeline
│
├── Integrated_Object_Detection_Lane_Segmentation_and_Tracking_for_Autonomous_Vehicles_Using_YOLOv8_and_DeepSORT.pdf
│   Research paper describing the integrated perception approach
│
├── .gitattributes
│   Git configuration file
│
└── README.md
    Project documentation
```

## Notebook

The `Autonomous_Vehicle_Perception.ipynb` notebook contains the implementation and experimentation workflow for the project.

It can be opened using:

- Jupyter Notebook
- JupyterLab
- Google Colab

## Research Paper

The repository includes the research paper:

`Integrated Object Detection, Lane Segmentation, and Tracking for Autonomous Vehicles Using YOLOv8 and DeepSORT`

The paper documents the methodology and integrated perception approach used in the project.

## Project Objectives

- Build an autonomous vehicle perception pipeline
- Detect objects in road scenes
- Segment lane structures
- Track multiple objects across frames
- Combine different perception tasks into one workflow
- Study the application of YOLOv8 and DeepSORT in autonomous driving

## Applications

The approach can support autonomous driving systems in tasks such as:

- Vehicle detection
- Pedestrian detection
- Road scene understanding
- Lane awareness
- Multi-object tracking
- Autonomous navigation and perception

## How to Run

Clone the repository:

```bash
git clone https://github.com/anjani-sah/Autonomous-Vehicle-Perception.git
cd Autonomous-Vehicle-Perception
```

Install the main Python dependencies:

```bash
pip install ultralytics opencv-python numpy matplotlib torch torchvision
```

Open the notebook:

```bash
jupyter notebook Autonomous_Vehicle_Perception.ipynb
```

You can also upload the notebook to Google Colab and run it there.

## Future Improvements

Potential extensions include:

- Larger-scale training and evaluation
- Improved lane segmentation accuracy
- Real-time video inference
- Model optimization for edge devices
- Integration with additional autonomous driving datasets
- Sensor fusion with LiDAR or other vehicle sensors
- Deployment on embedded hardware

## Author

Anjani Sah

GitHub: https://github.com/anjani-sah

Repository: https://github.com/anjani-sah/Autonomous-Vehicle-Perception
