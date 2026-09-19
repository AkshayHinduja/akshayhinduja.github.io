---
title   : "Deployable AI"
org     : "MBARI"
role    : "Software Engineer"
period  : "2024 – present"
teaserurl: "/assets/images/deployable-ai-triton.jpg"
imurl   : "/assets/images/deployable-ai-triton.jpg"
imcredit: "NOAA"
desc    : "On-vehicle perception for MBARI's autonomous underwater vehicles: multicamera drivers for edge computers, embedded machine learning for tasks such as tracking marine animals, and the link that lets perception drive vehicle behavior."
categories: Project
---

## Overview
Deployable AI puts perception on the vehicle. Ocean vehicles carry limited compute and limited bandwidth, so the camera system and the models that read it have to run at the sensor, not on shore. The photo shows the multicamera system on the nose of the AUV. I develop the software that runs it.

My contributions cover the camera drivers, the embedded vision and machine learning stack, and the interface that lets the results change what the vehicle does.

## Multicamera drivers for edge computers
Multicamera rigs on edge computers have to move a lot of pixels without dropping frames. A single-threaded capture path cannot keep up at high resolution and high frame rate.

I wrote custom drivers for these multicamera systems using multithreading. Capture, streaming and recording run in parallel so the pipeline keeps pace with the sensors. The drivers support 2K at 60 fps and handle both synchronous and asynchronous streaming and recording, so the cameras can run together as a rig or independently.

## Embedded AI and vision
I write Python code that interfaces with the optical sensors and feeds their streams into computer vision tasks, such as tracking marine animals as they pass the camera.

I also develop and refine machine learning models for on-device processing on embedded systems, where each model has to fit the available hardware budget.

## Reactive vehicle behaviors
The perception stack runs on the backseat computer. I interface it with the frontseat vehicle commands, so what the cameras see can drive reactive vehicle behaviors during a mission.

## Tools
Python, custom driver development, multithreading, machine learning models for on-device inference, embedded edge computers, multicamera systems.
