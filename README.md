# VIS-TIR Datasets
A visible-light and thermal-infrared images datasets for dual-spectrum depth estimation

update: we will publish the dataset after our paper accepted

## Hardware system for data collection
We use two hybrid [RGB-Thermal cameras](https://ieeexplore.ieee.org/document/8794320) which can output optical-aligned visible-light(VIS) and thermal-infrared(TIR) images to build a dual-spectrum stereo camera. A Velodyne-64E LiDAR sensor is used for 3D point cloud to get ground-truth.

![handware system](./img/camera.jpg)

## Data exapmle
For our dual-spectrum stereo camera, each data frame
contains six images: left/right VIS images, left/right TIR image,
and left/right depth map ground-truth.

![data frame example](./img/frame.jpg)

Datasets contains images with varing sences and illuminations.

![sence example](img/example.jpg)