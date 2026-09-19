---
title   : "Wideband echosounder drivers for ROVs"
org     : "MBARI"
role    : "Software Engineer"
period  : "2024 – present"
teaserurl:            # add image later
imurl   :             # add image later
desc    : "Python and C++ drivers for wideband echosounders on MBARI's remotely operated vehicles, with visual and CLI tools for low-bandwidth links."
categories: Project
---

## Overview
MBARI's remotely operated vehicles carry wideband echosounders for acoustic sensing in the water column. The instruments need software that can configure them and pull their returns back to the operator.

I wrote Python and C++ drivers to interface with those echosounders. The drivers expose the instrument parameters and the return data to the rest of the vehicle software.

I also wrote visual and CLI tools on top of the drivers. Operators use them to change parameters and visualize returns over low-bandwidth, sparse wireless communication links, where the tooling has to stay usable when data arrives slowly and in gaps.

## Tools
Python, C++, command-line tooling, wideband echosounders.
