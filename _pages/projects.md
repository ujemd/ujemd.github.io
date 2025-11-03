---
permalink: /projects/
title: "Projects"
excerpt: " "
layout: single
hhi_gallery:
  - url: ../hhi/tokenization.gif
    image_path: ../hhi/tokenization.gif
    alt: "Tokenization results"
  - url: ../hhi/walk.gif
  - image_path: ../hhi/walk.gif
  - alt: "Synthesis from limited data"
mst_gallery:
  - url: ../mst/mst_1.gif
    image_path: ../mst/mst_1.gif
    alt: "Mean Shift 1"
  - url: ../mst/mst_2.gif
    image_path: ../mst/mst_2.gif
    alt: "Mean Shift 2"
  - url: ../mst/mst_4.gif
    image_path: ../mst/mst_4.gif
    alt: "Mean Shift 3"
dist_gallery:
  - url: ../nss/AWN.png
    image_path: ../nss/AWN.png
    alt: "Additive white noise"
  - url: ../nss/JPEG.png
    image_path: ../nss/JPEG.png
    alt: "JPEG distortion"
  - url: ../nss/NU.png
    image_path: ../nss/NU.png
    alt: "Non uniformity distortion"
  - url: ../nss/blur.png
    image_path: ../nss/blur.png
    alt: "Blur"
vmmc_gallery:
  - url: ../vmmc/scene.jpg
    image_path: ../vmmc/scene.jpg
    alt: "Scene"
  - url: ../vmmc/vmmc.gif
    image_path: ../vmmc/vmmc.gif
    alt: "Point cloud"
nss_gallery:
  - url: ../nss/distortionFeatures.png
    image_path: ../nss/distortionFeatures.png
    alt: "Distortion features"
  - url: ../nss/SVM-scatter.png
    image_path: ../nss/SVM-scatter.png
    alt: "SVM results"
complex_gallery:
  - url: https://raw.githubusercontent.com/ujemd/ComplexAnalysis/master/img/r.5.gif
    image_path: https://raw.githubusercontent.com/ujemd/ComplexAnalysis/master/img/r.5.gif
    alt: "r.5"
  - url: https://raw.githubusercontent.com/ujemd/ComplexAnalysis/master/img/r.75.gif
    image_path: https://raw.githubusercontent.com/ujemd/ComplexAnalysis/master/img/r.75.gif
    alt: "r.75"
  - url: https://raw.githubusercontent.com/ujemd/ComplexAnalysis/master/img/r1.25.gif
    image_path: https://raw.githubusercontent.com/ujemd/ComplexAnalysis/master/img/r1.25.gif
    alt: "r1.25"
  - url: https://raw.githubusercontent.com/ujemd/ComplexAnalysis/master/img/r1.gif
    image_path: https://raw.githubusercontent.com/ujemd/ComplexAnalysis/master/img/r1.gif
    alt: "r1"
toc: true
---

## Human Motion Synthesis

Showcase of some of the results of my work in Human Motion Synthesis.

By training a sequence of generative adversarial networks (GANs), we generate new motion from limited training data, and even combine different types of motion. Here's an example of a walking motion that's completely generated.

![cvmp](../hhi/walk.gif){:height="85%" width="85%"}

## Augmented and Virtual Reality

### Head-coupled Perspective

A fun project where we created a window to a virtual 3D world :-) The algorithm works by detecting the user's face and estimating its 3D position with respect to a camera. With this information, the program is able to simulate a head-coupled perspective. This application is mainly based in this [article](https://medium.com/@michel.brisis/off-axis-projection-in-unity-1572d826541e), and our repository can be found [here](https://github.com/ujemd/off-axis-projection-unity).

![hc-pers](https://raw.githubusercontent.com/ujemd/off-axis-projection-unity/master/img/head-coupled-perspective.gif){:height="85%" width="85%"}

## Video Analysis

### Mean Shift Tracking with Corrected Background

Simple mean shift tracking implementation which uses background information, based on the paper _Robust mean-shift tracking with corrected
background-weighted histogram_ by Ning et al. It attempts to reduce the interference of background information in kernel-based tracking. Please refer to the [repository](https://github.com/ujemd/MeanShiftTracking-CBWH) for the C++ code.

{% include gallery id="mst_gallery" caption="Examples of mean shift tracking." %}

### Abandoned Object Detection

Classification of stationary objects into abandoned or stolen, based on the paper _Robust unattended and stolen object detection by fusing simple algorithms_ by San Miguel and Martinez ([reference](https://ieeexplore.ieee.org/document/4730375)).

![abandoned](../mst/abandoned.gif){:height="85%" width="85%"}

## Tomography and 3D Imaging

### 3D Image Reconstruction

Reconstruction of a mouse volume using filtered backprojection. The Matlab implementation can be found in the [repository](https://github.com/ujemd/3DFilteredBackProjection).

![mouse](../tibs/mouse.gif){:height="50%" width="50%"}

## Vision for Multiple/Moving Cameras

### 3D Reconstruction

Reconstruction of a scene by extracting and matching interest points. The points were detected using the KAZE detector, and
their features are provided by the DSP-SIFT descriptor. The reconstruction process consists of extracting the fundamental matrix, applying projective bundle adjustment and finally obtaining an Euclidean reconstruction.

{% include gallery id="vmmc_gallery" caption="Scene and its point cloud." %}

## Natural Scene Statistics of Fused Long Wave Infrared and Visible Light Images

This is an image processing piece about quality assessment, which can be found puclicly in IEEE Transactions on Image Processing: ["Predicting the Quality of Fused Long Wave Infrared and Visible Light Images"](http://ieeexplore.ieee.org/document/7904687/), David-Moreno D.E., Benítez-Restrepo H.D., Bovik A.C. This work proposes fused image quality metrics and presents a subjective human study for their construction and validation. Please refer to the [repository](https://github.com/ujemd/NSS-of-LWIR-and-Vissible-Images) for more details about the implementation.

{% include gallery id="dist_gallery" caption="Examples of distortions (Gaussian, JPEG compression, Non-uniformity, blur) occurring to fused LWIR-visible light images." %}

{% include gallery id="nss_gallery" caption="Scatter plot of features extracted from distorted images / Scatter plot for our metric prediction scores vs subjective scores." %}

## Complex Analysis

### Tinkering with Julia and Mandelbrot sets

Visualisation of the filled-in Julia set and the Mandelbrot set. A simple implementation provided in C# can be found in [here](https://github.com/ujemd/ComplexAnalysis).

{% include gallery id="complex_gallery" caption="Representations of the filled-in Julia set." %}
