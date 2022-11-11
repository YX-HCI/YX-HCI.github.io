---
layout: page
title: Safe navigation
description: Interactive Learning on Safe Navigation in Cluster Dynamic Environments
img: assets/img/project_imgs/RL_HI.png
importance: 4
category: Robotics
---

This is a research project that aims to investigate different safe reinforcement learning (RL) approaches for a robot to navigate safely in dynamic cluster environments.


# Abstract 
Safe navigation is essential for mobile autonomous systems to deploy in real-world environments. In this paper, we want to investigate different safe reinforcement learning (RL) approaches for a robot to navigate safely in dynamic cluster environments. Based on the same learning framework where safe action is used, if the RL agent provides an unsafe action, we developed two different approaches: one uses an optimization-based safety controller to produce safe actions, the other uses human interventions as safe actions. Our experiment results indicate that the optimization-based safety controller can safeguard the robot from collision, but the approach using human interventions achieves very similar performance as regular RL.


# Methodology
<div class="row justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/7648/RL_SC.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/7648/RL_HI.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, the proposed reinforcement learning approach with an SSA-based safety controller (safe RL-SC). On the right, the interactive learning approach using human interventions (safe RL-HI).
</div>

# Results
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/7648/tables.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The mean performance of 30 runs of each approach after 200 episodes of training (Success rate/Collision rate/Halting rate).
</div>
