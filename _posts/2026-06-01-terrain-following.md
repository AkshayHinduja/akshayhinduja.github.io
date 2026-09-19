---
title   : "Terrain avoidance and following for AUVs"
org     : "MBARI"
role    : "Software Engineer"
period  : "2024 – present"
teaserurl: "/assets/images/terrain-avoidance-sim-teaser.webp"
imurl   : "/assets/images/terrain-avoidance-sim.webp"
desc    : "Altitude control and obstacle avoidance for autonomous underwater vehicles, driven by profiling imaging sonar and DVL input."
categories: Project
---

## Overview
An autonomous underwater vehicle (AUV) has to hold a useful altitude above the seafloor while the terrain under it changes. Flying too high costs data quality. Flying too low risks a collision.

I wrote algorithms that take profiling imaging sonar returns and Doppler velocity log (DVL) input and use them to maintain altitude. The sonar supplies the shape of the seafloor ahead of the vehicle. The DVL supplies the altitude and velocity reference.

The algorithms build a forward-looking horizon model from those returns. The vehicle uses that model to correct for impending obstacles before it reaches them, rather than reacting only to what is directly below.

The screenshot above is from the Gazebo simulation used to develop the module. On the right, the vehicle flies over terrain with its sonar fan and DVL beams drawn. On the left, the module's log shows it switching from cruise to correction as the altitude drops, then resuming cruise once the terrain falls away.

## Tools
Profiling imaging sonar, Doppler velocity log (DVL), forward-looking horizon modeling.
