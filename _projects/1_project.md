---
layout: page
title: Domain Generalization
description: Learning models that generalize to unseen target domains without target data during training.
img: assets/img/publication_preview/arch.png
importance: 1
category: Research
---

My research focuses on domain generalization and robust perception for real-world computer vision systems. Traditional deep learning models are typically trained on static datasets, but their performance often degrades when deployed in dynamic and unseen environments. While modern foundation models benefit from internet-scale pretraining, they still struggle with fine-grained downstream tasks and out-of-distribution scenarios.

A key aspect of my research philosophy is the emphasis on **real-world deployment** rather than toy benchmark settings. The objective is not merely to achieve improvements on curated datasets, but to design models that remain reliable under practical challenges such as adverse weather, sensor degradation, missing modalities, unseen domains, and open-world conditions. My work therefore focuses on building deployable, scalable, and robust perception systems that generalize effectively beyond controlled laboratory environments.

---

## Vision-Only Domain Generalization

I have worked extensively on improving the robustness of vision-only models under severe environmental shifts such as rain, fog, night-time conditions, and sim-to-real transfer.

**Multi-Resolution Feature Perturbation (MRFP)**

We introduced MRFP, one of the earliest feature perturbation frameworks that leveraged an overcomplete branch architecture for domain generalization. The model was trained entirely in simulated environments but demonstrated strong generalization to real-world datasets and challenging weather conditions including fog and rain. This work established that carefully designed feature perturbation mechanisms can significantly improve robustness without requiring target-domain supervision.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/arch.png" title="MRFP Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    MRFP: Multi-resolution feature perturbation framework for Sim-to-Real generalizable semantic segmentation. (CVPR 2024)
</div>

**Metacognitive Learning for Environmental Robustness**

To further address environmental uncertainty, we proposed a metacognition-based training framework for semantic segmentation and detection tasks. The framework learns uncertainty-aware representations that enable models trained in sunny conditions to generalize effectively to adverse weather scenarios. This research demonstrated how metacognitive principles can improve resilience against unseen environmental conditions while preserving performance on standard domains.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/MCMRCNN.png" title="Metacognitive Mask R-CNN" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Metacognitive Mask R-CNN for domain generalization under environmental uncertainties such as fog, rain, and varying illumination. (ETAAV 2025)
</div>

---

## Multi-Modal Learning for Robust Perception

RGB imagery alone often becomes unreliable in low-light or adverse weather settings. To overcome these limitations, my work explores complementary sensing modalities such as Infrared (IR) and SAR, enabling robust perception under challenging conditions.

**SKD-Net**

In SKD-Net, we introduced a spectral-based knowledge distillation framework for RGB-IR learning in low-light robotic perception tasks. The method was designed to transfer complementary information across modalities while preserving modality-specific representations.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/icra_demo.drawio.png" title="SKD-Net" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    SKD-Net: Spectral-based knowledge distillation for RGB-IR low-light robotic perception. (ICRA 2024)
</div>

**OGP-Net**

Building on this direction, we proposed OGP-Net, one of the first frameworks to tightly integrate channel exchange mechanisms, pixel-level contrastive distillation, and knowledge distillation for missing-modality robustness. The framework learns modality-shared representations while retaining modality-specific characteristics, allowing robust segmentation even when one modality is unavailable at inference time.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/final11.drawio_updated.drawio.png" title="OGP-Net Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    OGP-Net: Optical guidance with pixel-level contrastive distillation for robust multi-modal and missing-modality segmentation. (AAAI 2025)
</div>

---

## Foundation Models and Vision-Language Learning

Although foundation models and vision-language models (VLMs) exhibit remarkable zero-shot capabilities, they often produce noisy predictions for dense prediction tasks such as segmentation and detection, particularly in adverse or unseen domains. My recent work focuses on adapting these large-scale pretrained models for robust fine-grained perception while preserving their broad generalization capabilities.

**Zero-Shot Domain Adaptation with Contrastive Learning**

We proposed a systematic contrastive learning framework that leverages textual attributes to improve encoder robustness under adverse conditions such as rain, fog, and night-time environments. Using models such as CLIP, the framework improves zero-shot adaptation performance without requiring labeled target-domain data. In parallel, we also introduced one of the early prompt-learning formulations specifically designed for ResNet-based backbones, extending prompt tuning beyond transformer architectures.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/PIN_arch.drawio.png" title="Picazo Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Picazo: Pixel-aligned contrastive learning for zero-shot domain adaptation. (CVPR 2025)
</div>

