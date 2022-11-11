---
layout: page
title: Cross-modal data augmentation
description: Discriminative Cross-Modal Data Augmentation for Medical Imaging Applications
img: assets/img/project_imgs/iclr21.jpg
importance: 1
category: Generative Models
---

This is a research project that aim to mitigate the data deficiency issue via cross-modality data augmentation in the medical imaging domain. Here's the Paper Arxiv link: [Discriminative Cross-Modal Data Augmentation for Medical Imaging Applications](https://arxiv.org/pdf/2010.03468.pdf)

# Abstract
While deep learning methods have shown great success in medical image analysis, they require a number of medical images to train. Due to data privacy concerns and unavailability of medical annotators, it is oftentimes very difficult to obtain a lot of labeled medical images for model training. In this paper, we study cross-modality data augmentation to mitigate the data deficiency issue in the medical imaging domain. We propose a discriminative unpaired image-to-image translation model which translates images in source modality into images in target modality where the translation task is conducted jointly with the downstream prediction task and the translation is guided by the prediction. Experiments on two applications demonstrate the effectiveness of our method. 


# Methodology
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/duiit/archi.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The architecture of our model. The source modality and target modality is CT and MRI respectively. For clarity, we omit the adversarial loss in translating CTs to MRIs.
</div>


# Results
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/duiit/tables.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Comparison between our method and baselines.
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/duiit/iclr21.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/duiit/translated_images.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, some examples of translating MRIs to CTs by CycleGAN and our method. As shown in the regions marked with ovals, our method can better preserve fine-grained details in the translated images than CycleGAN. On the right, examples of translating MRI and PET images into CTs.
</div>

# Citation

{% raw %}
```
@article{yang2020discriminative,
  title={Discriminative Cross-Modal Data Augmentation for Medical Imaging Applications},
  author={Yang, Yue and Xie, Pengtao},
  journal={arXiv preprint arXiv:2010.03468},
  year={2020}
}
```
{% endraw %}





