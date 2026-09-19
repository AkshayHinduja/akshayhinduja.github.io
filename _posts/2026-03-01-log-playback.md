---
title   : "3D dive log playback"
org     : "MBARI"
role    : "Software Engineer"
period  : "2024 – present"
videourl : "/assets/video/tethystales.mp4"
posterurl: "/assets/images/tethystales-poster.jpg"
teaserurl:            # not used while videourl is set
imurl   :             # not used while videourl is set
desc    : "Open-source, containerized ROS 2 and RViz tooling that replays vehicle dive logs as a 3D reconstruction of the navigation, vehicle state and science data."
linkurl : "https://hub.docker.com/r/mbari/tethystales"
linklabel: "Docker Hub"
categories: Project
---

## Overview
Dive logs hold everything a vehicle recorded, but a raw log is hard to reason about after the fact. Engineers and scientists want to see what the vehicle did, not read a table of it.

I wrote ROS 2 and RViz Docker images that ingest vehicle logs and play them back as a 3D representation of the navigation during a dive. The containers keep the playback environment reproducible across machines.

The playback also shows readouts of vehicle state data and science readings alongside the 3D view, so a track can be read together with the measurements taken along it.

The tool is open source. The images are published on Docker Hub as [mbari/tethystales](https://hub.docker.com/r/mbari/tethystales).

## Tools
ROS 2, RViz, Docker.
