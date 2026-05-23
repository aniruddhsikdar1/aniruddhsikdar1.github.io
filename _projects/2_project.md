---
layout: page
title: Multi-Spectral Learning
description: Fusion and cross-modal learning across RGB, infrared, and SAR imaging modalities for robust perception.
img: assets/img/publication_preview/final11.drawio_updated.drawio.png
importance: 2
category: Research
---

Multi-spectral learning exploits complementary information across imaging modalities — RGB, infrared (IR), and Synthetic Aperture Radar (SAR) — to build perception systems that are robust under challenging conditions such as low light, fog, and adverse weather. Our work addresses cross-modal fusion, missing-modality robustness, spectral knowledge distillation, and semi-supervised image translation, targeting applications in robotic perception, aerial surveillance, and autonomous systems.

OGP-Net: Optical Guidance Meets Pixel-Level Contrastive Distillation for Robust Multi-Modal Segmentation (AAAI 2025):

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/final11.drawio_updated.drawio.png" title="OGP-Net Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    OGP-Net combines optical guidance with pixel-level contrastive distillation to achieve robust multi-modal segmentation even when one or more input modalities are missing at test time.
</div>

SKD-Net: Spectral-Based Knowledge Distillation in Low-Light Thermal Imagery (ICRA 2024):

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/icra_demo.drawio.png" title="SKD-Net Demo" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    SKD-Net uses spectral-domain knowledge distillation to transfer perceptual knowledge from RGB to thermal imagery, significantly improving robotic perception in low-light environments.
</div>

SSL-RGB2IR: Semi-Supervised RGB-to-IR Image Translation (IROS 2024):

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/adain_final.drawio.png" title="SSL-RGB2IR Translation Framework" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/indraeye.png" title="RGB-IR Results" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    SSL-RGB2IR translates RGB images to IR using a semi-supervised framework, enabling training data augmentation for both semantic segmentation and object detection without requiring paired IR annotations.
</div>
