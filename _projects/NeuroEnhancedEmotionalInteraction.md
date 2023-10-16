---
layout: page
title: Neuro-Enhanced Emotional Interaction 
tags: "#Brain Cumputer Interaction, #Emotion, #HRI. "
description: A System Design for Multi-Modal Emotion Regulation and Management in Human-Robot and Human-Computer Interactions.
img: assets/img/project_imgs/Multi-ModalEmotionRegulation/title.png
importance: 6
category: "Human-Computer Interaction (HCI)"
---


Here’s the project paper: 
- **Xiang, Y.** A System Design for Multi-Modal Emotion Regulation and Management in Human-Robot and Human-Computer Interactions.'' In *2024 19th ACM/IEEE International Conference on Human-Robot Interaction (HRI)*. (Submitted). 

**Research on Emotion Recognition and Regulation:**

Analysis of the core literature in the Web of Science indicates a quantifiable growth in the research on emotion recognition and regulation in recent years. Keywords analysis revealed a close relationship between emotion recognition and regulation and electroencephalogram (EEG) signals. A knowledge graph analysis was conducted on the connectivity between emotions and brain-machine-related factors.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/Multi-ModalEmotionRegulation/1.jpg" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 1. Knowledge graph analysis of the connection between emotions and brain-computer relations.
</div>



**Expert Interview Coding:**

In-depth interviews were conducted with doctors from the **Shanghai Mental Health Center**. The interviews covered five main sections, including professional experience, emotional triggers, emotion regulation strategies, and specific implementation methods.

**User Study:**

**Survey:**

The survey included sections on personal information, self-assessment of daily emotional states, three scales (**PSS** for stress, **SAS** for anxiety, **SDS** for depression), and crowd demands for stress relief and healing elements and methods.

**Target User Identification and Coding:**

Based on self-assessment and scale results, 24 users with high stress and anxiety values were selected for interviews and coding. The study identified user personas and preferences for relaxing scenes.

**User Needs:**

Real-time perception of emotional states, emotional system management, positive guidance, and regulation for stress and emotional issues. Users require visual and quantifiable indicators to perceive their current emotional states.

**System Design and Development:**

*Software Development:*
Rhino was used for scene prototyping, Touch Designer and Unity for rendering, and Launch Virtual Serial Port Driver for serial communication and brain-machine interaction. The platform was developed for emotional recognition and visualization by exploring EEG data.

*Hardware:*
EEG caps (eego mylab), Emotiv BCI Epoc, and related brain-machine interface devices were used for signal capture and real-time interaction.

**I. Monitoring and Identification System:**

Utilizing different frequency data, brain-machine interface signals were processed for serial communication and then visualized using Touch Designer. The system included emotional decoding algorithm development.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/Multi-ModalEmotionRegulation/2.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 2. DEMO development of monitoring and identification system.

</div>


<div class="row justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/Multi-ModalEmotionRegulation/3.1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/Multi-ModalEmotionRegulation/3.2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    Figure 3. DEMO development process.
</div>





**II. Emotion Regulation System:**

Six categories of video stimuli were selected to validate their impact on user emotional stress (plants, fire, stream, rainy weather, sunlight, seaside).



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/Multi-ModalEmotionRegulation/4.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 4. Preliminary experiment process.

</div>

<div class="row justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/Multi-ModalEmotionRegulation/5.1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/Multi-ModalEmotionRegulation/5.2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    Figure 5. Formal experiment process.
</div>



**III. Management and Service System:**

Customized emotion management includes monitoring and regulation. The monitoring system visualizes EEG waves for user perception, while the regulation system offers various modules and real-time monitoring, allowing users to select emotion management health reports.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/Multi-ModalEmotionRegulation/6.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 4. APP Demo of management and service system

</div>



**Research Contributions:**

- Investigating the impact of brain-machine interaction on emotional stress relief through various regulation design patterns.
- Developing an emotion monitoring, recognition, and regulation training platform based on EEG signals.
- Designing a multi-sensory regulation training platform and service system through brain-machine interaction, recommending tailored regulation methods based on the analysis results.


**Professional Collaboration and Technical Support:**

- Collaboration with **Ruijin Hospital Brain Disease Center** and participation in their research projects on **brain-machine interfaces and neuroregulation in the field of emotional disorders**.
- Collaboration with the **Shanghai Mental Health Center**, providing professional guidance and design suggestions for various emotional regulation and brain-machine interface experiments, including algorithm development and application methods.

