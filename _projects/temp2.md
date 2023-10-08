---
layout: page
title: Hand Synthesis <a href="https://yy-gx.github.io/assets/pdf/Proposal_hand_synthesize.pdf" target="_blank" rel="noopener noreferrer" class="float-right"><i class="fas fa-file-pdf"></i></a>
description: 
img: assets/img/project_imgs/hand.png
importance: 2
category: Generative Models
---




This is an on-going project advised by professor [Greg Turk](https://faculty.cc.gatech.edu/~turk/). The existing popular generative models (e.g., StyleGAN, Stable Diffusion) perform very poorly in synthesizing hands, which have complicated geometry. Therefore, the research aims to use generative models to synthesize lifelike hands via leveraging some additional information in the input data, including:
- keypoints positions
- skeletons
- dorsal/ventral
- left/right
- ...

 Here's the preliminary research proposal (drafted in August 2022): [proposal](https://yy-gx.github.io/assets/pdf/Proposal_hand_synthesize.pdf).

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/hand.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    One synthesized hand via StyleGAN with our methods.
</div>
