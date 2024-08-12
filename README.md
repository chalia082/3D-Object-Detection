# ToF Sensor Data Processing

This repository contains code and documentation for processing data obtained from a Time-of-Flight (ToF) sensor. The notebook provides functionality to read, process, and visualize point cloud data (X, Y, Z, I) from the sensor.

## Project Overview

The project focuses on dimensioning and analyzing data captured by a ToF sensor. This includes:

- Reading Point Cloud data from a binary file.
- Applying median filtering to reduce noise in the data.
- Extracting depth maps and intensity images from the sensor data.
- Compensating for geometric distortion using camera intrinsics.

## Files in the Repository

- **Final_Dimensioning.ipynb**: The main Jupyter notebook containing the code for reading and processing ToF sensor data.

## Requirements

To run the notebook, the following Python packages are required:

- `cv2` (OpenCV)
- `matplotlib`
- `numpy`
- `scipy`

You can install the required packages using the following command:

```bash
pip install opencv-python-headless matplotlib numpy scipy
```

## Usage

1. Read Point Cloud Data: The notebook includes a function read_PCL(sz, fileName) to read point cloud data from a binary file. The function returns X, Y, Z coordinates and intensity information.

2. Process Data: The data is processed to create depth maps and intensity images, with optional median filtering to mitigate noise.

3. Visualization: Use matplotlib to visualize the depth maps and intensity images.

## Running the Notebook

To run the notebook:

Clone the repository:
```
git clone https://github.com/chalia082/3D-Object-Detection
cd your-repository-name
jupyter notebook Final_Dimensioning.ipynb
```
