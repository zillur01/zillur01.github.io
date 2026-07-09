---
layout: page
title: HD Maps for Autonomous Driving
description: SLAM map and Semantic map of the ODD
img: assets/img/projects/slam_map_gif.gif
importance: 2
category: Research
---



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/projects/slam_map_gif.gif" title="SLAM Map" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/projects/semantic_map.png" title="Semantic Map" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

High-definition (HD) maps play a pivotal role in enabling autonomous cars to navigate and operate safely. These intricate maps provide detailed and precise information about roadways, traffic signs, lane markings, intersections, and other critical features. By integrating real-time data from various sensors with static information from HD maps, self-driving vehicles can make informed decisions, plan routes, and navigate complex environments with enhanced accuracy and reliability. HD maps are a fundamental component in the quest for safer and more efficient autonomous driving solutions.

Our HD map consists of two maps. The first one is a SLAM map which creates a 3D environment from LiDAR and IMU data. For our project, we have used an Ouster OS2-128 LiDAR and a 6-axis IMU. We implemented Fast-LIO and LIO-SAM models. Both of them worked successfully but we chose a modified version of LIO-SAM, also known as liorf. It generated an effective SLAM map by keeping the size relatively small.

SLAM model: [https://github.com/zillur01/liorf](https://github.com/zillur01/liorf)

The second map of our project is a Lanelet2 map. This map provides lane marking information, road width, traffic signs, traffic signals location etc. Combined with the SLAM map, we now have everything we need. We are using Tier4 lanelet2 map tool box to create the map.


