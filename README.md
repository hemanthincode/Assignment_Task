# Deep Learning Internship Assignment - Face Swapping

## Overview
This project demonstrates the use of a diffusion model to replace the face in a provided human image with another face image. The final output maintains a natural appearance through various image processing techniques.

## Steps
1. **Extract Images from PDF**: Extracted images from the provided PDF file using PyMuPDF.
2. **Face Detection**: Detected faces in the source and target images using Haar Cascades.
3. **Face Alignment**: Aligned the source face with the target face using affine transformation based on facial landmarks.
4. **Histogram Matching**: Matched histograms for better color consistency between the source and target faces.
5. **Face Swapping**: Used the Stable Diffusion model to generate a face-swapped image.
6. **Blending**: Applied Poisson blending for a seamless and natural integration of the source face into the target image.

## How to Run
1. Install the required libraries:
   ```bash
   pip install PyMuPDF opencv-python-headless diffusers torch scikit-image dlib imutils
2. Run the provided Python script:
   python "face_swapping.ipynb"
