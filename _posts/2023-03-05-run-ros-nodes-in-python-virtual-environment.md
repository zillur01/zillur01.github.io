---
layout: post
title: Run ROS Nodes in Python Virtual Environment
date: 2023-03-05
description: In this article, I described how to use ROS Python Nodes in a virtual environment using proper interpreters.
redirect: https://medium.com/@zillur-rahman/run-ros-nodes-in-python-virtual-environment-3ea5455cc81
external_source: Medium
tags: [ROS, Python, Robotics]
categories: [Robotics]
feed_content: >
  Python virtual environments are essential when robotics projects need isolated dependencies,
  but ROS nodes often fail when the wrong interpreter is used. This article explains two practical
  ways to run ROS Python nodes with the correct interpreter: using a direct shebang that points to
  the virtual environment, and using catkin_make with an explicit PYTHON_EXECUTABLE. It also covers
  the extra packages needed inside the environment so ROS can run correctly.
---

External article on Medium.