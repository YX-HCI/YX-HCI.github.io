---
layout: page
title: Multi-robot path finding <a href="https://yy-gx.github.io/assets/pdf/BCBSD__in_progress_.pdf" target="_blank" rel="noopener noreferrer" class="float-right"><i class="fas fa-file-pdf"></i></a>
description: Anytime Bounded Conflicted-Based algorithm for Dynamic Environments
img: assets/img/project_imgs/icra21.gif
importance: 3
category: Robotics
---


This is a research project that proposes a bounded conflicted-based algorithm for dynamic environments. Here's the project paper link: [BCBSD: Anytime Bounded Conflicted-Based algorithm for Dynamic Environments](https://yy-gx.github.io/assets/pdf/BCBSD__in_progress_.pdf).


# Abstract 
We present a noval algorithm for MAPF(multi-agent path finding) problem in real world scenarios. Considering the inaccuracies in perception and dynamic properties of real-world events, we use accurate decentralized perception to enhance global detection of obstacles. Based on anytime BCBS algorithm we develop the low level Focal Search to consider the dynamic obstacles and unpredictable events in real-world situations. 

# Methodology
<div class="row justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/mapf/algo1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/mapf/algo2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, low level of anytime BCBS for dynamic obstacles. On the right, detect dangerous points.
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/mapf/a1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/mapf/a2.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    In the figure, taller robots are dynamic obstacles, which central perceptions cannot get their positions accurately nor in real-time. Their motions are marked as red arrows. Small robots are agents we can control by our algorithm, with certain start and goal locations. Their calculated paths are marked as blue arrows. The rectangular boxes are static obstacles, which cannot move and their positions are exactly known by central server. As Our method is CBS based algorithm. We developed anytime BCBS to handle real world scenarios where there might be unpredictable events and the central perception suffered from inaccurate detection of dynamic obstacle. We use detection from decentralized robot to enhance the centralized perception for more accurate path planning.
</div>

