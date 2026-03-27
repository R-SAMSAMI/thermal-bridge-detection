# Thermal Bridge Detection using YOLO and UAS Thermal Imagery

This project presents a deep learning–based framework for detecting rooftop thermal bridges using thermal imagery collected from Uncrewed Aerial Systems (UAS). The focus is on lightweight object detection models that balance accuracy and computational efficiency for practical deployment.

---

## Overview

Thermal bridges are localized areas of increased heat transfer in building envelopes. Detecting them at scale using aerial thermal imagery is challenging and traditionally relies on manual interpretation.

This project evaluates modern YOLO architectures (YOLOv8, YOLOv11, YOLOv26) for automated detection using thermal-only imagery, reflecting realistic inspection conditions.

---

## Project Structure

thermal-bridge-detection/

- thermal_bridge_detection.ipynb  
- thermal_bridge_detection_figures.ipynb  
- figures/

---

## Methods

- Dataset: TBBRv2 (Thermal Bridges on Building Rooftops)  
- Input: Thermal imagery (single modality)  
- Models:
  - YOLOv8 (n, s, m, l)
  - YOLOv11 (n, s, m, l)
  - YOLOv26 (n, s, m, l)
- Evaluation Metrics:
  - mAP@0.5
  - mAP@0.5–0.95
  - Precision
  - Recall
  - F1-score

---

## Sample Results

![Model Comparison](figures/Figure10.png)

*Qualitative and quantitative comparison of YOLOv8, YOLOv11, and YOLOv26 models for thermal bridge detection using UAS thermal imagery.* for full visualizations and analysis.

---

## Related Publication

This repository supports the following research work currently under review:

Samsami, R., and Jafari Kang, S. (2026).  
*Lightweight YOLO-Based Detection of Rooftop Thermal Bridges Using Uncrewed Aerial System (UAS) Thermal Imagery: Comparative Evaluation of Modern YOLO Architectures.*  
ASCE Open: Multidisciplinary Journal of Civil Engineering (under review).

If you use this work, please cite the above paper.

---

## Setup

Install dependencies:

pip install ultralytics opencv-python numpy matplotlib pandas torch

---

## Dataset

This project uses the Thermal Bridges on Building Rooftops dataset (TBBRv2).

The dataset and original implementation can be accessed here:  
https://github.com/Helmholtz-AI-Energy/TBBRDet

The dataset includes UAS-collected thermal imagery with annotated rooftop thermal bridge regions.

---

## Notes

- This repository does not redistribute the dataset.  
- Please download the dataset from the official source above.  
- Paths in notebooks may need to be adjusted for your environment.   

---

## Author

Reihaneh Samsami  
Assistant Professor, Construction Management  
University of New Haven
