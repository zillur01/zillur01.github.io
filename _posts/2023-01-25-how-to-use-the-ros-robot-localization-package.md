---
layout: post
title: How to Use the ROS Robot Localization Package to Fuse Multiple Localization Sensors Data
date: 2023-01-25
description: In this article, I described how to perform sensor fusion using an Extended Kalman Filter in ROS. Highly recommended for autonomous robotics enthusiasts.
redirect: https://medium.com/@zillur-rahman/how-to-use-the-ros-robot-localization-package-534fe04014d3
external_source: Medium
tags: [ROS, Sensor Fusion, Kalman Filter, Robotics]
categories: [Robotics]
feed_content: >
  This article introduces the ROS robot_localization package for beginners who want to fuse wheel
  encoder and IMU data for mobile robot localization. It explains why multiple sensors are needed,
  how TF frames like odom and base_link should be configured, and how the package uses an Extended
  Kalman Filter to combine noisy measurements into a more reliable pose estimate. The article also
  walks through a Husky simulation setup in Gazebo and shows the expected filtered odometry result.
---

External article on Medium.