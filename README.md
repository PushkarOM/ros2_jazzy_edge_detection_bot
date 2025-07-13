# ros2_jazzy_edge_detection_bot

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

Build the workspace:
```bash
colcon build
```

Source the workspace:
```bash
source install/setup.zsh
#or
source install/setup.bash
```


Usage
Launch the bot simulation with Gazebo and RViz:

```bash
ros2 launch bot_bringup bringup.launch.py
```
Notes
This project uses the ROS 2 Jazzy distribution.

Gazebo runs with software rendering for better compatibility in virtual machines.

Ensure your environment is properly set up with ROS 2 Jazzy before running.

Contributing
Feel free to submit issues or pull requests to improve the bot.

Created by Pushkar — Inspired by a workshop mentor.