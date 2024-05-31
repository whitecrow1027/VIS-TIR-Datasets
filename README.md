# VIS-TIR Datasets
A visible-light and thermal-infrared images datasets for dual-spectrum depth estimation in [paper](https://ieeexplore.ieee.org/document/10146199)

You can download the dataset with [BaiduYun](https://pan.baidu.com/s/1nQt-e3wxJdfMEuafnE7cGQ?pwd=msdd)

If you are inconvenient to use BaiduYun, we will update a download link for Onedrive later.

## Hardware system for data collection
We use two hybrid [RGB-Thermal cameras](https://ieeexplore.ieee.org/document/8794320) which can output optical-aligned visible-light(VIS) and thermal-infrared(TIR) images to build a dual-spectrum stereo camera. A Velodyne-64E LiDAR sensor is used for 3D point cloud to get ground-truth.

The stereo baseline between left and right camera is 0.5m, and the camera focal length is 1.6345*10^3mm

update: add calibration parameter from Matlab. Please note that:
1. The released images have been calibrated. 
2. The calibration parameter of the original image with image size 1280x960. The released images are cut to remove some of the sky area at the top with the final size 1280x800.

![handware system](./img/camera.jpg)

## Data exapmle
For our dual-spectrum stereo camera, each data frame
contains six images: left/right VIS images, left/right TIR image,
and left/right depth map ground-truth.

![data frame example](./img/frame.jpg)

Datasets contains images with varing sences and illuminations.

![sence example](img/example.jpg)

## cites
If the current dataset is helpful to your research, you can cite the following papers：
```
@article{DBLP:journals/tits/GuoQXXK23,
  author       = {Yubin Guo and
                  Xinlei Qi and
                  Jin Xie and
                  Cheng{-}Zhong Xu and
                  Hui Kong},
  title        = {Unsupervised Cross-Spectrum Depth Estimation by Visible-Light and
                  Thermal Cameras},
  journal      = {{IEEE} Trans. Intell. Transp. Syst.},
  volume       = {24},
  number       = {10},
  pages        = {10937--10947},
  year         = {2023},
  url          = {https://doi.org/10.1109/TITS.2023.3279559},
  doi          = {10.1109/TITS.2023.3279559},
  timestamp    = {Mon, 01 Apr 2024 11:14:52 +0200},
  biburl       = {https://dblp.org/rec/journals/tits/GuoQXXK23.bib},
  bibsource    = {dblp computer science bibliography, https://dblp.org}
}

@inproceedings{DBLP:conf/icra/ZhangGGGLSHYWYP19,
  author       = {Yigong Zhang and
                  Yicheng Gao and
                  Shuo Gu and
                  Yubin Guo and
                  Minghao Liu and
                  Zezhou Sun and
                  Zhixing Hou and
                  Hang Yang and
                  Ying Wang and
                  Jian Yang and
                  Jean Ponce and
                  Hui Kong},
  title        = {Build your own hybrid thermal/EO camera for autonomous vehicle},
  booktitle    = {International Conference on Robotics and Automation, {ICRA} 2019,
                  Montreal, QC, Canada, May 20-24, 2019},
  pages        = {6555--6560},
  publisher    = {{IEEE}},
  year         = {2019},
  url          = {https://doi.org/10.1109/ICRA.2019.8794320},
  doi          = {10.1109/ICRA.2019.8794320},
  timestamp    = {Fri, 06 Oct 2023 13:00:13 +0200},
  biburl       = {https://dblp.org/rec/conf/icra/ZhangGGGLSHYWYP19.bib},
  bibsource    = {dblp computer science bibliography, https://dblp.org}
}
```
