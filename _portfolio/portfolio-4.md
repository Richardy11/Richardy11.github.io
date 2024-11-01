---
title: "Automated MRI Toolkit for Brain Structure Analysis"
excerpt: "Introducing an **Automated MRI Toolkit** that synthesizes T2-weighted images from T1-weighted MRI scans, enabling precise brain structure analysis without requiring multiple imaging modalities. This toolkit simplifies research workflows and reduces patient scan time. <br/><img src='/images/MRI.png'>"
collection: portfolio
---

Overview
======
The **Automated MRI Toolkit** streamlines brain structure analysis by generating T2-weighted images directly from T1-weighted (T1w) scans. This approach reduces the need for dual-scan sessions, minimizing patient time in the MRI and lowering costs while maintaining structural contrast and detail.

![MRI Toolkit](/images/MRI.png)

Design
======
The toolkit uses **machine learning models**, including **U-Net** and **CycleGAN** architectures, to accurately synthesize T2w images from T1w inputs. For **image normalization** and **intensity standardization**, it incorporates **Nyul’s method** for consistent inputs, while **FSL’s FAST** segmentation isolates critical brain regions. This integrated process ensures reliable, high-fidelity image synthesis, supporting efficient and comprehensive brain structure analysis.

Results
======
Tests on diverse datasets show the **MRI Toolkit** reliably synthesizes T2-weighted images with structural accuracy comparable to traditional scans. Initial evaluations highlight its potential to **reduce scan times and enhance data utility** in clinical and research workflows. For a detailed report, view the [full report](https://drive.google.com/file/d/11DCDbo6HlgmwllCqoNdVNq89o1mrF9Lm/view?usp=sharing).
