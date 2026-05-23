---
layout: page
title: Domain Generalization
description: Learning models that generalize to unseen target domains without target data during training.
img: assets/img/publication_preview/arch.png
importance: 1
category: Research
---

Domain generalization addresses one of the fundamental challenges in deploying deep learning models in the real world: the performance gap that emerges when a model trained on one domain (e.g., simulation) is applied to a different unseen domain (e.g., real-world imagery). The goal is to learn representations that are invariant to domain-specific nuisances — such as lighting, texture, weather, and sensor characteristics — using only source domain data, without any access to the target domain during training. Our work spans Sim-to-Real segmentation, zero-shot domain adaptation, and aerial object detection under environmental uncertainties.

MRFP: Learning Generalizable Semantic Segmentation from Sim-2-Real with Multi-Resolution Feature Perturbation (CVPR 2024):

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/arch.png" title="MRFP Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    MRFP applies multi-resolution feature perturbations during training to encourage the model to learn domain-invariant representations, enabling robust Sim-to-Real transfer for semantic segmentation.
</div>

Picazo: Pixel-Aligned Contrastive Learning for Zero-Shot Domain Adaptation (CVPR 2025):

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/PIN_arch.drawio.png" title="Picazo Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Picazo uses pixel-aligned contrastive learning to align source and target feature distributions at the pixel level, achieving zero-shot domain adaptation without any target domain supervision.
</div>

DGMeta: Domain Generalization for Environmental Uncertainties Using Metacognitive Mask R-CNN (ETAAV 2025):

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/MCMRCNN.png" title="Metacognitive Mask R-CNN" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A metacognitive Mask R-CNN framework that improves domain generalization for aerial object detection under environmental uncertainties such as fog, rain, and varying illumination.
</div>
