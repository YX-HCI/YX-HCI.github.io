---
layout: page
title: Safe IRL <a href="https://yy-gx.github.io/assets/pdf/Paper- DeGov4VC.pdf" target="_blank" rel="noopener noreferrer" class="float-right"><i class="fas fa-file-pdf"></i></a>
description: Decentralized Governance for Virtual Community (DeGov4VC)
img: assets/img/project_imgs/p1.png
importance: 1
category: C1
---

This is a project I led when I was being a research assistant in the MIT Media Lab-City Science Lab @ Shanghai for one year. And published as the first author in DIS ‘23 WiP.    

Here’s the project paper link: 

- Yan Xiang, Qianhui Fan, Kejiang Qian, Jiajie Li, Yuying Tang, and Ze Gao. (2023). “Decentralized Governance for Virtual Community (DeGov4VC): Optimal Policy Design of Human-plant Symbiosis Co-creation.” In Companion Publication of the 2023 ACM Designing Interactive Systems Conference (DIS '23 Companion). Association for Computing Machinery, New York, NY, USA, 207–212. https://doi.org/10.1145/3563703.3596621, (ACM).


This is an on-going research project that aims to mitigate safety issues in Inverse Reinforcement Learning (IRL) via leveraging the Control Barrier Function (CBF), advised by professor [Matthew Gombolay
](https://core-robotics.gatech.edu/people/matthew-gombolay/). Progressive results are accepted by [CoRL' 22 Learning for Agile Robotics (LAR) Workshop](https://www.agilerobotscorl2022.com/).


# Abstract 
Learning from Demonstration (LfD) is a powerful method for enabling robots to perform novel tasks as it is often more tractable for a non-roboticist end-user to demonstrate the desired skill and for the robot to efficiently learn from the associated data than for a human to engineer a reward function for the robot to learn the skill via reinforcement learning (RL). Safety issues arise in modern LfD techniques, e.g., Inverse Reinforcement Learning (IRL), just as they do for RL; yet, safe learning in LfD has received little attention. In the context of agile robots, safety is especially vital due to the possibility of robot-environment collision, robot-human collision, and damage to the robot. In this paper, we propose a safe IRL framework, **CBFIRL**, that leverages the Control Barrier Function (CBF) to enhance the safety of the IRL policy. The core idea of CBFIRL is to combine a loss function inspired by CBF requirements with the objective in an IRL method, both of which are jointly optimized via gradient descent. In the experiments, we show our framework performs safer compared to IRL methods without CBF, that is $\sim15\%$ and $\sim20\%$ improvement for two levels of difficulty of a 2D racecar domain and $\sim 50\%$ improvement for a 3D drone domain. 


# Methodology
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/corl/arch.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This figure depicts the architecture of CBFIRL.
</div>


# Results
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/corl/tables.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This table shows the comparison between CBFIRL and AIRL on two domains.
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/corl/heatmap.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/corl/real_agents_crop.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, Heatmap of learned CBF. On the right, 2D racecar environment.
</div>
