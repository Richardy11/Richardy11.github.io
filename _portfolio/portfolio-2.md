---
title: "Processing and Evaluation Pipeline for Neuromodulation of Respiratory Muscles"
excerpt: "Respiratory complications are a leading cause of death in patients with chronic spinal cord injury (SCI), significantly impacting their quality of life. **Neuromodulation**, a promising therapeutic approach, involves electrical stimulation to modulate nerve activity and enhance respiratory function. To support this effort, a comprehensive MATLAB pipeline was developed to **automatically detect, analyze, and compare electromyography (EMG) properties** in SCI patients undergoing neuromodulation therapy, contributing to the development of improved diagnostic and therapeutic strategies aimed at alleviating respiratory complications in this population. <br/><img src='/images/Pipeline_Demo.png'>"
collection: portfolio
---

Overview
======
This pipeline automates neuromodulation assessment by processing recorded EMG signals from respiratory muscles through two main stages: **1) Preprocess** — filtering noise and preparing EMG data, and **2) Evaluation** — identifying and extracting key parameters to compare pre- and post-neuromodulation states in SCI patients and healthy controls.

![Pipeline](/images/Pipeline_Design.png)

Preprocess
======
EMG excerpts for each respiration cycle are extracted using lung airway pressure measurements. To reduce noise, the pipeline employs **Adaptive Template Subtraction** (Petersen et al. 2020) to eliminate rhythmic artifacts, such as heartbeats.

![Preprocess](/images/preprocess.png)

Evaluation
======
For SCI patients, **abnormal breathing cycles or failed respiration initiation** are common and must be filtered out to accurately compare successful cycles. An **original Principal Component Analysis (PCA)-based method** isolates abnormal cycles by analyzing the rolling standard deviation of EMG signals.

![PCA](/images/PCA.png)

In each cycle, the start time, end time, and activation amplitude vary across muscles, making activation regions difficult to locate. This pipeline introduces a method that **cross-correlates airway pressure with EMG rolling standard deviation**, aligning similar patterns to identify peak correlation points and define precise activation ranges.

![Cross](/images/Cross_corr.png)

Results
======
This example compares the highest EMG amplitude during several breathing cycle across SCI patients before and after neuromodulation, and in healthy controls. Neuromodulation improved muscle activity in SCI patients, approaching healthy levels in three key muscles.

![results](/images/results.png)

Impact
======
The pipeline's **versatility** has led to its application in two additional neuromodulation studies, broadening its impact significantly. By providing a reliable tool for isolating and analyzing muscle activity, it enables deeper insights into neuromodulation’s effects, establishing a valuable resource for research and clinical applications in SCI and beyond.
