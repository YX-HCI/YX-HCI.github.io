---
layout: page
title: Multimodal BCI Game for Children <a href="https://yx-hci.github.io/assets/pdf/BCI.pdf" target="_blank" rel="noopener noreferrer" class="float-right"><i class="fas fa-file-pdf"></i></a>
description: Exploration of Brain-Computer Interaction for Supporting Children’s Attention Training - A Multimodal Design Based on Attention Network and Gamification.
img: assets/img/project_imgs/p3.jpg
importance: 3
category: C1
---



This is a project I led when I was Information and Interaction Lab @ School of Design for over 2 year. And published as the first student author in IJERPH.    

Here’s the project paper link: 
- Chang, D., Xiang, Y., Zhao, J., Qian, Y., & Li, F. (2022). Exploration of Brain-Computer Interaction for Supporting Children’s Attention Training: A Multimodal Design Based on Attention Network and Gamification Design.International Journal of Environmental Research and Public Health, 19(22), 15046, https://doi.org/10.3390/ijerph192215046, (SCI, IF=4.614, JCR Q1, First student author).



Recent developments in brain-computer interface (BCI) technology have shown great potential in terms of estimating users’ mental state and supporting children’s attention training. However, existing training tasks are relatively simple and lack a reliable task-generation process. Moreover, the training experience has not been deeply studied, and the empirical validation of the training effect is still insufficient. This study thusly proposed a BCI training system for children’s attention improvement. In particular, to achieve a systematic training process, the attention network was referred to generate the training games for alerting, orienting and executive attentions, and to improve the training experience and adherence, the gamification design theory was introduced to derive attractive training tasks. A preliminary experiment was conducted to set and modify the training parameters. Subsequently, a series of contrasting user experiments were organized to examine the impact of BCI training. To test the training effect of the proposed system, a hypothesis-testing approach was adopted. The results revealed that the proposed BCI gamification attention training system can significantly improve the participants’ attention behaviors and concentration ability. Moreover, an immersive, inspiring and smooth training process can be created, and a pleasant user experience can be achieved. Generally, this work is promising in terms of providing a valuable reference for related practices, especially for how to generate BCI attention training tasks using attention networks and how to improve training adherence by integrating multimodal gamification elements.

# Establishment of BCI Gamification Training System

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/bci/1.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The overall framework of the training system (authors’ proposal).
</div>



The BCI attention training system based on ANT and gamification is developed. In particular, two subsystems are constructed, including the hardware system, which detects the brain signals, and the software system, which mainly includes a training game referring to ANT and the Octalysis framework. in particular, consumer-grade brain–computer devices are employed to detect the EEG signals from users. The data are then transmitted to data analysis software, which allows the retrieval of brain wave data by third-party applications or devices and conducts the data processing, data filtering and basic calculations. With the brain signals inputs, the game development tool of Unity is used to realize the training game. The connections between the hardware and software are presented.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/bci/2.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The detailed development procedures of the training system (authors’ proposal).
</div>


Phase 1 is to configure the hardware settings to detect and collect the brain signals. Phases 2 and 3 are to construct the training games. With the data captured by BCI devices and the training games, the whole training system can be built.


# Game development
## Training software - Game Development Platform



<div class="row justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/4.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    Left: Attention value thresholds for different difficulty levels. Right: The structure of the game system.
</div>




<div class="row justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/5.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/6.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: The sequence of events of the alerting game.  Right: Higher difficulty of the alerting game.
</div>

## Multimodal Interaction System Based on Gamification Design

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/bci/7.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Difficulty levels of the operation interaction modes.
</div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/bci/8.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Visual interfaces for different game scenarios. (a) Visual interface of the alerting game. (b) Visual interface of the orientation game. (c) Visual interface of the executive control game.
</div>





<div class="row justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/9.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/10.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: Examples of the training incentives and feedback. Right: Examples of the feedback animation after one round of training..
</div>

# Evaluation Experiments of the BCI Attention Training Game

## A. Preliminary Experiments  
### Establishment of EEG Training Set  


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/bci/11.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 14.EEG command training.
</div>



