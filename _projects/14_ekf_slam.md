---
layout: post
title: FSD EKF SLAM
permalink: /projects/fsd-ekf-slam
excerpt: |
  Implementation of EKF SLAM algorithm for Formula Student Driverless car
  <center><img width="600" src="/pics/14_ekf_slam/ekf_slam_demo.gif"></center>
  <br>
date: 2020-01-10
order_number: 3
---
{% include button.html text="Github repository" icon="github" link="https://github.com/macstepien/fsd_ekf_slam" color="#0366d6" %}

EKF SLAM that I implemented during my work on Formula Student Driverless car. I used C++ and Eigen for matrix operations. It also includes a simple cone detector, which processes Lidar data with PCL and calculates the position of a cone. Detected cones are later used as observations for EKF SLAM. The whole thing was implemented as a ROS Node.

{% include video.html id="TMYYV3xASdM" title="EKF SLAM demo" %}
