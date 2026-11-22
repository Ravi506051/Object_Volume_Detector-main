# Object Dimension Detector

A Streamlit computer-vision prototype that estimates object dimensions from images using monocular depth estimation and a known-size reference object.

## Run locally

~~~bash
git clone https://github.com/Ravi506051/Object_Volume_Detector-main.git
cd Object_Volume_Detector-main
python -m venv .venv
# Windows: .venv\Scripts\activate
pip install -r requirements.txt
streamlit run app.py
~~~

The first run may need to download the configured pretrained depth model. See Getting_Started.md for project-specific setup notes. main.py and the notebooks contain related experiments.

## Measurement workflow

Provide an image, identify a reference object with known dimensions, estimate relative depth, then review the scale-calibrated dimension estimate.

## Calibration and limits

Monocular depth is generally relative. Scale depends on reference size, camera angle, perspective, object boundaries, and image quality. Treat outputs as approximate. Validate against independently measured objects and report errors across multiple examples before practical use.

## Reference-object calibration

The app uses a known-size reference for scale calibration; its default reference width is 0.0856 m (an ID-1 card). Confirm the selected reference and its real measurement before interpreting estimates. Changing the camera viewpoint or reference size changes the scale.


## Maintainer

Ravi Kumar Rao · [GitHub](https://github.com/Ravi506051)
