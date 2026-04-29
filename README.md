# Hybrid Crowd Counting and Real-Time Alert System

## Overview
This project implements a hybrid crowd monitoring system that combines object detection (YOLOv12) and density estimation (CSRNet-Lite) to accurately estimate crowd size in real-time scenarios.

The system dynamically switches between detection and density-based approaches using a fusion strategy to handle both sparse and highly congested crowds.

---

## Key Features
- Hybrid model combining YOLOv12 (detection) and CSRNet-Lite (density estimation)
- Dynamic fusion logic for improved counting accuracy
- Real-time processing using RTSP video streams
- Density map dimming for noise reduction
- Automated alert system using MQTT and Telegram APIs

---

## Methodology
- Detection Branch: YOLOv12 for identifying individuals in sparse scenes  
- Density Branch: CSRNet-Lite for estimating counts in dense crowds  
- Fusion Logic: Selects optimal output based on crowd conditions  
- Preprocessing: Frame slicing for real-time performance  
- Post-processing: Density map dimming to suppress background noise  

---

## Results
- Mean Absolute Error (MAE): **8.7** (ShanghaiTech Dataset)
- 37% improvement over detection-only approaches
- 5% improvement over density-only approaches
- Real-time performance: **~16 FPS**

---

## Tech Stack
- Python
- PyTorch
- OpenCV
- YOLOv12
- CSRNet-Lite
- MQTT
- Google Colab

---

## Project Structure

---

## How to Run
1. Open the notebook in Google Colab
2. Install required dependencies
3. Run all cells sequentially
4. Provide input video stream or dataset

---

## Note
- Outputs have been removed for a cleaner repository
- Run all cells to reproduce results
- Dataset and model weights are not included due to size constraints

---

## Publication
This work is published in:
**I3CTCON Conference**

---

## Future Improvements
- Multi-camera integration
- Edge deployment optimization
- Improved fusion strategies using learning-based approaches

---

## Author
**Sripriya A H**
