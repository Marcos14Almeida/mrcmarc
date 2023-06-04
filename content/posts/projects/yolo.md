---
title: "Detecting license plates and pedestrians using YOLO"
date: 2020-12-10T20:08:28-03:00
description: Undergraduate thesis
hero: /images/projects/yolo.png
theme: Toha
menu:
  sidebar:
    name: 20-Undergraduate thesis - YOLO
    identifier: yolo
    parent: projects
    weight: 500
---


**Development**

Start: 08/2020.

End: 12/2020.


**Project description**

YOLO (You Only Look Once) is a real-time object detection algorithm that can detect and identify objects in images and videos. It works by dividing an image into a grid of cells and predicting the object class and bounding box for each cell, using a single convolutional neural network. YOLO is known for its speed and accuracy, making it popular for various computer vision applications such as self-driving cars, surveillance, and robotics.

My undergraduate thesis consisted of detecting license plates for cars and pedestrians and comparing the performance of versions 3.0 tiny, 4.0 and 4.0 tiny. The code was developed using google colab to use some source of GPU. The train dataset was collected by a PhD student, but I used random street photos under different conditions to test the results. The results can be seen in the images below. I also recorded videos with YOLO performing in real-time.

**Screenshot**

<div style="display: flex; flex-direction: column;  align-items: center;">
  
  <img src="/posts/projects/images/yolo/yolo 1.png" alt="Image 1" style="width: 60%; margin: 10px;">
    <figcaption>Comparison YOLO versions for license plates</figcaption>
<br>
  <img src="/posts/projects/images/yolo/yolo 2.png" alt="Image 2" style="width: 60%; margin: 10px;">
    <figcaption>Comparison YOLO versions for license plates and pedestrians</figcaption>
<br>
  <img src="/posts/projects/images/yolo/yolo 3.png" alt="Image 3" style="width: 60%; margin: 10px;">
    <figcaption>Comparison YOLO versions for license plates and pedestrians</figcaption>
<br>

</div>


**Tools**
- Neural Networks
- YOLO
- Google Colab
