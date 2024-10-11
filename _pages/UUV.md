---
layout: single
permalink: /UUV/
author_profile: true
classes: wide
title: Unmanned Underwater Vehicle (UUV)

toc: true
toc_label: "Table of Contents"


feature_row:
  - image_path: /assets/images/uuv_1.jpeg
    title: "UUV"
    excerpt: "The first manufactured prototype from Vanttec."
  - image_path: /assets/images/uuv_cfd.jpeg
    title: "Computational Fluid Dynamics (CFD)"
    excerpt: "CFD analysis was followed to detect water vortex that could affect the UUV."
  - image_path: /assets/images/uuv_test.gif
    title: "First test"
    excerpt: "The first UUV test with stable flotation and teleoperated movement."


---

# Introduction
VantTec's UUV is a project at Tecnológico de Monterrey. After a long stay in Germany, I came back to Mexico and took over the UUV, which faced significant challenges, including my lack of familiarity with underwater robotics. After a year of team effort of more than 16 undergraduate students, the UUV became a reality and is ready to continue the legacy of previous generations. This are the first results entirely done by my administration: 

{% include feature_row id="feature_row" %}

# Software/Localization
The UUV is based on ROS Noetic and it is aimed to contain the next localization scheme.
![image-center](/assets/images/localization_scheme.png){: .align-center}

## Contribution
There are missing sensors that make impossible to work on a localization scheme. For this reason, we are working at the moment to supply the missing sensores with a camera, specifically aiming an underwater backscatter removal and image color enhancing, as well as optical flow in the underwater application.

# Vision
At the moment, we are working with synthetic data, i.e., rendered images, to feed object detector models. This is done using a pipeline with diffusion models. Given that we want the image to be already annotated, then we are using ControlNet neural network architecture. The result is shown next.

![image-center](/assets/images/synthetic_overview.jpeg){: .align-center}

## Contribution
At the moment we are conditionining the diffusion process to incorporate the actual coefficients of the underwater image formation model, i.e., attenuation coefficients.