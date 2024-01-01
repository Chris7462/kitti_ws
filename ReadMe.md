# Kitti vision: Unraveling Localization and Perception in Autonomous Driving

## TL; DR
### Clone repository:
```bash
git clone --recurse-submodules https://github.com/Chris7462/kitti_ws.git
cd kitti_ws
colcon build --symlink-install
source ./install/setup.bash
```
### Download Kitti ros2bag
Download [KITTi 2011\_09\_29\_drive\_0071](https://drive.google.com/file/d/1PZ7xIgH5Ja_kpzbRrAyZVJ_6ojxR6btw/view?usp=drive_link) and untar the compressed file:

```bash
tar --zstd -xf 2011_09_29_drive_0071_sync_bag.tar.zst
```
Put this uncompressed ros2 bag under the *kitti_ws* folder.

### Launch Kitti
```bash
ros2 launch kitti_launches kitti_main_launch.py
```
The *kitti\_main\_launch.py* launches everything.


## Introduction
In the realm of autonomous driving, accurate localization and robust perception are crucial components for ensuring the safety and efficiency of vehicles. This project aims to leverage the [KITTI dataset](https://www.cvlibs.net/datasets/kitti/setup.php) to showcase advancements in localization and perception algorithms, contributing to the ongoing development of autonomous systems.

## Localization
The [localization](https://github.com/Chris7462/localization) module encompasses implementations of state-of-the-art localization algorithms, such as Simultaneous Localization and Mapping (SLAM), Visual Odometry, and LiDAR Odometry. More details can be found in [localization](https://github.com/Chris7462/localization) repository.

<!--
* Implement state-of-the-art localization algorithms, such as Simultaneous Localization and Mapping (SLAM), Visual Odometry, of LiDAR Odometry, using the KITTI dataset.
* Evaluate the performance of the localization system in different scenarios, including urban environments, highways, and challenging weather conditions.
* Visualize and analyze the accuracy and robustness of the localization algorithm through metrics like trajectory error, pose estimation, and consistency.
-->

## Perception
The [perception](https://github.com/Chris7462/perception) module includes the development of the perception system using deep learning techniques for object detection, classification, and tracking for the Kitti dataset.
<!--
* Utilize convolutional neural networks (CNNs) or other relevant models to identify and track objects such as vehicles, pedestrians, and cyclists.
* Assess the performance of the perception system by measuring metrics like precision, recall, and F1 score, and evaluate its generalization across diverse scenes.
-->

## Tools and Others:
* [Kitti URDF](https://github.com/Chris7462/kitti_urdf)
* [Kitti Launches](https://github.com/Chris7462/kitti_launches)
* [Kitti to ros2bag](https://github.com/Chris7462/kitti_to_ros2bag)
* [Trajectory Server](https://github.com/Chris7462/trajectory_server)
