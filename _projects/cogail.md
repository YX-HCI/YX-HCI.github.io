---
layout: page
title: Human Robot Collaboration <a href="https://yy-gx.github.io/assets/pdf/CS_8803___RLR___Final.pdf" target="_blank" rel="noopener noreferrer" class="float-right"><i class="fas fa-file-pdf"></i></a>
description: Learning Diverse Strategies for Human Robot Collaboration via GAIL
img: assets/img/project_imgs/tasks.png
importance: 5
category: Robotics
---


This is a research project that focus on Human-robot collaboration. Here's the project paper link: [Learning Diverse Strategies for Human Robot Collaboration via GAIL](./assets/pdf/example_pdf.pdf)


# Abstract 
Human-robot collaboration will largely improve human efficiency in the future. But it's a hard problem for the robot to sense the diverse strategies that human could adopt and take corresponding actions. A recent approach provides a possible solution to this problem. The Co-GAIL method, which can handle diverse human behaviors for training robot assistants, optimizes human and robot strategies collaboratively during interactive learning. In this paper, we improved the actual collaboration experience between human and robot by proposing two alphas. One is to create a more separable strategy space for the Co-GAIL method. The other one is to introduce a pre-trained role detector to make the flexible switch between human and robot be possible. We don't see a clear improvement in the alpha-1, but a follow-up experiments could indirectly explain the possible reasons. But alpha-2 achieves a nearly similar performance as a pre-defined upper bound.

# Methodology
<div class="row justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/8803/cogail.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/8803/alpha2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, Co-GAIL architecture. On the right, role detector architecture.
</div>



# Results
<div class="row justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/8803/comparison_alpha1(weight1)_baseline.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/8803/alpha2_comparison.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, successful rate with respect to the number of epochs. On the right, comparison between upper bound and alpha-2.
</div>

