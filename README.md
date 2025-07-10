
# Perception and Navigation for Mobile Robots and UAVs

This repository contains multiple sub-projects focused on sensor fusion, perception, and navigation using various sensor combinations on mobile robots such as the Husky A200 and a quadcopter. Each folder contains specific experiments or implementations involving different combinations of sensors for localization and navigation.

---

## 📁 Folder Structure and Descriptions

### 🛩️ Quadcopter-Based Sensor Fusion

- **IMU+Barometer+GPS+Magnetometer_Using_Quadcopter**  
  Combines inertial measurements with barometric pressure, GPS, and magnetometer data for altitude and orientation estimation.

- **IMU+GPS+Lidar_Using_Quadcopter**  
  Uses GPS for global positioning, LIDAR for obstacle sensing, and IMU for attitude estimation to navigate the quadcopter safely in outdoor environments.

- **IMU+Radar+GPS_Using_Quadcopter**  
  Integrates radar for long-range obstacle detection with GPS and IMU data for robust navigation in GPS-available environments.

- **IMU+Ultra_wideband_Using_Quadcopter**  
  Fuses IMU with UWB data for precise indoor localization without relying on GPS.

- **IMU+VisualOdometry_Using_Quadcopter**  
  Implements visual odometry using onboard cameras, integrated with IMU data for pose estimation.

- **IMU+VisualSLAM_Using_Quadcopter**  
  Full SLAM pipeline combining camera data with IMU measurements to simultaneously localize and map the environment.

---

### 🤖 Husky A200-Based Sensor Fusion

- **IMU+Camera_Using_Husky_A200**  
  Uses an onboard camera and IMU for localization and movement tracking in indoor or semi-structured environments.

- **IMU+GPS+Wheel_Encoder_Using_Husky_A200**  
  Combines odometry (wheel encoders), GPS, and IMU for outdoor navigation with drift correction.

- **IMU+Lidar+Camera_Using_Husky_A200**  
  Implements a sensor suite of LIDAR, camera, and IMU for visual-LIDAR odometry or SLAM-based navigation.

- **IMU+Wheel_Encoders+Camera_Using_Husky_A200**  
  Uses wheel odometry and camera data fused with IMU to navigate indoor structured environments.

- **IMU+Wheel_Encoders+Lidar_Using_Husky_A200**  
  Combines LIDAR with wheel encoders and IMU to implement a SLAM system or local path planning.

## 🎯 Objective

The core objective of this repository is to:
- Implement and compare different **sensor fusion** strategies for pose estimation.
- Study the effects of sensor drift, noise, and availability.
- Provide practical ROS-based configurations for both indoor and outdoor robot localization.

Each folder is self-contained and includes:
- Sensor configuration
- ROS launch files
- Data recording and playback scripts (bag files, where applicable)
- Pose estimation code or pipelines

---

## 📜 License

This project is licensed under the [Apache License ](./LICENSE).

---

## 🤝 Contributions

Contributions are welcome! If you want to add new sensor fusion techniques, navigation algorithms, or improve documentation, feel free to open a PR.

