<!-- ---
title: About Newton
--- -->

<style>
  /* ══════════════════════════════════════
     Section headers
     ══════════════════════════════════════ */
  .os-section { margin: 2.5rem 0 1.2rem; }
  .os-section h2 {
    font-size: 1.25rem;
    font-weight: 700;
    border-left: 4px solid var(--global-theme-color);
    padding-left: 0.75rem;
    margin-bottom: 0.25rem;
    color: var(--global-text-color);
  }
  .os-section-desc {
    font-size: 0.87rem;
    color: var(--global-text-color-light);
    margin: 0 0 0.9rem 1rem;
  }

  /* ══════════════════════════════════════
     Package card
     ══════════════════════════════════════ */
  .os-card {
    border: 1px solid var(--global-divider-color);
    border-radius: 10px;
    overflow: hidden;
    margin-bottom: 1.4rem;
    background: var(--global-card-bg-color);
    box-shadow: 0 1px 5px rgba(0,0,0,0.05);
    transition: box-shadow 0.2s;
  }
  .os-card:hover { box-shadow: 0 4px 16px rgba(0,0,0,0.10); }
  .os-card-header {
    padding: 0.75rem 1.3rem;
    border-bottom: 1px solid var(--global-divider-color);
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    gap: 0.6rem;
  }
  .os-card-title {
    font-size: 1.05rem;
    font-weight: 700;
    color: var(--global-text-color);
    margin: 0;
    flex: 1;
    min-width: 0;
  }
  .os-card-body {
    padding: 1rem 1.3rem;
    display: flex;
    gap: 1.5rem;
    align-items: flex-start;
    flex-wrap: wrap;
  }
  .os-card-text { flex: 1; min-width: 220px; }
  .os-card-text p { font-size: 0.91rem; margin-bottom: 0.5rem; line-height: 1.65; }
  .os-card-text ul { padding-left: 1.2rem; margin: 0.4rem 0; }
  .os-card-text li { font-size: 0.91rem; margin-bottom: 0.35rem; line-height: 1.6; }
  .os-card-img-wrap { flex-shrink: 0; width: 280px; max-width: 100%; text-align: center; }
  .os-card-img-wrap img {
    width: 100%; height: auto; border-radius: 6px;
    border: 1px solid var(--global-divider-color); display: block;
  }
  .os-card-img-caption {
    font-size: 0.77rem; color: var(--global-text-color-light);
    margin-top: 0.4rem; font-style: italic; line-height: 1.4;
  }

  /* ══════════════════════════════════════
     Shared: link pills, topic tags
     ══════════════════════════════════════ */
  .os-link-pill {
    display: inline-flex; align-items: center; gap: 0.3rem;
    font-size: 0.75rem; font-weight: 600; padding: 3px 11px;
    border-radius: 20px; text-decoration: none;
    border: 1px solid var(--global-theme-color);
    color: var(--global-theme-color); white-space: nowrap;
    transition: background 0.15s, color 0.15s;
  }
  .os-link-pill:hover { background: var(--global-theme-color); color: #fff; }
  .os-link-pill svg { width: 13px; height: 13px; fill: currentColor; flex-shrink: 0; }

  .os-topics { display: flex; flex-wrap: wrap; gap: 0.4rem; margin-top: 0.6rem; }
  .os-topic {
    font-size: 0.74rem; font-weight: 500; padding: 3px 11px;
    border-radius: 14px; background: var(--global-theme-color);
    color: #fff; letter-spacing: 0.01em;
  }
  .os-topic-label {
    font-size: 0.73rem; font-weight: 700; text-transform: uppercase;
    letter-spacing: 0.07em; color: var(--global-text-color-light);
    margin: 0.85rem 0 0.15rem;
  }

  /* ══════════════════════════════════════
     Dataset cards
     ══════════════════════════════════════ */
  .ds-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1.2rem;
  }
  @media (max-width: 860px) { .ds-grid { grid-template-columns: 1fr; } }

  .ds-card {
    border-radius: 12px;
    overflow: hidden;
    background: var(--global-card-bg-color);
    border: 1px solid var(--global-divider-color);
    box-shadow: 0 2px 8px rgba(0,0,0,0.06);
    display: flex;
    flex-direction: column;
    transition: box-shadow 0.22s, transform 0.22s;
  }
  .ds-card:hover {
    box-shadow: 0 8px 28px rgba(0,0,0,0.13);
    transform: translateY(-3px);
  }

  /* Gradient top strip — set via inline style */
  .ds-banner { height: 5px; width: 100%; flex-shrink: 0; }

  /* Preview image fills top of card, below banner */
  .ds-img-wrap { position: relative; overflow: hidden; max-height: 160px; }
  .ds-img-wrap img {
    width: 100%; height: 160px; object-fit: cover; display: block;
    filter: brightness(0.92);
    transition: filter 0.25s, transform 0.35s;
  }
  .ds-card:hover .ds-img-wrap img { filter: brightness(1); transform: scale(1.03); }

  /* Floating status pill over the image */
  .ds-status {
    position: absolute; top: 0.6rem; right: 0.7rem;
    font-size: 0.68rem; font-weight: 700; padding: 3px 9px;
    border-radius: 20px; letter-spacing: 0.04em; backdrop-filter: blur(4px);
  }
  .ds-status-public   { background: rgba(16,185,129,0.9); color: #fff; }
  .ds-status-internal { background: rgba(99,102,241,0.9); color: #fff; }
  .ds-status-kaggle   { background: rgba(32,129,226,0.9); color: #fff; }

  .ds-body { padding: 0.95rem 1.1rem 1.1rem; flex: 1; display: flex; flex-direction: column; }

  .ds-head { margin-bottom: 0.6rem; }
  .ds-name {
    font-size: 1.08rem; font-weight: 800; margin: 0 0 0.1rem;
    color: var(--global-text-color); letter-spacing: -0.01em;
  }
  .ds-subtitle {
    font-size: 0.8rem; color: var(--global-text-color-light);
    margin: 0; font-style: italic;
  }

  /* Stats chips row */
  .ds-stats { display: flex; flex-wrap: wrap; gap: 0.4rem; margin: 0.6rem 0; }
  .ds-stat {
    display: inline-flex; align-items: center; gap: 0.3rem;
    background: var(--global-bg-color, #f8f9fa);
    border: 1px solid var(--global-divider-color);
    border-radius: 7px; padding: 0.25rem 0.65rem;
  }
  :root[data-theme="dark"] .ds-stat,
  @media (prefers-color-scheme: dark) { .ds-stat { background: rgba(255,255,255,0.06); } }
  .ds-stat-icon { font-size: 0.85rem; line-height: 1; }
  .ds-stat-val  { font-size: 0.83rem; font-weight: 700; color: var(--global-text-color); }
  .ds-stat-key  { font-size: 0.72rem; color: var(--global-text-color-light); }

  .ds-desc { font-size: 0.88rem; line-height: 1.63; color: var(--global-text-color); margin-bottom: 0.5rem; }

  /* Modality badges */
  .ds-modalities { display: flex; flex-wrap: wrap; gap: 0.35rem; margin: 0.6rem 0 0.5rem; }
  .ds-mod {
    font-size: 0.71rem; font-weight: 600; padding: 2px 9px;
    border-radius: 6px; display: inline-flex; align-items: center; gap: 0.2rem;
  }
  .ds-mod-rgb    { background: #dbeafe; color: #1e40af; border: 1px solid #93c5fd; }
  .ds-mod-ir     { background: #fef3c7; color: #92400e; border: 1px solid #fbbf24; }
  .ds-mod-sar    { background: #ede9fe; color: #5b21b6; border: 1px solid #a78bfa; }
  .ds-mod-sonar  { background: #d1fae5; color: #065f46; border: 1px solid #34d399; }
  .ds-mod-aerial { background: #fce7f3; color: #9d174d; border: 1px solid #f9a8d4; }
  .ds-mod-ground { background: #e0f2fe; color: #075985; border: 1px solid #7dd3fc; }
  .ds-mod-sim    { background: #f0fdf4; color: #166534; border: 1px solid #86efac; }
  .ds-mod-synth  { background: #fff7ed; color: #9a3412; border: 1px solid #fdba74; }

  /* Footer links row */
  .ds-links { display: flex; flex-wrap: wrap; gap: 0.4rem; margin-top: auto; padding-top: 0.75rem; }

  @media (max-width: 600px) { .os-card-img-wrap { width: 100%; } }
</style>

<!-- ═══════════════════════════════════════ -->
<!--  OPEN-SOURCE PACKAGES                   -->
<!-- ═══════════════════════════════════════ -->
<div class="os-section">
  <h2>📦 Open-Source Packages</h2>
  <p class="os-section-desc">Publicly released tools and libraries for the research community.</p>

  <div class="os-card">
    <div class="os-card-header">
      <span class="os-card-title">CLIP-CAM: Explainable Image–Text Alignment for CLIP Models</span>
      <a href="https://github.com/adityagandhamal/clip_cam" target="_blank" class="os-link-pill">
        <svg viewBox="0 0 16 16" xmlns="http://www.w3.org/2000/svg">
          <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38
                   0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13
                   -.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66
                   .07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15
                   -.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0
                   1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82
                   1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01
                   1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"/>
        </svg>
        GitHub
      </a>
      <a href="https://pypi.org/project/clip-cam/" target="_blank" class="os-link-pill">
        <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <path d="M12 0C5.372 0 0 5.373 0 12s5.372 12 12 12 12-5.373 12-12S18.628 0 12 0zm0
                   2c5.514 0 10 4.486 10 10s-4.486 10-10 10S2 17.514 2 12 6.486 2 12 2zm-1
                   5v6H7l5 5 5-5h-4V7h-2z"/>
        </svg>
        PyPI
      </a>
    </div>
    <div class="os-card-body">
      <div class="os-card-text">
        <p>
          <strong>CLIP-CAM</strong> is an open-source Python package for generating
          <strong>Grad-CAM–style visual explanations</strong> in
          <strong>Vision Transformer (ViT)–based CLIP models</strong>, enabling deeper
          insight into how specific image regions drive image–text similarity scores.
        </p>
        <ul>
          <li>Modular and extensible framework for visualizing cross-modal attention in CLIP, built around <strong>Grad-CAM–based heatmap generation</strong>.</li>
          <li>Customised for CLIP's dual-encoder architecture, revealing which image patches contribute most to a given text query.</li>
          <li>Lightweight API — works with standard HuggingFace and OpenAI CLIP checkpoints with minimal setup.</li>
        </ul>
        <p class="os-topic-label">Tech Stack &amp; Topics</p>
        <div class="os-topics">
          <span class="os-topic">CLIP</span>
          <span class="os-topic">Vision Transformers</span>
          <span class="os-topic">Grad-CAM</span>
          <span class="os-topic">Explainability</span>
          <span class="os-topic">Image–Text Alignment</span>
          <span class="os-topic">PyPI Package</span>
        </div>
      </div>
      <div class="os-card-img-wrap">
        <img src="/assets/images/clip_cam.png" alt="CLIP-CAM attention heatmap visualization" />
        <p class="os-card-img-caption">Attention heatmap over the image for a given text prompt.</p>
      </div>
    </div>
  </div>
</div>

<!-- ═══════════════════════════════════════ -->
<!--  DATASET CONTRIBUTIONS                  -->
<!-- ═══════════════════════════════════════ -->
<div class="os-section">
  <h2>🗄️ Dataset Contributions</h2>
  <p class="os-section-desc">Benchmarks and datasets released to advance research in multi-modal perception and autonomous systems.</p>

  <div class="ds-grid">

    <!-- ── IndraEye ── -->
    <div class="ds-card">
      <div class="ds-banner" style="background: linear-gradient(90deg, #f97316, #ef4444);"></div>
      <div class="ds-img-wrap">
        <img src="/assets/img/publication_preview/indraeye.png" alt="IndraEye dataset" />
        <span class="ds-status ds-status-kaggle">Kaggle · Public</span>
      </div>
      <div class="ds-body">
        <div class="ds-head">
          <h3 class="ds-name">IndraEye</h3>
          <p class="ds-subtitle">Multi-Spectral UAV Dataset · Aerial Object Detection</p>
        </div>
        <div class="ds-stats">
          <div class="ds-stat"><span class="ds-stat-icon">📷</span><span class="ds-stat-val">EO + IR</span><span class="ds-stat-key">Modalities</span></div>
          <div class="ds-stat"><span class="ds-stat-icon">🚁</span><span class="ds-stat-val">UAV</span><span class="ds-stat-key">Platform</span></div>
          <div class="ds-stat"><span class="ds-stat-icon">🏆</span><span class="ds-stat-val">82 Teams</span><span class="ds-stat-key">Competition</span></div>
        </div>
        <p class="ds-desc">
          Paired <strong>Electro-Optical (RGB)</strong> and <strong>Infrared</strong> aerial imagery captured at slant angles from UAV platforms, designed for drone-based object detection under challenging real-world conditions. Hosted as India's first drone object detection Kaggle competition at ETAAV, IISc, sponsored by SwaYaan (MeitY, GoI).
        </p>
        <div class="ds-modalities">
          <span class="ds-mod ds-mod-rgb">📷 EO / RGB</span>
          <span class="ds-mod ds-mod-ir">🌡️ Infrared</span>
          <span class="ds-mod ds-mod-aerial">🚁 Aerial</span>
        </div>
        <div class="os-topics">
          <span class="os-topic">Object Detection</span>
          <span class="os-topic">Multi-Spectral Fusion</span>
          <span class="os-topic">Domain Adaptation</span>
        </div>
        <div class="ds-links">
          <a href="https://www.kaggle.com/competitions/etaav-eo-ir" target="_blank" class="os-link-pill">Kaggle ↗</a>
          <a href="https://ieeexplore.ieee.org/document/10052789" target="_blank" class="os-link-pill">Paper ↗</a>
        </div>
      </div>
    </div>

    <!-- ── AetherVision-Bench ── -->
    <div class="ds-card">
      <div class="ds-banner" style="background: linear-gradient(90deg, #6366f1, #0ea5e9);"></div>
      <div class="ds-img-wrap">
        <img src="/assets/img/publication_preview/bench4.drawio.png" alt="AetherVision-Bench" />
        <span class="ds-status ds-status-public">Public · Benchmark</span>
      </div>
      <div class="ds-body">
        <div class="ds-head">
          <h3 class="ds-name">AetherVision-Bench</h3>
          <p class="ds-subtitle">Open-Vocabulary RGB-IR Benchmark · Multi-Angle Segmentation</p>
        </div>
        <div class="ds-stats">
          <div class="ds-stat"><span class="ds-stat-icon">🗂️</span><span class="ds-stat-val">13+</span><span class="ds-stat-key">Datasets</span></div>
          <div class="ds-stat"><span class="ds-stat-icon">📐</span><span class="ds-stat-val">MSRIQ</span><span class="ds-stat-key">Novel Metric</span></div>
          <div class="ds-stat"><span class="ds-stat-icon">🔭</span><span class="ds-stat-val">CVPR '25</span><span class="ds-stat-key">Workshop</span></div>
        </div>
        <p class="ds-desc">
          Large-scale benchmark consolidating <strong>13+ datasets</strong> across RGB and infrared modalities for open-vocabulary segmentation evaluation across aerial and ground perspectives. Introduces <strong>MSRIQ</strong>, a novel metric for cross-modal segmentation uncertainty, and an object-localization track for foundation VLMs.
        </p>
        <div class="ds-modalities">
          <span class="ds-mod ds-mod-rgb">📷 RGB</span>
          <span class="ds-mod ds-mod-ir">🌡️ Infrared</span>
          <span class="ds-mod ds-mod-aerial">🚁 Aerial</span>
          <span class="ds-mod ds-mod-ground">🚶 Ground</span>
        </div>
        <div class="os-topics">
          <span class="os-topic">Open-Vocab Segmentation</span>
          <span class="os-topic">VLM Evaluation</span>
          <span class="os-topic">Multi-View</span>
        </div>
        <div class="ds-links">
          <a href="https://arxiv.org/abs/2506.03709" target="_blank" class="os-link-pill">arXiv ↗</a>
          <a href="/publications/pixel2perspective/" class="os-link-pill">Webpage ↗</a>
        </div>
      </div>
    </div>

    <!-- ── Side Scan Sonar Dataset ── -->
    <div class="ds-card">
      <div class="ds-banner" style="background: linear-gradient(90deg, #0d9488, #0284c7);"></div>
      <div class="ds-img-wrap">
        <img src="/assets/img/publication_preview/m1_m2_detection_2.png" alt="Side Scan Sonar Dataset" />
        <span class="ds-status ds-status-public">Public · Research</span>
      </div>
      <div class="ds-body">
        <div class="ds-head">
          <h3 class="ds-name">Side Scan Sonar Dataset</h3>
          <p class="ds-subtitle">Syn2Real Underwater Mine-Like Object Detection</p>
        </div>
        <div class="ds-stats">
          <div class="ds-stat"><span class="ds-stat-icon">🌊</span><span class="ds-stat-val">SSS</span><span class="ds-stat-key">Sensor</span></div>
          <div class="ds-stat"><span class="ds-stat-icon">💣</span><span class="ds-stat-val">Mine-Like</span><span class="ds-stat-key">Target</span></div>
          <div class="ds-stat"><span class="ds-stat-icon">🔄</span><span class="ds-stat-val">Syn + Real</span><span class="ds-stat-key">Domains</span></div>
        </div>
        <p class="ds-desc">
          Paired <strong>synthetic and real Side-Scan Sonar (SSS)</strong> imagery curated for Syn2Real domain generalization research in underwater mine-like object detection. Supports evaluation of models trained on simulated environments and tested under real underwater acoustic imaging conditions.
        </p>
        <div class="ds-modalities">
          <span class="ds-mod ds-mod-sonar">🔊 Side-Scan Sonar</span>
          <span class="ds-mod ds-mod-sim">🖥️ Synthetic</span>
          <span class="ds-mod ds-mod-ground">🌊 Underwater</span>
        </div>
        <div class="os-topics">
          <span class="os-topic">Syn2Real</span>
          <span class="os-topic">Domain Generalization</span>
          <span class="os-topic">Object Detection</span>
          <span class="os-topic">Underwater Perception</span>
        </div>
        <div class="ds-links">
          <a href="https://ieeexplore.ieee.org/document/10919029/" target="_blank" class="os-link-pill">Paper ↗</a>
        </div>
      </div>
    </div>

    <!-- ── Simulated IR Dataset ── -->
    <div class="ds-card">
      <div class="ds-banner" style="background: linear-gradient(90deg, #7c3aed, #db2777);"></div>
      <div class="ds-img-wrap">
        <img src="/assets/img/publication_preview/adain_final.drawio.png" alt="Simulated IR Dataset" />
        <span class="ds-status ds-status-internal">Research · Internal</span>
      </div>
      <div class="ds-body">
        <div class="ds-head">
          <h3 class="ds-name">Simulated IR Dataset</h3>
          <p class="ds-subtitle">Semi-Supervised RGB-to-IR Translation for Perception Training</p>
        </div>
        <div class="ds-stats">
          <div class="ds-stat"><span class="ds-stat-icon">🌡️</span><span class="ds-stat-val">Infrared</span><span class="ds-stat-key">Modality</span></div>
          <div class="ds-stat"><span class="ds-stat-icon">🖥️</span><span class="ds-stat-val">Simulated</span><span class="ds-stat-key">Source</span></div>
          <div class="ds-stat"><span class="ds-stat-icon">🤖</span><span class="ds-stat-val">SSL</span><span class="ds-stat-key">Approach</span></div>
        </div>
        <p class="ds-desc">
          Synthetically generated <strong>Infrared (IR) imagery</strong> produced via semi-supervised <strong>RGB-to-IR image translation</strong> for augmenting training pipelines in semantic segmentation and object detection tasks. Designed to bridge the modality gap where paired real IR data is scarce, enabling robust training of IR-capable perception models.
        </p>
        <div class="ds-modalities">
          <span class="ds-mod ds-mod-rgb">📷 RGB (Source)</span>
          <span class="ds-mod ds-mod-ir">🌡️ Infrared (Generated)</span>
          <span class="ds-mod ds-mod-synth">⚙️ Synthetic</span>
        </div>
        <div class="os-topics">
          <span class="os-topic">Image Translation</span>
          <span class="os-topic">Semi-Supervised</span>
          <span class="os-topic">Data Augmentation</span>
          <span class="os-topic">IR Perception</span>
        </div>
        <div class="ds-links">
          <a href="https://ieeexplore.ieee.org/document/10802815" target="_blank" class="os-link-pill">Paper ↗</a>
        </div>
      </div>
    </div>

  </div><!-- end .ds-grid -->
</div>
