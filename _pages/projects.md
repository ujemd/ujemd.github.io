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
  - url: ../mst/mst_3.gif
    image_path: ../mst/mst_3.gif
    alt: "Mean Shift 3"
toc: true
---

## Video Analysis

### Mean Shift Tracking with Corrected Background

Simple mean shift based tracking using background information, based on the paper _Robust mean-shift tracking with corrected
background-weighted histogram_ by Ning et al. ![Repository.](https://github.com/ujemd/MeanShiftTracking-CBWH)

{% include gallery id="mst_gallery" caption="Examples of mean shift tracking." %}

![ball](../mst/mst_1.gif){:height="40%" width="40%"} ![basketball](../mst/mst_2.gif){:height="40%" width="40%"} ![road](../mst/mst_4.gif){:height="40%" width="40%"}

### Abandoned Object Detection

Classification of stationary objects into abandoned or stolen, based on the paper _Robust unattended and stolen object detection by fusing simple algorithms_ by San Miguel and Martinez (![Reference](https://ieeexplore.ieee.org/document/4730375)). 

![abandoned](../mst/abandoned.gif){:height="85%" width="85%"}

## Tomography and 3D Imaging

### 3D Image Reconstruction

Reconstruction of a mouse volume using filtered backprojection. ![Repository.](https://github.com/ujemd/3DFilteredBackProjection)

![mouse](../tibs/mouse.gif){:height="50%" width="50%"}

## Natural Scene Statistics of Fused Long Wave Infrared and Visible Light Images

Small demonstration of the work presented in:

["Predicting the Quality of Fused Long Wave Infrared and Visible Light Images"](http://ieeexplore.ieee.org/document/7904687/), David-Moreno D.E., Benítez-Restrepo H.D., Bovik A.C.

Which proposes fused image quality metrics and presents a subjective human study for their construction and validation. Files included are: the Matlab implementation of an *opinion distortion unaware* and an *opinion aware fused image quality analyzer*, the original raw opinion scores, Z-scores after subject rejection, and Differential Mean Opinion Scores (DMOS). Please refer to the ![repository](https://github.com/ujemd/NSS-of-LWIR-and-Vissible-Images).

![morrisgra](../nss/MorrisGra.png)

*Fused LWIR-visible light image*

