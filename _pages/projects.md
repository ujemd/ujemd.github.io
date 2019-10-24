---
permalink: /projects/
title: "Projects"
excerpt: " "
layout: single
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
    alt: "Blurring"
toc: true
---

## Video Analysis

### Mean Shift Tracking with Corrected Background

Simple mean shift tracking implementation which uses background information, based on the paper _Robust mean-shift tracking with corrected
background-weighted histogram_ by Ning et al. It attempts to reduce the interference of background information in kernel-based tracking. Please refer to the ![repository.](https://github.com/ujemd/MeanShiftTracking-CBWH) for the C++ code.

{% include gallery id="mst_gallery" caption="Examples of mean shift tracking." %}

### Abandoned Object Detection

Classification of stationary objects into abandoned or stolen, based on the paper _Robust unattended and stolen object detection by fusing simple algorithms_ by San Miguel and Martinez (![Reference](https://ieeexplore.ieee.org/document/4730375)). 

![abandoned](../mst/abandoned.gif){:height="85%" width="85%"}

## Tomography and 3D Imaging

### 3D Image Reconstruction

Reconstruction of a mouse volume using filtered backprojection. The Matlab implementation can be found in the ![repository.](https://github.com/ujemd/3DFilteredBackProjection)

![mouse](../tibs/mouse.gif){:height="50%" width="50%"}

## Natural Scene Statistics of Fused Long Wave Infrared and Visible Light Images

This is an image processing piece about quality assessment, which can be found puclicly in IEEE Transactions on Image Processing: ["Predicting the Quality of Fused Long Wave Infrared and Visible Light Images"](http://ieeexplore.ieee.org/document/7904687/), David-Moreno D.E., Benítez-Restrepo H.D., Bovik A.C. This work proposes fused image quality metrics and presents a subjective human study for their construction and validation. Please refer to the ![repository](https://github.com/ujemd/NSS-of-LWIR-and-Vissible-Images) for more details about the implementation.

{% include gallery id="dist_gallery" caption="Examples of distortions occurring to fused LWIR-visible light images." %}

