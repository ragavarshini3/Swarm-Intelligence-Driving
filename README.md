# Swarm-Intelligence-Driving
# Swarm Intelligence Driving: Autonomous Vehicles with V2V Communication for Cooperative Driving

## 🚗 Project Overview

Swarm Intelligence Driving is a ROS 2–based autonomous vehicle simulation framework that demonstrates cooperative driving through Vehicle-to-Vehicle (V2V) communication. The project leverages swarm intelligence principles to enable multiple autonomous agents to coordinate their movement, share information, avoid obstacles, and navigate efficiently in a shared environment.

The system is developed using ROS 2, Gazebo, Nav2, SLAM, and robot control packages to simulate intelligent cooperative driving behaviors in dynamic environments.

---

## 🎯 Objectives

* Simulate autonomous vehicle behavior in a ROS 2 environment.
* Enable Vehicle-to-Vehicle (V2V) communication between agents.
* Implement cooperative navigation strategies.
* Demonstrate swarm intelligence concepts in autonomous driving.
* Perform mapping, localization, and path planning.
* Improve safety through collaborative obstacle awareness.

---

## ✨ Features

* 🚘 Autonomous vehicle simulation
* 📡 Vehicle-to-Vehicle (V2V) communication
* 🧠 Swarm intelligence–based coordination
* 🗺️ SLAM-based environment mapping
* 📍 Localization using Nav2
* 🚧 Dynamic obstacle avoidance
* 🎮 Gazebo simulation environment
* 📊 RViz visualization and monitoring
* 🔄 Multi-agent cooperative driving

---

## 🏗️ System Architecture

```text
+----------------------+
| Autonomous Vehicle A |
+----------+-----------+
           |
           | V2V Communication
           |
+----------v-----------+
| Autonomous Vehicle B |
+----------+-----------+
           |
           | Shared Environment Data
           |
+----------v-----------+
| Navigation & Planning|
+----------+-----------+
           |
           v
+----------------------+
| Gazebo + ROS 2       |
+----------------------+
```

---

## 📂 Project Structure

```text
Swarm-Intelligence-Driving/
│
├── src/
│   └── ros_bot/
│       ├── config/
│       ├── description/
│       ├── launch/
│       ├── worlds/
│       ├── package.xml
│       └── CMakeLists.txt
│
├── first_save.yaml
├── first_save.pgm
├── first_serial.data
└── README.md
```

---

## 🛠️ Technologies Used

* ROS 2
* Gazebo Simulator
* Nav2
* RViz
* SLAM Toolbox
* Python
* URDF/Xacro
* Linux (Ubuntu)

---

## 📋 Prerequisites

Before running the project, install:

* ROS 2 Humble (or compatible version)
* Gazebo
* Nav2
* SLAM Toolbox
* RViz2
* Python 3.x

---

## ⚙️ Installation

### Clone the Repository

```bash
git clone https://github.com/ragavarshini3/Swarm-Intelligence-Driving.git
cd Swarm-Intelligence-Driving
```

### Build the Workspace

```bash
colcon build
```

### Source the Workspace

```bash
source install/setup.bash
```

---

## ▶️ Running the Simulation

### Launch Gazebo Environment

```bash
ros2 launch ros_bot launch_sim.launch.py
```

### Launch Robot State Publisher

```bash
ros2 launch ros_bot rsp.launch.py
```

### Start Mapping

```bash
ros2 launch ros_bot online_async_launch.py
```

### Start Navigation

```bash
ros2 launch ros_bot navigation_launch.py
```

---

## 🗺️ Mapping and Localization

The project supports:

* Environment mapping using SLAM Toolbox
* Occupancy grid generation
* Localization using saved maps
* Autonomous path planning with Nav2

Map files:

```text
first_save.yaml
first_save.pgm
```

---

## 📡 Vehicle-to-Vehicle Communication

The V2V module enables vehicles to:

* Exchange positional information
* Share obstacle data
* Coordinate navigation decisions
* Improve traffic flow efficiency
* Reduce collision risks

---

## 🧠 Swarm Intelligence Concepts

The project incorporates swarm intelligence principles:

* Decentralized decision making
* Cooperative behavior
* Distributed information sharing
* Collective navigation
* Adaptive obstacle avoidance

These concepts allow autonomous vehicles to act as a coordinated system rather than isolated agents.

---

## 📸 Simulation Components

### Robot Description

* Camera Sensor
* Depth Camera
* LiDAR Sensor
* Differential Drive Controller

### Simulation Worlds

```text
empty.world
new.world
obstacles.world
```

---

## 📈 Future Enhancements

* Multi-vehicle swarm simulation
* Reinforcement Learning–based coordination
* Dynamic traffic management
* Smart intersection control
* Edge AI integration
* Real-world V2V communication protocols
* Autonomous platooning

---

## 🔬 Applications

* Intelligent Transportation Systems (ITS)
* Smart Cities
* Autonomous Logistics
* Fleet Coordination
* Traffic Optimization
* Cooperative Robotics Research

---

## 👩‍💻 Author

**Ragavarshini**

Engineering Student | Autonomous Systems & AI Enthusiast

GitHub: https://github.com/ragavarshini3

---

## 📜 License

This project is intended for educational and research purposes.

---

## ⭐ Acknowledgements

* ROS 2 Community
* Open Robotics
* Gazebo Simulator
* Nav2 Project
* SLAM Toolbox Contributors
