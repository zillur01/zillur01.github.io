---
layout: page
title: UNLV Autonomous Driving
description: Deploy a full autonomous driving software stack on a real car equipped with necessary hardware.
img: assets/img/projects/unlv_car_gif.gif
importance: 1
category: Research
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/projects/unlv_car_gif.gif" title="Autonomous Driving" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/projects/unlv_car.jpg" title="UNLV Autonomous Car" class="img-fluid rounded z-depth-1" %}
    </div>
</div>



UNLV Autonomous Vehicle: Our dedicated team has been deeply involved in advancing autonomous vehicle technology. I have had the privilege of leading a group of highly motivated graduate and undergraduate students in this endeavor. After over a year of dedicated effort, we are now witnessing promising results. We have successfully implemented self-driving technology on our university campus, utilizing a customized Lincoln MKZ equipped with an array of sensors, including 4 LiDARS, 5 RADARS, SONAR, 4 Lucid vision cameras, a thermal camera, IMU, GPS, and drive-by-wire technology. As for our software stack, we've tailored open-source Autoware Universe to accommodate our sensor suite, enabling the vehicle to operate autonomously within its Operational Design Domain (ODD). Our self-driving car rigorously adheres to all traffic regulations, including stop signs, traffic lights, right-of-way, parking, and more.

Here is the summary of how we implemented the software stack:
- Calibrated the sensors: get extrinsic and intrinsic parameters of LiDARS, cameras, etc learn more
- Created HD map of the ODD: 3D SLAM map for localization and lanelet2 map for route networks and traffic rules. learn more
- Interfacing: Converted actuator CAN messages like current velocity, steering angle, gear status, etc from the vehicle to Autoware-like format. Then converted the control commands generated from the autoware to CAN messages. 

code: [https://github.com/zillur-av/mkz_interface](https://github.com/zillur-av/mkz_interface)

[https://bitbucket.org/DataspeedInc/dbw_ros/src/ros2/](https://bitbucket.org/DataspeedInc/dbw_ros/src/ros2/)

I have made many changes to the interfacing module. If you need the exact code, please contact me. We are using the Lincoln MKZ 2017 hybrid model with dataspeed by-wire CAN systems. The by-wire system was installed by AutonomousStuff.
Besides those major modifications, we needed to modify some programs related to the Ouster lidar message and IMU messages. Autoware Universe software stack works on top of ROS2 humble version. 

github link: [https://github.com/zillur-av/autoware](https://github.com/zillur-av/autoware)


