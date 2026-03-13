# ROS2 Mobile Manipulator

A mobile manipulator robot built in ROS2, combining a differential drive base with a 2-DOF robotic arm. Designed for autonomous navigation and object manipulation tasks.

---

## Overview

This project implements a mobile manipulator capable of navigating an environment and performing pick and place operations. The robot is built entirely in URDF/Xacro, simulated in Gazebo, and controlled through ROS2 topics.

The long term goal is to integrate autonomous navigation, motor control and mobile manipulation using MoveIt — enabling the robot to autonomously move to a location, plan arm motion and interact with objects.

---

## Robot Architecture

- **Base:** Differential drive mobile base
- **Arm:** 2-DOF robotic arm mounted on base
- **Simulation:** Gazebo with ROS2 Gazebo Bridge
- **Description:** Fully parametric URDF written in Xacro

---

## Current Progress

- [x] Mobile base URDF with differential drive
- [x] 2-DOF robotic arm URDF
- [x] Gazebo simulation setup with plugins
- [x] ROS2 Gazebo Bridge configuration
- [x] Bringup launch file
- [x] Base velocity control via `/cmd_vel`
- [x] Arm joint control via topic publishing

---

## Demo

**Mobile Base Movement**
> Differential drive base moving in a circle by publishing to `/cmd_vel`

https://github.com/bangadmadhav/ros2-mobile-manipulator/media/bot_moving_version1.webm

**Arm Control**
> 2-DOF arm joints being controlled via topic publishing
https://github.com/bangadmadhav/ros2-mobile-manipulator/media/mobile_manipulator_manipulating_robotic_arm.png

---

## Planned Features

- ROS2 Control integration for motor control
- Autonomous navigation with Nav2
- MoveIt integration for arm motion planning
- Full mobile manipulation — navigate to object, plan and execute pick and place

---

## Tech Stack

- ROS2
- Gazebo
- ROS2 Gazebo Bridge
- URDF / Xacro
- Nav2 *(planned)*
- MoveIt *(planned)*
```
