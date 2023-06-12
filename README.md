# TurtleBot3 Remote Control

This project implements a TurtleBot3 robot with an Android app for remote control and collision avoidance logic using LIDAR data.

## Nodes

### Remote Control Node

This node is responsible for receiving user inputs from the Android app, translating them into motor control commands, and publishing them on a specific ROS topic. It allows users to remotely control the TurtleBot3's movements.

#### Subscribed Topics

- None

#### Published Topics

- `/cmd_vel` (geometry_msgs/Twist)

  This topic publishes Twist messages to control the TurtleBot's wheels and movements.

#### Parameters

- None


## Installation

1. Make sure you have ROS installed on your machine. If not, follow the ROS installation instructions at http://wiki.ros.org/ROS/Installation.

2. Clone this repository into your ROS workspace:

   ```bash
   $ cd <your_ros_workspace>/src
   $ git clone <repository_url>

3. Build the workspace:

$ cd <your_ros_workspace>
$ catkin build
