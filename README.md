# Camera Calibration Using OpenCV

This project implements a camera calibration pipeline using OpenCV. The goal of camera calibration is to estimate the intrinsic camera parameters and lens distortion coefficients in order to correct image distortion and enable accurate computer vision measurements.

The calibration process is performed using multiple images of a chessboard pattern captured from different angles.

## Overview

Camera calibration is a fundamental step in computer vision applications that require geometric accuracy, such as 3D reconstruction, augmented reality, and robotics.  
This project uses OpenCV’s calibration functions to compute:

- Camera intrinsic matrix
- Distortion coefficients
- Rotation and translation vectors

## Requirements

To run this project, you need:

- Python 3.7 or higher
- OpenCV
- NumPy

## Install the required dependencies using pip:

```
pip install opencv-python numpy
```
Installation

## Clone the repository:

```
git clone https://github.com/your-repo/camera-calibration-opencv.git
cd camera-calibration-opencv
```

## Usage

Prepare Calibration Images

Capture multiple images of a chessboard pattern.

Ensure:

Different orientations and distances

Good lighting

The entire chessboard is visible

Place all images in the specified calibration folder.

Run Calibration

Execute the calibration script:
```
python calibration.py
```

## Output

After running the script, the following parameters are computed and displayed:

Camera matrix (intrinsic parameters)

Distortion coefficients

Rotation and translation vectors

Reprojection error (optional)

These parameters can be used to undistort images or as input for further computer vision tasks.

## Computer Vision Techniques Used

Camera Calibration

Corner Detection

Geometric Transformations

Lens Distortion Correction
