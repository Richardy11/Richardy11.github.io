---
title: "3D Visual Feedback System for Neuroprosthetics Control"
excerpt: "This project introduces ***the Reviewer***, a novel 3D visual feedback system that enhances myoelectric prosthesis control by allowing users to visualize their EMG signals in real-time. This system **clarifies the relationship between muscle activity and the machine learning algorithms behind prosthetic control**. With intuitive feedback, it tackles challenges like learning curves and misclassifications, helping users produce clearer, more consistent signals for improved neuroprosthetic usability. <br/><img src='/images/3D_System.png'>"
collection: portfolio
---

Overview
======
Upper limb myoelectric prostheses often use pattern recognition (PR) systems that translate electromyography (EMG) signals into specific movements. However, as the number of prosthesis movements grows, users face challenges in generating distinct EMG signals to operate all degrees of freedom. Existing training methods rely on trial and error, where a practitioner guides the user based on EMG strength and channel distribution. We present ***the Reviewer***, a visual feedback interface that projects EMG data into the decoder's classification space, **providing intuitive insight into the PR algorithm’s behavior**.

![Motor-based training overview](/images/3D_System.png)

Design
======
Motor-based training in PR-based prostheses includes calibration and exploration phases. In calibration, users perform muscle contractions to record EMG signals, training the motion classifier. In exploration, users receive visual feedback, traditionally via virtual arms, to assess control and refine muscle activity.

![Illustration of motor based training](/images/Demo.png)

Traditional methods are **limited by feedback solely on control output**, leaving a gap in real-time PR algorithm feedback. *The Reviewer* fills this by providing a 3D representation of EMG patterns in decision space, enabling users to visually understand classification accuracy.

![Reviewer vs. Virtual Arm](/images/3DvsVirtual_4.png)

- **The Reviewer (A-C):** Clusters EMG patterns based on calibration, marking rest at the origin. Users see a white cursor representing gesture positions in feature space, offering a 3D view of their movements.
- **Traditional Virtual Arm (D-F):** Displays real-time arm movements based on the PR system’s classifications.

![Reviewer System in Action](/images/3D_System_2.png)

*The Reviewer* enhances PR-based prosthesis control by **enabling users to grasp the link between EMG signals and prosthetic output**, improving both precision and efficiency. A [video demonstration](https://youtube.com/playlist?list=PL9xm11JA4CqgeT2lceSz3rczH2rSDDvDC&si=0_WO4YIB3C59vh_N) is available, illustrating the system's design and experimental setup.

Results
======
In a 10-session study with 12 participants, *the Reviewer* significantly outperformed traditional virtual arm feedback. Key benefits include:
1) **Improved Functionality:** Higher task completion rates and metric improvements in the Fitts’ Law Test.
2) **Scalable Control:** Sustained completion rates as new movements were introduced.
3) **Higher Engagement:** Users recalibrated more frequently for complex assessments, indicating greater motivation and engagement.

For the full report, see the published paper: [Pattern Separability Visual Feedback To Improve Pattern Recognition Decoding Performance](/publication/MEC24_paper_52).

Impact
======
*The Reviewer* represents a breakthrough in PR-controlled prostheses, enhancing accessibility and usability, showcased at **AAOP** and **MEC** conferences. Currently, it is undergoing commercialization by **Infinite Biomedical Technologies**, aiming to benefit the amputee community broadly.

![Showcase](/images/showcase.png)
