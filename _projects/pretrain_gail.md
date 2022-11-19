---
layout: page
title: Pre-train of GAIL <a href="https://yy-gx.github.io/assets/pdf/CS_7649___Final.pdf" target="_blank" rel="noopener noreferrer" class="float-right"><i class="fas fa-file-pdf"></i></a>
description: Initialization Study of Generative Adversarial Imitation Learning
img: assets/img/project_imgs/7649/framework.png
importance: 6
category: Robotics
---

This is a GaTech course research project that proposes a flexible framework for studying GAIL's initialization. Here's the project paper link: [Initialization Study of Generative Adversarial Imitation Learning](./assets/pdf/example_pdf.pdf)


# Abstract 
Generative Adversarial Imitation Learning (GAIL) is an approach of imitation learning that uses demonstration data by experts and learns the unknown environment’s policy directly from data. One of its drawbacks is that it is unstable and difficult to train, so we propose a flexible framework for studying GAIL's initialization. We design 3 experiments and show that certain instantiations of our framework yields significant improvement gains. We have also provided several conclusions that are valuable for practical GAIL training.

# Methodology
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/7649/framework.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Framework for the initialization of GAIL. The GAIL method will be used as a downstream module for a repeatable pre-train module, where different combinations of method and dynamics will be studied in this report.
</div>

# Results
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/7649/tables.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Statistical Data for All Settings.
</div>
