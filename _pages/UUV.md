---
layout: single
permalink: /UUV/
author_profile: true
classes: wide
title: Unmanned Underwater Vehicle (UUV)

toc: true
toc_label: "Table of Contents"
---

# Introduction
VantTec's UUV is a project at Tecnológico de Monterrey. After a long stay in Germany, I came back to Mexico and took over the UUV, which faced significant challenges, including my lack of familiarity with underwater robotics. After a year of team effort of more than 16 undergraduate students, the UUV became a reality and is ready to continue the legacy of previous generations. This are the first results entirely done by my administration: 

<figure class="third">
  <a href="/assets/images/uuv_1.jpeg">
  <img src="/assets/images/uuv_1.jpeg"></a>

  <a href="/assets/images/uuv.jpeg">
  <img src="/assets/images/uuv.jpeg"></a>

  <a href="/assets/images/uuv_test.gif">
  <img src="/assets/images/uuv_test.gif"></a>

  <a href="/assets/images/uuv_cfd.jpeg">
  <img src="/assets/images/uuv_cfd.jpeg"></a>

  <a href="/assets/images/uuv_simulated.jpeg">
  <img src="/assets/images/uuv_simulated.jpeg"></a>

  <a href="/assets/images/uuv_equipo.jpeg">
  <img src="/assets/images/uuv_equipo.jpeg"></a>

</figure>

# Localization
The UUV aims to contain th next localization scheme.
![image-center](/assets/images/localization_scheme.png){: .align-center}

At the moment the UUV contains only an IMU, a hydrophone and a ZED2i, i.e., an incomplete localization scheme. Therefore, the decision to develop algorithms with a stronger emphasis on the camera were being reviewed, e.g., NeRF-SLAM, 3d Gaussian Splats, color enhancement for underwater applications.

## Working on:
- Underwater backscatter removal and color enhancing and reviewing for real-time methods.
- Optical flow for obtaining linear velocities aimed for underwater SLAM.

# Vision
At the moment, we are working with synthetic data, i.e., rendered images with annotations, to feed object detection models. This is done using a pipeline with diffusion models. Given that we want the image to be already annotated, we are using ControlNet neural network architecture. The result is shown next.

![image-center](/assets/images/synthetic_overview.jpeg){: .align-center}

## Working on: 
- Targeted for IROS2025: synthetic data generation for underwater applications. A novel approach introducing actual physical coefficients to condition diffusion models.