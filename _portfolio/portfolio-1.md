---
title: "3D Visual Feedback System for Neuroprosthetics Control"
excerpt: "This project improves myoelectric prosthesis control through a novel 3D visual feedback system called **Reviewer**, which allows users to visualize their EMG signals in real-time. This system helps users understand how their muscle activity influences the machine learning algorithms underlying control. By providing intuitive visual feedback, it mitigates challenges such as steep learning curves and misclassifications, enabling users to produce clearer, more consistent signals and ultimately enhancing the usability of neuroprosthetics. <br/><img src='/images/3D_System.png'>"
collection: portfolio
---

Overview
======
State-of-the-art upper limb myoelectric prostheses often use pattern recognition (PR) control systems that translate electromyogprahy (EMG) signals into desired movements. As the number of possible prosthesis movements increase, users have difficulty generating sufficiently separable EMG signals that reliably operate all possible degrees of freedom Current training regimens attempt to increase the separability of a user’s EMG signals through trial and error, wherein a practitioner prompts a user to generate EMG signals and provides advice based on the strength and channel distribution of the EMG. We introduce a novel visual feedback interface, the **Reviewer**, which projects incoming EMG data into the classification space of the underlying decoder, enabling intuitive visualization of the pattern recognition (PR) algorithm’s behavior.


Design
======
Motor-based training for PR-based prostheses involves calibration and exploration. During calibration, users perform muscle contractions to record EMG signals, which are used to train a motion classifier algorithms. In exploration, users assess control using visual feedback training programs, like a virtual arm, and can improve control by adjusting muscle activity or recalibrating with new EMG data.

![Illustration of motor based training](/images/Demo.png)

Traditional training methods are limited by their focus on only providing users with feedback on control output. This reveals a gap in current training paradigms, as no existing program offers real-time feedback to show users how the underlying PR algorithm interprets EMG data in its decision space.

![Reviewer VS Virtual Arm](/images/3D_System_2.jpg)

This Reviewer aims to enhance control performance in myoelectric PR-based prostheses by providing users a digestible understanding of the relationship between their input EMG signals and the prosthesis output by projecting them into a 3D space, enabling improvements in control precision and efficiency.

![Reviewer VS Virtual Arm](/images/3DvsVirtual_4.png)

Above is the representation of visualization feedback during gesture performance:
(A-C) The **Reviewer**: Using the PR algorithm, EMG patterns are clustered based on features extracted during calibration. The resting position is marked as the origin (0, 0, 0). Guided by patient data, the system maximizes interclass variance and minimizes within-class variance. During exploration, users see a white cursor representing their gesture’s position in feature space, which they can rotate for a comprehensive view.
(D-F) Virtual Arm: Traditional training method, displays real-time arm movements based on gesture classification by the PR system.


Results
======
In a 10-session study involving 12 participants, users utilizing the **Reviewer** significantly outperformed those using traditional virtual arm feedback training methods. Key improvements included:
 **1) Functionality:** Increased completion rates and improvements in secondary metrics during Fitts’ Law Test assessments for PR-based control.
 **2) Control Scalability:** Attenuated decrease in completion rates when new movements were introduced.
 **3) User Engagement:** Higher engagement and motivation during training, indicated by an increased number of recalibrations before the most complex control assessments.

 For a full report, please refer to the pulished conference paper: 
<a href="/publication/MEC24_paper_52" target="_blank">Full Report on 3D Visual Feedback System for Neuroprosthetics Control</a>


Impact
======
The study results demonstrate that 3D visual feedback tied to the intrinsic decision-space of a pattern recognition-based myoelectric decoder (e.g., the Reviewer system) significantly outperforms standard clinical visualization methods (e.g., virtual arm) in improving control proficiency among naïve prosthesis users. This proposed visualization paradigm marks a significant advancement in making PR-controlled prostheses more accessible and user-friendly, fostering broader adoption and enhanced functional integration. The effectiveness of this system has been showcased at the American Academy of Orthotists and Prosthetists (AAOP) and the Myoelectric Control Symposium (MEC), the premier conference for myoelectric control. Additionally, the system is undergoing commercialization by Infinite Biomedical Technologies, aiming to make a broader impact on the amputee community.

Role of Participants
======
Richard Yang is with the Electrical Engineering Department of Johns Hopkins University. He co-developed the 3D visual system's code, designed and conducted all clinical trials, analyzed the collected data, and wrote the manuscript.

Gyorgy M. Lévay, Christopher L. Hunt, Megan C. Hodgson, Damini Agarwal, Daniel Czeiner, and Rahul R. Kaliki are with Infinite Biomedical Technologies (IBT). They developed the pattern recognition code that this system relies on, for which IBT holds a patent, and co-developed the 3D visual system's code.

Nitish V. Thakor is a co-founder of IBT; his affiliation and potential conflict of interest have been disclosed to the relevant institutions, with conflict management overseen by JHU.