---
layout: page
title: View-Agnostic Domain Generalization
description: Segmentation and detection models that generalize across aerial and ground viewpoints without view-specific retraining.
img: assets/img/publication_preview/bench4.drawio.png
importance: 5
category: Research
---

Developing perception models that remain robust across drastically different viewpoints — drone, aerial, and ground-level — without requiring view-specific adaptation or retraining.

{% include figure.liquid loading="eager" path="assets/img/publication_preview/bench4.drawio.png" title="AetherVision-Bench" class="img-fluid rounded z-depth-1" %}

**Key contributions:**
- **AetherVision-Bench** (CVPRW 2025) — Large open-vocabulary RGB-IR benchmark covering multi-angle segmentation across aerial and ground perspectives.
- **Pixel2Perspective** (ICRA 2026, under review) — Expands AetherVision-Bench to 13 datasets, adds an object-localization track for foundation VLMs, and introduces MSRIQ for quantifying cross-modal RGB-IR segmentation uncertainty. [Project page](/publications/pixel2perspective/)
- **SAGA** (CVPRW 2025) — Semantic-aware gray color augmentation for visible-to-thermal cross-modal adaptation across drone and ground-based vision systems.
- **VISTA-CLIP** (CVPRW 2025) — Visual incremental self-tuned adaptation for continual panoptic segmentation across diverse domain shifts.
