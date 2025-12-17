# Self-Driving Vehicle (ROS 2 Bumperbot Workspace)

This repository contains my ROS 2 workspace for a **self-driving mobile robot** based on the *Bumperbot* platform.  
It focuses on **odometry, control and sensor fusion** for autonomous navigation, using ROS 2 nodes written in both Python and C++.

The project is organised as a standard ROS 2 workspace in `bumperbot_ws/` and can be used to simulate or extend a small-scale self-driving vehicle in Gazebo.

---

## 🚀 Main Goals

- Implement a **mobile robot software stack** in ROS 2
- Practice **kinematics, odometry, control and sensor fusion**
- Run and visualise the robot in **Gazebo** and **RViz2**
- Build a solid base for future work on **navigation and autonomous driving**

---

## 🧱 Project Structure

```text
Self-Driving-Vehicle/
└── bumperbot_ws/
    ├── src/                 # ROS 2 packages for the Bumperbot robot
    │   ├── bumperbot_description/   # URDF/Xacro models and robot description
    │   ├── bumperbot_bringup/       # Launch files for simulation / robot bring-up
    │   ├── bumperbot_control/       # Control nodes (velocity, PID, etc.)
    │   ├── bumperbot_sensors/       # Sensor interfaces and fusion nodes
    │   ├── bumperbot_localization/  # Odometry & localization nodes
    │   └── bumperbot_utils/         # Helper utilities (msgs, configs, etc.)
    ├── CMakeLists.txt
    ├── package.xml
    └── (build/, install/, log/ after compilation)
