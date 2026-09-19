---
title   : "Localization in GPS-denied environments with bathymetric submaps"
org     : "MBARI"
role    : "Software Engineer"
period  : "2024 – present"
teaserurl: "/assets/images/submap-localization-process.webp"
imurl   : "/assets/images/submap-localization-process.webp"
desc    : "Submap-based localization for autonomous underwater vehicles in low-altitude surveys, fusing particle filter updates with a pose graph to produce geo-localized 3D maps."
categories: Project
---

## Overview
An autonomous underwater vehicle (AUV) cannot use GPS underwater, and acoustic positioning is not always available either. In low-altitude surveys the ultra-short baseline (USBL) lock can drop out, which leaves the vehicle without an absolute position reference.

I used Stochastic Variational Gaussian Processes to localize AUVs against bathymetric submaps and prior surveys when USBL lock is unavailable. The seafloor itself becomes the reference.

I also developed a fusion system that ties particle filter updates to a pose graph. This lets submap-based loop closures enter the same estimate as the vehicle's dead-reckoned navigation, and produces accurate, geo-localized 3D maps and trajectory estimates.

## Tools
Stochastic Variational Gaussian Processes, particle filtering, pose graph optimization, bathymetric submaps.
