# Object Dimension Estimation from Images

A computer-vision application that explores estimating object dimensions and distance from one or more camera images using monocular depth estimation and a known reference measurement.

## Workflow
1. Upload a front image and, optionally, a side image.
2. Estimate relative depth using a pre-trained depth model.
3. Select a reference object with a known real-world dimension.
4. Calibrate scale from the reference measurement.
5. Estimate object dimensions and distance.
6. Combine views when the two-view workflow is used.

## Technology
Python · Streamlit · Computer Vision · Depth Estimation · DPT

## Getting started
```bash
git clone https://github.com/Ravi506051/Object_Volume_Detector-main.git
cd Object_Volume_Detector-main
pip install -r requirements.txt
```
Launch the Streamlit entry point specified in the repository. Review the model setup instructions before running inference.

## Accuracy considerations
Monocular depth maps are generally relative, and dimension estimates depend on camera geometry, reference-object accuracy, image quality and object boundaries. Treat measurements as approximate unless calibrated against physical measurements.

## Future improvements
Add calibration examples, uncertainty ranges, repeatability tests and comparisons against measured ground truth.

## Maintainer
**Ravi Kumar Rao** · [GitHub](https://github.com/Ravi506051)

## Skills Demonstrated

- Computer vision
- monocular depth estimation
- reference-based calibration
- image processing
- measurement uncertainty.

## Portfolio Context

This project is part of my hands-on learning portfolio. The repository documents the workflow and implementation; results should be reproduced from the included code and data before being used in reports or professional claims.
