---
layout: page
title: Complex-Valued Deep Learning
description: Fully complex-valued neural architectures for signal and image processing with richer representational capacity.
img: assets/img/publication_preview/ICASSP_Block.drawio.png
importance: 6
category: Research
---

Complex-valued deep learning extends conventional real-valued neural networks to operate entirely in the complex domain, where each neuron processes both the amplitude and phase of a signal. This yields richer representational capacity and is particularly well-suited for signals that inherently carry phase information — such as InSAR (Interferometric Synthetic Aperture Radar) imagery and RF signals. Our work introduces the first fully complex-valued architectures for visual perception and SAR-based building segmentation. [Code](https://github.com/Sumanth181099/DeepMAO)

Fully Complex-Valued Deep Learning Model for Visual Perception (ICASSP 2023):

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/ICASSP_Block.drawio.png" title="Complex-Valued Visual Perception Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A fully complex-valued deep learning scheme for visual perception tasks. The network operates end-to-end in the complex domain, demonstrating improved representational capacity and performance over real-valued counterparts.
</div>

FC2MFN: Fully Complex-Valued Fully Convolutional Multi-Feature Fusion Network for InSAR Segmentation (SSCI 2022):

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/CVCMFFNet-block_diagram.drawio.png" title="FC2MFN Block Diagram" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    FC2MFN is a fully complex-valued fully convolutional network with multi-feature fusion for building segmentation from InSAR imagery, leveraging complex-valued operations throughout to preserve phase coherence.
</div>
