# Object Dimension Estimation from Images

A computer-vision application exploring object dimension and distance estimation from camera images using monocular depth estimation and a known reference measurement.

## Workflow
1. Upload a front image and, optionally, a side image.
2. Estimate relative depth with a pretrained depth model.
3. Select a reference object with a known real-world dimension.
4. Calibrate the scale using the reference measurement.
5. Estimate object dimensions and distance.
6. Combine views when the two-image workflow is enabled.

## Technology
Python · Streamlit · Computer Vision · Depth Estimation · DPT

## Setup
```bash
git clone https://github.com/Ravi506051/Object_Volume_Detector-main.git
cd Object_Volume_Detector-main
pip install -r requirements.txt
```
Launch the Streamlit entry point specified in the repository and follow its model setup instructions.

## Technical Considerations
Monocular depth maps are generally relative rather than absolute. Estimated dimensions depend on camera geometry, reference-object accuracy, image quality, perspective, and object boundaries. Treat outputs as approximations unless validated against physical measurements.

## Validation Ideas
- Compare estimates with ruler or caliper measurements.
- Repeat captures at different distances and angles.
- Record absolute and percentage measurement error.
- Test objects with different shapes and surface textures.

## Future Improvements
Add calibration guidance, uncertainty ranges, repeatability tests, and a benchmark against measured ground truth.

## Maintainer
**Ravi Kumar Rao** · [GitHub](https://github.com/Ravi506051)
