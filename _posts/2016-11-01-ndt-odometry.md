---
title   : "3D point cloud NDT odometry"
org     : "Carnegie Mellon University"
role    : "Computer Vision course project"
period  : "Fall 2016"
teaserurl:            # add image later
imurl   :             # add image later
desc    : "A ROS odometry package for a Velodyne VLP-16, using the Normal Distributions Transform for scan matching."
categories: Project
---

## Overview
Odometry from a lidar comes down to registering one scan against the next. The registration method decides how well it holds up.

For this Computer Vision course project I developed an odometry package in ROS using a Velodyne VLP-16. The algorithm uses the Normal Distributions Transform for scan matching between 3D point clouds.

The work followed on from a robotics internship at Tsuneishi Shipbuilding in Fukuyama, Japan, from May to June 2016, where I implemented ICP and NDT-based localization with the same VLP-16 sensor.

## Tools
ROS, Velodyne VLP-16, Normal Distributions Transform, 3D point clouds.
