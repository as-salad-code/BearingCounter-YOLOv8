# AI-Assisted Real-Time Part Counting for Heat Treatment Furnace

## Overview
This project presents an AI-powered computer vision system for **real-time part counting** at both the inlet and outlet sections of a multistage heat treatment furnace. By leveraging the **YOLOv8 object detection model**, the system delivers highly accurate performance in challenging industrial environments, ensuring reliability and efficiency for monitoring production lines.

---

## Problem Statement
During the heat treatment of bearing components, parts are moved through multiple processing stages inside the furnace. Monitoring the number of parts entering and exiting is critical — if fewer parts exit than those entering, it indicates that some parts are stuck within the furnace. This can lead to **quality degradation** of materials and increased production risks. Hence, a robust and automated counting mechanism is essential.

---

## Objectives
- Build a computer vision system for **real-time part counting** at inlet and outlet sections.  
- Achieve **99.9% accuracy** using the YOLOv8 deep learning model.  
- Ensure **reliable performance in harsh industrial conditions** such as heat, dust, and vibrations.  
- Optimize the use of hardware for cost-effectiveness and scalability.  

---

## Challenges
- Small part dimensions (**25–75 mm**).  
- Harsh conditions with **dust, vibration, and temperatures up to 70°C**.  
- **Variable conveyor speeds** at the inlet depending on part size.  
- **Random, overlapping movement** of parts at the outlet, causing occlusion.  

---

## Methodology
1. **Data Acquisition** – Capturing video streams from furnace inlet and outlet sections.  
2. **Preprocessing** – Frame extraction and resizing for consistency.  
3. **Annotation** – Labeling parts for model training.  
4. **Detection** – Training and applying YOLOv8 for part identification.  
5. **Counting** – Real-time object counting with validation against annotated data.  

---

## Results
- **Perfect classification** between `ring` and `background` classes (100% accuracy).  
- **No misclassifications** (zero off-diagonal confusion matrix entries).  
- Achieved **99.96% model accuracy** with zero false positives/negatives.  
- **Robust handling** of overlapping parts without compromising accuracy.  
- Balanced dataset ensured high reliability across conditions.  

---

## Implementation
The system includes:  
- Training scripts for YOLOv8 model development.  
- Prediction modules for real-time part detection and counting.  
- Frame extraction tools for dataset preparation.  
- Evaluation scripts for testing performance metrics.  

---

## Requirements
- Python 3.8+  
- OpenCV  
- Ultralytics YOLOv8  
- CUDA-enabled GPU (recommended for training and inference)  

---
## ⚙️ Installation

```bash
# Clone the repository
git clone https://github.com/as-salad-code/BearingCounter-YOLOv8.git
cd BearingCounter-YOLOv8

# Install dependencies
pip install -r requirements.txt
```



## Usage
### Training
```bash
# Navigate to the Training directory
cd Training

# Run the training notebook
jupyter notebook Training.ipynb
```

### Prediction
```bash
# For real-time prediction on video
python Predict.py
```

### Frame Extraction
```bash
# To extract frames from video for annotation
python frame.py
```


## Project Team
- Ms. [Sharvari Korde - LinkedIn](https://www.linkedin.com/in/sharvari-korde-85b993268/)
- Mr. [Aditya Chavan - LinkedIn](https://www.linkedin.com/in/aditya-chavan-5117aa268/)
- Mr. [Bhavin Baldota - LinkedIn](https://www.linkedin.com/in/bhavin-baldota-103553234/)
- Mr. [Saumya Shah - LinkedIn](https://www.linkedin.com/in/saumya-shah-9b2579273/)

<img width="4608" height="3456" alt="SKF" src="https://github.com/user-attachments/assets/27913676-56fc-4f98-bc6e-cc91aebb1399" />

