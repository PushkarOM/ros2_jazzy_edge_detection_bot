# ros2_jazzy_edge_detection_bot
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

[![ROS Jazzy](https://img.shields.io/badge/ROS-2%20Jazzy-blue?logo=ros)](https://docs.ros.org/en/jazzy/)


## Overview
This project implements an **Edge Detection Bot** using ROS 2 Jazzy. The bot is designed to detect edges in its environment and navigate accordingly. The implementation follows a workshop guided by a mentor and includes simulation using Gazebo and visualization with RViz.

## Features
- Edge detection node for obstacle avoidance
- Differential drive controller setup
- Simulation environment using Gazebo with software rendering support
- RViz visualization with robot model and sensor data
- Modular ROS 2 packages: `bot_description`, `bot_controller`, `bot_bringup`, and `bot_script`

## Installation
1. Clone the repository:
   ```bash
   git clone --recurse-submodules git@github.com:PushkarOM/ros2_jazzy_edge_detection_bot.git
   cd ros2_jazzy_edge_detection_bot
   ```
Make sure you are in the root of the workspace (`ros2_jazzy_edge_detection_bot`) when running these commands.
Build the workspace:
```bash
colcon build --symlink-install
```

Source the workspace:
```bash
source install/setup.zsh
#or this is you are using bash
source install/setup.bash
```


Usage
Launch the bot simulation with Gazebo and RViz:

```bash
# Terminal 1
ros2 launch bot_bringup bringup.launch.py

# Terminal 2
ros2 run bot_script edge_detection
```
**Notes :**
1) This project uses the ROS 2 Jazzy distribution.

2) Gazebo runs with software rendering for better compatibility in virtual machines.

Ensure your environment is properly set up with ROS 2 Jazzy before running.

### Contributing
Feel free to submit issues or pull requests to improve the bot.

### License
This project is licensed under the [MIT License](LICENSE).

### Credits

This project is based on the original work by [Curious-Utkarsh](https://github.com/Curious-Utkarsh) in the ROS 2 Humble workshop.

Original repository: [https://github.com/Curious-Utkarsh/bot_ws](https://github.com/Curious-Utkarsh/bot_ws)

Created by Pushkar — Inspired by a workshop mentor [@Curious-Utkarsh](https://github.com/Curious-Utkarsh).