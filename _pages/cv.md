---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* Bachelor of Science in Electrical Engineering, Johns Hopkins University, Aug 2021 - June 2025
* Bachelor of Science in Neuroscience, Johns Hopkins University, Aug 2021 - June 2025
* GPA: 3.82

Research experience
======
* **Neuroengineering & Biomedical Instrumentation Laboratory, Nitish V. Thakor**
<br>The Johns Hopkins University, Aug 2021 – present
  * 3D Visual Feedback System for Myoelectric Motor Training:
    * Developed a Python-based 3D visual feedback system using Linear Discriminant Analysis to enhance control accuracy in myoelectric motor training.
    * Conducted 200+ EMG-based Fitts Law clinical trials on healthy and amputee subjects to assess 3D visual feedback’s impact on prosthesis control.
    * Demonstrated improved pattern recognition control performance in naive operators, enhancing adaptability to complex tasks through motor-based training.
  * Implantable System Wavelet Compression:
    * Developing an implantable system using wavelet compression to minimize motor unit transmission size.
    * Engineered motor unit separation algorithms to isolate motor units and filter out signal contamination.
    * Designing and manufacturing an all-in-one micro recorder, simulator, and wirelessly charged implantable hardware system for rat implant studies.
    * Performing 10+ RPNI and VDMT reinnervation surgeries on rats to study the effects of implantable systems on retaining motor unit information.

* **Neuroplasticity & Repair Laboratory, Daniel C. Lu**
<br>University of California Los Angeles, Oct 2022 – Jun 2024
  * Led the development of a comprehensive MATLAB pipeline with a multidisciplinary team to detect and analyze EMG properties in spinal cord injury patients before and after neuromodulation.
  * Pioneered a PCA-based model to detect abnormalities in breathing and gait cycles in spinal cord injury patients, effectively filtering out contaminated trials from the analysis.
  * Designed a filtering algorithm utilizing adaptive template subtraction to remove ECG artifacts and baseline noise from raw EMG signals.
  * Innovatively cross-correlated lung airway pressure with EMG rolling standard deviation to pinpoint activation regions in respiratory muscles.
  * Developed an automated system for detecting evoked potentials in lower limb muscles.

* **Laboratory of Mechanical System and Vibration, Xiangyang Zhu**
<br>Shanghai Jiao Tong University, Jun 2023 – Sep 2023
  * Developed an offline system using the Support Vector Machine algorithm for ultrasound, mechanomyography, and Near-Infrared Spectroscopy (NIRS) signals.
  * Conducted tests on EMG-NIRS feature fusion, demonstrating an improvement in offline classification accuracy from 81% to 90%.
  * Developed an embedded C framework to facilitate command transfer from a PC to the myoelectric prosthetic arm’s microcontroller.

* **Institute for Artificial Intelligence, Qining Wang**
<br>Peking University, Jan 2019 – May 2021
  * Co-developed an adaptive algorithm for real-time Maximum Dorsiflexion timing detection in robotic transtibial prostheses, improving control across varying speeds and ramp conditions with 100% accuracy.
  * Collected gait data on three amputees at Peking University and EMG + EEG data of biathlon athletes at Dalian Paralympic Training Center.
  * Created muscle training guide for 40+ biathlon athletes.

Publications
======
<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>

Skills
======
* Coding: Matlab, Python, C, C++，LDA, SVM, K-means, CNN
* Electrical Engineering: PCB Design, KiCad, Arduino, Microprocessors, Signal Systems, Microfabrication
* Biology: EMG/EEG Recording and Analyzing, Motor Unit Spike Sorting, Amputee Clinical Trials, Rat Handling, RPNI/VDMT surgeries

Relevant Coursework
======
* Bioelectricity from Neurons to Semiconductors
* Signals and Systems
* Computational Neuroscience
* Microfabrication Laboratory

Research Interests
======
* Neural Interfaces and Neuroprosthetics
* EMG/EEG Pattern Recognition and Signal Processing
* Spinal Cord Injury Rehabilitation
* Motor Unit Signal Compression and Reconstruction
* Multimodal Sensory Feedback in Neuroprosthetics

Academic Reference
======
* Nitish V. Thakor, PhD (Email: nthakor@bme.jhu.edu)
* Ruyi Huang, PhD (Email: ruyihuang@mednet.ucla.edu)
* Jason Trageser, PhD (Email: jtrages3@jhu.edu)
