# Multi-Class Object Detection (CNN)

CNN-based multi-class object detection and localization project that predicts both object class labels and bounding box coordinates from images.

---

## Overview

This project demonstrates an end-to-end computer vision pipeline:

- Image preprocessing and augmentation  
- CNN feature extraction  
- Multi-class classification head  
- Bounding-box regression head  
- Training + evaluation workflow  
- Visualization of detection outputs

---

## Model Design (High Level)

CNN Backbone → Feature Maps →  
- Classification Head (Softmax class probabilities)  
- Bounding Box Head (x, y, w, h regression)

Loss:
- Cross-Entropy (classification)
- Smooth L1 / MSE (bounding box regression)

---

## Key Features

- Multi-class object detection + localization
- Data augmentation for better generalization
- Training script structure under `src/`
- Outputs folder for predictions and evaluation plots
- Screenshots folder for detection examples

---

## Tech Stack

- Python
- Deep Learning (CNN)
- NumPy
- OpenCV (visualization)
- Matplotlib (plots)

---

## Repository Structure

- `src/` — model + training / inference scripts  
- `notebooks/` — experiments and EDA  
- `data/` — dataset notes / samples  
- `outputs/` — prediction outputs and evaluation artifacts  
- `screenshots/` — example detection results  

---

## How to Run (Template)

```bash
pip install -r requirements.txt
python src/main.py