### Determination of Focus Value Thresholds

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/bci/12.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 15.Recording time of Focus value measurement.
</div>

## B. Formal Experiments

### Participants

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/bci/13.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The game training process of the experimental group.
</div>


### Experiment Process
The experimental process lasted 16 days and consisted of three parts.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/bci/14.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Experiment process.
</div>


### Evaluation Metrics
In children’s behavior evaluation, the Conners Child Behavior Scale (Parent Edition) was used. The four-point rating scale of 0, 1, 2, 3 (annotated by “Never”, “Sometimes”, “Often”, “Very often”) was used.

To assess children’s concentration level, the Schulte Grid Test was adopted. Considering the young age of the children, a 4 × 4 size Schulte Grid Test was adopted in this experiment.

For user experience evaluation, In-Game Experience scale was provided. It is a streamlined version of the GEQ, which is usually used to assess players’ game experience, which consists of seven dimensions: immersion, tension, competence, challenge, flow, and positive and negative affect, with two questions under each dimension, totaling 14 questions.

# Results Analysis

## Participants’ original attention ability in two groups before the training 



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/bci/15.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Conners Child Behavior Scale score comparison between the experimental group and the control group before the experiment.
</div>



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/bci/16.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The Schulte grid test comparison between the experimental group and the control group before the experiment.
</div>

No significant difference is presented in their original concentration ability, and the subsequent comparison of their training results has analytical significance.






## Analysis of the Training Results before and after the Experiment

### Comparative Analysis before and after Training in Experimental Group


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/bci/17.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The Conners Child Behavior Scores of the experimental group before and after the experiment.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/bci/18.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The Schulte Grid Test results before and after the experiment in the experimental group.
</div>

### Comparative Analysis before and after Training in Control Group
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/bci/19.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The Conners Child Behavior Scores in the control group before and after the experiment.
</div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/bci/20.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The Schulte Grid Test results before and after the experiment in the control group.
</div>

According to the analysis above, it can be concluded that the experimental group with BCI training showed significantly improved attention levels. The training game could provide a positive intervention effect on children’s attention performance.

### Analysis of the Game Reaction Time 
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/bci/21.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The rate of change of the attention network parameters.
</div>


To further analyze participants’ performance in each attention network, the participants’ reaction time (RT), which is the main parameter to measure the efficiency of each network, was emphatically analyzed. In particular, the change rate of the participants’ RT between the first-time training and last training was calculated. The rate of change = (RT (first time) − RT (last time))/RT (first time). The positive change rate means an improvement was presented. The higher the absolute value of the change rate, the better the improvement effect is.



### Analysis of Game Experience


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/bci/22.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The score of each dimension of the game experience scale.
</div>


From the emotion-related scores, it can be seen that users enjoyed the training process very much, and clear positive feelings can be observed. The ratings on immersion and fluency are also good (higher than 3.0), which reflects that the game can create an immersive training environment and deliver a smooth game process for the participants. The ratings of competence and challenge are acceptable, which means the training has proper difficulty since the participants can have basic control over the tasks and feel challenged to some extent. The feedback on tension is low (with a score of 1.0), which implies the overall training is comfortable, and more inspiring challenges can be considered.



# Contributions

Specifically, the study makes several contributions as follows:

1. The development of a new and effective BCI attention training system with reference to attention network theory, which can guide task generation for altering, orienting and executive attentions.
2. A multimodal gamification design approach, which can guide the integration of multimodal design elements for improving user experience and training adherence.
3. The demonstration of the efficiency of the proposed BCI training game in improving normal children’s attention ability via a hypothesis-testing experiment.

Generally, valuable references are provided for BCI attention training practices in designing effective and attractive training tasks, and for systematic evaluation of the training effect. Especially in the context of school education, the training system can provide an enjoyable way to help young students improve their attention level and better prepare for systematic school learning. 

To better investigate the BCI intervention influence, long-term training will be considered to help participants achieve basic learning of brain–computer interaction, and to then arrange the training tasks with complete BCI control to investigate if it can lead to a higher training efficiency and better training effect.










