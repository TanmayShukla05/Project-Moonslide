# Project Moonslide

Project Moonslide is an Astronomy Club, IIT Kanpur mentorship project focused on automated lunar landslide detection using Chandrayaan-2 imagery. The project combines computer vision, remote sensing, planetary science, and machine learning to identify landslide-prone regions on the lunar surface.

## Mentors
- Mihir
- Shreyansh
- Tanmay
- Tripti

## Mentees
- Anuj
- Arnav
- Harshit
- Kartik
- Mayank
- Niharika
- Sayantan
- Sheetal

## Project Overview

The project aims to build an automated landslide detection pipeline for Chandrayaan-2 satellite imagery by leveraging modern computer vision and machine learning techniques.

Key components include:

- Unsupervised computer vision pipeline for automatic generation of labeled training data.
- YOLOv8-based object detection framework for landslide identification.
- Physics-guided feature extraction using slope, aspect, structure tensor anisotropy, and Chebyshev polynomial fitting.
- Large-scale processing of Chandrayaan-2 imagery and elevation products.
- GIS-assisted spatial analysis of detected landslide regions.

## Technical Highlights

- Built an unsupervised CV pipeline that auto-generates labeled training data for a YOLOv8 object detector, eliminating manual annotation bottlenecks.
- Designed a 9-stage data pipeline:

```text
PDS4 Parsing
    ↓
Newton-Raphson Coordinate Solving
    ↓
Memory-Efficient Binary I/O
    ↓
Sobel / Gaussian Filtering
    ↓
Physics-Guided Feature Extraction
    ↓
Automatic Label Generation
    ↓
YOLO Dataset Creation
    ↓
Model Training
    ↓
Evaluation & Analysis
