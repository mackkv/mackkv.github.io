---
permalink: /
title: "Kevin Mack: PhD Student, Research Assistant"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I'm a graduate student and research assisstant in the <a href="https://sites.google.com/clarkson.edu/cu-cosine-lab/home">CoSiNe Lab</a> at Clarkson University. My focus is on various topics in Machine Learning, Signal Processing, and Communications. I have also worked on engineering education projects, with a focus on creating and using mobile apps as tools for learning and education outreach.  

This site is still a work in progress, and is being updated incrimentally to include projects that I have worked on, and works that can be found publicly.


Some quick examples of my interests and work
======
Some of my most recent work with underwater LiDAR. The project uses a time-of-flight (ToF) camera, which has been modified to perform optical sensing and object detection in the underwater environment. This technology has the potential to be highly useful for situational awareness, due to its inherent high framerate sensing and it's ability to determine absolute size of the object in question. The general principle behind ToF technology is given by the figure below.
![tof_basics](files/TOF_BASICS.png)

The underwater environment poses a challenge for underwater optical sensing, due to the high amounts of signal scattering and absorption (see figure below).
![tof_uw](files/TOF_UWScatter.png)

The stock ToF camera needs to be modified to fit the underwater application. This is done by using the camera's pulsed CW signal to drive a 525nm 1 Watt laser diode. Some of the circuit board revisions, as well as photos of the field testing apparatus that was developed by undergraduate students at <a href="http://www.gcc.edu/">Grove City College</a> are given in the figure below.
![tof_hardware](files/UWTOF_HARDWARE.png)

Here is a GUI made with PyQt used for viewing data from a time-of-flight (ToF) camera. The app receives data over tcp connection, and displays in the GUI. This project can be found <a href="https://github.com/mackkv/CaptureGUI">here.</a>
![gui](files/gui_gif.gif)

The setups for two specific exepriments are given in the figure below,
![experiments](files/UWTOF_Experiments.png)

and the results for close range experiments are given in the form of range images.
![exp_results_close](files/UWTOF_CLOSE_TVL1.png)

The above results are obtained from treating the data with a digital filter to remove the camera's inherent noise, then the scatter is treated with a primal dual algorithm that solves the $L_1$ total variation (TV) regularization image reconstruction problem. The details are published <a href="https://mackkv.github.io/publications/SPIE21_Conference">here.</a>

Personal and Course Projects
======
### Signal and Image Processing
Output from a semantic segmentation neural network. The colors represent segments of the image that belong to certain class of objects. The .gif shows the raw input data, the pixel classification, and the overlay for two slightly different settings. The network was trained on the <a href="https://www.cityscapes-dataset.com/">cityscapes dataset</a>, and was an implementation of known neural network structures that work well for this problem. The test data was recorded from my own dashcam. This work served as my project for my Neuromorphic Computing course.
![dashcam](files/potsdam_dashcam.gif)

#### Image Restoration and Underwater ToF Simulation
![wr3d_imgs](files/simulation_images_T6.png)
### Automation
#### HomeAssistant Project
![HomeAssistant](files/Auto-Garden-GUI-cropped.png)

#### Underwater LiDAR Test Tank
![tacTankMatlab](files/matlab_gui_1.png)
![tacTankMatlab_1](files/matlab_gui_2.png)
