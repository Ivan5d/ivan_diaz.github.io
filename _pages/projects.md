---
layout: single
permalink: /projects/
title: "Projects"
classes: wide
header: 
  overlay_image: /assets/images/horcones.jpeg
  caption: "Photo location: La Huasteca natural park in Monterrey, Nuevo Leon, Mexico"
author_profile: true
excerpt: Here is a list of the projects that I've been working on, as well as the links to the publicly available source codes. 
---

### Computer Vision
[Synthetic Data Generation](https://github.com/vanttec/vanttec_synthdata): Procedural pipeline implementation for synthetic image renderization to feed segmentation and object detection models used within autonomous vehicles. This is an upgrade to my work at Evocortex GmbH.

[Explainable AI for Synthetic Data Generation](https://github.com/Ivan5d/AI_Synthdata): Implementation of XAI methods for visualizing the object detection flaws, with a focus on improving the synthetic data generation strategy. This is an upgrade to my work at Evocortex GmbH.

Image classification for glaucoma (eyes disease): image classfication using a 1) image segmentation and 2) image classificator for glaucoma diagnosis. Project for the [Hospital de la Ceguera](https://apec.org.mx/)

## Underwater Autonomous Vehicle (UUV)
[UUV's Repository and Gazebo Simulation](https://github.com/vanttec/vanttec_uuv): The repo is based on the Robotic Operating System (ROS), but student generations has passed and the repo is broken on different ROS, Python versions and branches. At the moment, I'm trying to solve all the issues for an integration. In addition, the gazebo implementation for testing underwater robot's sensors and algorithms is based on ROS melodic and it's missing key sensors such as the sonar, so I'm trying to update that.

## Next projects
**Real-time image color correction for underwater applications:** The UUV can't rely more on the camera for path planning, given that there exist attenuation coefficients occuring on the water. In addition, the image correction models requires a couple of seconds for a single image to correct.