**CROMPT**

We further extended this line of work with CROMPT, which adapts CLIP via cross-modal prompting to achieve robust zero-shot generalization under adverse weather conditions. By jointly conditioning visual and textual prompts on weather-aware context, the model retains CLIP's broad generalization capabilities while substantially improving robustness in rain, fog, and low-light scenes.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/m1_m2_detection_2.png" title="CROMPT" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    CROMPT: Adapting CLIP via cross-modal prompting for robust zero-shot generalization under adverse weather.
</div>

**Open-Vocabulary and Out-of-Distribution Generalization**

Another major direction of my research involves understanding and improving open-vocabulary segmentation models under challenging out-of-distribution scenarios. I have worked extensively on prompt learning for open-vocabulary models, cost aggregation mechanisms, optimal transport formulations, and cross-domain generalization across highly diverse benchmarks — including medical imaging, agriculture, autonomous navigation, aerial imagery, and underwater perception.

**OV-COAST**

In OV-COAST, we introduced a cost aggregation framework based on optimal transport for open-vocabulary semantic segmentation. The method improves alignment between visual and textual representations, enabling stronger generalization to unseen domains and categories.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/fig1_other.drawio.png" title="OV-COAST" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    OV-COAST: Cost aggregation with optimal transport for open-vocabulary semantic segmentation. (CVPRW 2025)
</div>

**CoLoRA**

Extending OV-COAST's optimal transport formulation, CoLoRA is a prompt learning framework that combines two key components: Cost-Aware Optimal Transport via Aggregation (COAT) and LoRA adaptation applied at model convergence. Evaluated across 19 multi-domain datasets, CoLoRA achieves state-of-the-art performance, producing a more generalizable open-vocabulary segmentation model while adding only a marginal increase in parameters compared to the baseline, and consistently outperforms existing methods across diverse domains. [Project page](/publications/colora/)

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/EP_1st_pageV8_no_shadow.png" title="CoLoRA" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    CoLoRA: Optimal transport meets LoRA for multi-domain open-vocabulary segmentation. (IROS 2026)
</div>

---

## Publications

**Vision-Only Domain Generalization**
- MRFP: Learning Generalizable Semantic Segmentation from Sim-2-Real with Multi-Resolution Feature Perturbation — *CVPR 2024*
- Domain Generalization for Environmental Uncertainties using Metacognitive Mask R-CNN — *ETAAV 2025*

**Multi-Modal Learning**
- SKD-Net: Spectral-based Knowledge Distillation in Low-Light Thermal Imagery for Robotic Perception — *ICRA 2024*
- OGP-Net: Optical Guidance Meets Pixel-Level Contrastive Distillation for Robust Multi-Modal and Missing Modality Segmentation — *AAAI 2025*

**Vision-Language and Foundation Models**
- PICAZO: Pixel-Aligned Contrastive Learning for Zero-Shot Domain Adaptation — *CVPR 2025*
- CROMPT: Adapting CLIP via Cross-Modal Prompting for Robust Zero-Shot Generalization under Adverse Weather

**Open-Vocabulary Segmentation**
- OV-COAST: Cost Aggregation with Optimal Transport for Open-Vocabulary Semantic Segmentation — *CVPRW 2025*
- CoLoRA: Optimal Transport Meets LoRA for Multi-Domain Open-Vocabulary Segmentation — *IROS 2026* — [project page](/publications/colora/)

---

## Further Resources

A broader overview of this research, including its motivation, methodology, and real-world impact, is presented in my [PhD thesis defence](https://youtu.be/GEYRJsyct4c?si=OdDc6-BjTMDvDKXm).

Additionally, several of these themes — domain generalization, robust perception, and multi-sensor fusion — are covered in depth in our [NPTEL course on AI-Driven Perception, Mapping and Planning for Autonomous Drones](https://onlinecourses.nptel.ac.in/e-learning/preview/noc26_ee96), which provides a structured treatment of how these techniques translate to deployable aerial systems.
