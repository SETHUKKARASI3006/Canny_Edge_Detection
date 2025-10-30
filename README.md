# Canny_Edge_Detection
This repository contains an implementation of the Canny Edge Detection algorithm. This multi-stage algorithm is widely recognized as an optimal edge detector for various computer vision applications.

## Features
- **Implementation of the Canny Algorithm**: A step-by-step implementation of the classic Canny edge detection process.

- **Core Steps Included**: Implementation covers all stages of the algorithm:

  - **Noise Reduction** (using Gaussian Blur)

  - **Finding the Intensity Gradient** (using operators like Sobel)

  - **Non-Maximum Suppression**

  - **Double Thresholding**

  - **Edge Tracking by Hysteresis**

## Prerequisites
To run this project, you will need to have the following installed:

- **Python** (e.g., Python 3.x)

- **Required Libraries**:

  - `numpy` (for numerical operations)

  - `opencv-python` (or similar image processing library for image I/O and visualization)

  - Add any other specific libraries here, e.g., `matplotlib`.

## Algorithm Steps

The Canny Edge Detection algorithm involves the following sequential steps:

1.  **Gaussian Blurring:** Smooths the image to reduce noise that could lead to false edge detection.
2.  **Gradient Calculation:** Calculates the gradient intensity and direction using derivative masks (e.g., Sobel filters).
3.  **Non-Maximum Suppression (NMS):** Thins the edges by only preserving local maxima of the gradient magnitude.
4.  **Double Thresholding:** Classifies pixels as **strong**, **weak**, or **non-edges** based on high and low thresholds.
5.  **Hysteresis Tracking:** Finalizes the edges by keeping only the **weak** edges that are connected to **strong** edges.
