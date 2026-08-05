<!-- ---
title: About Newton
--- -->

<style>
  /* ── Section headers ── */
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

  /* ── Package card ── */
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
  .os-link-pill {
    display: inline-flex;
    align-items: center;
    gap: 0.3rem;
    font-size: 0.75rem;
    font-weight: 600;
    padding: 3px 11px;
    border-radius: 20px;
    text-decoration: none;
    border: 1px solid var(--global-theme-color);
    color: var(--global-theme-color);
    white-space: nowrap;
    transition: background 0.15s, color 0.15s;
  }
  .os-link-pill:hover { background: var(--global-theme-color); color: #fff; }
  .os-link-pill svg { width: 13px; height: 13px; fill: currentColor; flex-shrink: 0; }

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

  .os-card-img-wrap {
    flex-shrink: 0;
    width: 280px;
    max-width: 100%;
    text-align: center;
  }
  .os-card-img-wrap img {
    width: 100%;
    height: auto;
    border-radius: 6px;
    border: 1px solid var(--global-divider-color);
    display: block;
  }
  .os-card-img-caption {
    font-size: 0.77rem;
    color: var(--global-text-color-light);
    margin-top: 0.4rem;
    font-style: italic;
    line-height: 1.4;
  }

  /* ── Topic / tech tags ── */
  .os-topics { display: flex; flex-wrap: wrap; gap: 0.4rem; margin-top: 0.75rem; }
  .os-topic {
    font-size: 0.74rem;
    font-weight: 500;
    padding: 3px 11px;
    border-radius: 14px;
    background: var(--global-theme-color);
    color: #fff;
    letter-spacing: 0.01em;
  }
  .os-topic-label {
    font-size: 0.73rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.07em;
    color: var(--global-text-color-light);
    margin: 0.85rem 0 0.15rem;
  }

  /* ════════════════════════════════
     Dataset cards (creative layout)
     ════════════════════════════════ */
  .ds-card {
    border-radius: 12px;
    overflow: hidden;
    margin-bottom: 1.6rem;
    background: var(--global-card-bg-color);
    box-shadow: 0 2px 8px rgba(0,0,0,0.07);
    transition: box-shadow 0.2s, transform 0.2s;
  }
  .ds-card:hover {
    box-shadow: 0 6px 22px rgba(0,0,0,0.12);
    transform: translateY(-2px);
  }

  /* Coloured banner at top of each dataset card */
  .ds-banner {
    height: 6px;
    width: 100%;
  }

  .ds-inner {
    padding: 1.1rem 1.4rem 1.25rem;
  }

  .ds-head {
    display: flex;
    align-items: flex-start;
    flex-wrap: wrap;
    gap: 0.6rem;
    margin-bottom: 0.9rem;
  }
  .ds-name-block { flex: 1; min-width: 0; }
  .ds-name {
    font-size: 1.15rem;
    font-weight: 800;
    margin: 0 0 0.15rem;
    color: var(--global-text-color);
    letter-spacing: -0.01em;
  }
  .ds-subtitle {
    font-size: 0.82rem;
    color: var(--global-text-color-light);
    margin: 0;
    font-style: italic;
  }
  .ds-links { display: flex; flex-wrap: wrap; gap: 0.4rem; align-items: center; }

  /* Stats row */
  .ds-stats {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-bottom: 1rem;
  }
  .ds-stat {
    display: flex;
    align-items: center;
    gap: 0.35rem;
    background: var(--global-bg-color, #f8f9fa);
    border: 1px solid var(--global-divider-color);
    border-radius: 8px;
    padding: 0.3rem 0.75rem;
  }
  @media (prefers-color-scheme: dark) {
    .ds-stat { background: rgba(255,255,255,0.05); }
  }
  :root[data-theme="dark"] .ds-stat { background: rgba(255,255,255,0.05); }
  .ds-stat-icon { font-size: 0.95rem; line-height: 1; }
  .ds-stat-val  { font-size: 0.88rem; font-weight: 700; color: var(--global-text-color); }
  .ds-stat-key  { font-size: 0.76rem; color: var(--global-text-color-light); }

  /* Two-column body inside dataset card */
  .ds-body {
    display: flex;
    gap: 1.4rem;
    align-items: flex-start;
    flex-wrap: wrap;
  }
  .ds-desc { flex: 1; min-width: 200px; }
  .ds-desc p { font-size: 0.91rem; line-height: 1.65; margin-bottom: 0.5rem; }
  .ds-desc ul { padding-left: 1.2rem; margin: 0.3rem 0; }
  .ds-desc li { font-size: 0.91rem; line-height: 1.6; margin-bottom: 0.35rem; }

  .ds-preview {
    flex-shrink: 0;
    width: 260px;
    max-width: 100%;
  }
  .ds-preview img {
    width: 100%;
    height: auto;
    border-radius: 8px;
    border: 1px solid var(--global-divider-color);
    display: block;
  }
  .ds-preview-caption {
    font-size: 0.76rem;
    color: var(--global-text-color-light);
    font-style: italic;
    margin-top: 0.4rem;
    text-align: center;
    line-height: 1.4;
  }

  /* Sensor / modality badges */
  .ds-modalities { display: flex; flex-wrap: wrap; gap: 0.4rem; margin-top: 0.8rem; }
  .ds-mod {
    display: inline-flex;
    align-items: center;
    gap: 0.25rem;
    font-size: 0.73rem;
    font-weight: 600;
    padding: 3px 10px;
    border-radius: 6px;
  }
  .ds-mod-rgb    { background: #dbeafe; color: #1e40af; border: 1px solid #93c5fd; }
  .ds-mod-ir     { background: #fef3c7; color: #92400e; border: 1px solid #fbbf24; }
  .ds-mod-sar    { background: #ede9fe; color: #5b21b6; border: 1px solid #a78bfa; }
  .ds-mod-sonar  { background: #d1fae5; color: #065f46; border: 1px solid #34d399; }
  .ds-mod-aerial { background: #fce7f3; color: #9d174d; border: 1px solid #f9a8d4; }
  .ds-mod-ground { background: #e0f2fe; color: #075985; border: 1px solid #7dd3fc; }

  @media (max-width: 620px) {
    .os-card-img-wrap, .ds-preview { width: 100%; }
  }
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
          <li>Customised for CLIP's dual-encoder architecture, allowing fine-grained interpretation of which image patches contribute most to a given text query.</li>
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

  <!-- ── IndraEye ── -->
  <div class="ds-card">
    <div class="ds-banner" style="background: linear-gradient(90deg, #f97316, #ef4444);"></div>
    <div class="ds-inner">
      <div class="ds-head">
        <div class="ds-name-block">
          <h3 class="ds-name">IndraEye</h3>
          <p class="ds-subtitle">Multi-Spectral UAV Dataset for Aerial Perception</p>
        </div>
        <div class="ds-links">
          <a href="https://www.kaggle.com/competitions/etaav-eo-ir" target="_blank" class="os-link-pill">
            Kaggle ↗
          </a>
          <a href="https://ieeexplore.ieee.org/document/10052789" target="_blank" class="os-link-pill">
            Paper ↗
          </a>
        </div>
      </div>

      <div class="ds-stats">
        <div class="ds-stat">
          <span class="ds-stat-icon">📷</span>
          <span class="ds-stat-val">2</span>
          <span class="ds-stat-key">Modalities</span>
        </div>
        <div class="ds-stat">
          <span class="ds-stat-icon">🚁</span>
          <span class="ds-stat-val">UAV</span>
          <span class="ds-stat-key">Platform</span>
        </div>
        <div class="ds-stat">
          <span class="ds-stat-icon">🎯</span>
          <span class="ds-stat-val">Slant-Angle</span>
          <span class="ds-stat-key">View</span>
        </div>
        <div class="ds-stat">
          <span class="ds-stat-icon">🏆</span>
          <span class="ds-stat-val">ETAAV</span>
          <span class="ds-stat-key">Competition</span>
        </div>
      </div>

      <div class="ds-body">
        <div class="ds-desc">
          <p>
            <strong>IndraEye</strong> is a multi-spectral aerial dataset captured from UAV platforms at slant angles, providing paired <strong>Electro-Optical (RGB)</strong> and <strong>Infrared (IR)</strong> imagery for drone-based object detection and perception research.
          </p>
          <ul>
            <li>Paired EO–IR imagery from a slant-angle UAV viewpoint, capturing challenging real-world lighting and weather conditions.</li>
            <li>Used as the official dataset for <strong>India's first drone-based object detection competition</strong> at ETAAV, IISc Bangalore, hosted on Kaggle with 82 competing teams.</li>
            <li>Sponsored by <strong>SwaYaan (MeitY, Government of India)</strong>; supports research in multi-modal aerial perception and domain generalization.</li>
            <li>Underpins multiple publications in multi-spectral fusion, visible-to-thermal domain adaptation, and UAV perception.</li>
          </ul>
          <div class="ds-modalities">
            <span class="ds-mod ds-mod-rgb">📷 EO / RGB</span>
            <span class="ds-mod ds-mod-ir">🌡️ Infrared (IR)</span>
            <span class="ds-mod ds-mod-aerial">🚁 Aerial / UAV</span>
          </div>
          <p class="os-topic-label">Tasks &amp; Applications</p>
          <div class="os-topics">
            <span class="os-topic">Object Detection</span>
            <span class="os-topic">Multi-Spectral Fusion</span>
            <span class="os-topic">Domain Adaptation</span>
            <span class="os-topic">Aerial Perception</span>
          </div>
        </div>
        <div class="ds-preview">
          <img src="/assets/img/publication_preview/indraeye.png" alt="IndraEye dataset sample imagery" />
          <p class="ds-preview-caption">Sample EO–IR imagery pairs from the IndraEye dataset.</p>
        </div>
      </div>
    </div>
  </div>

  <!-- ── AetherVision-Bench ── -->
  <div class="ds-card">
    <div class="ds-banner" style="background: linear-gradient(90deg, #6366f1, #0ea5e9);"></div>
    <div class="ds-inner">
      <div class="ds-head">
        <div class="ds-name-block">
          <h3 class="ds-name">AetherVision-Bench</h3>
          <p class="ds-subtitle">Open-Vocabulary RGB-Infrared Benchmark · Multi-Angle Segmentation</p>
        </div>
        <div class="ds-links">
          <a href="https://arxiv.org/abs/2506.03709" target="_blank" class="os-link-pill">
            arXiv ↗
          </a>
          <a href="/publications/pixel2perspective/" class="os-link-pill">
            Webpage ↗
          </a>
        </div>
      </div>

      <div class="ds-stats">
        <div class="ds-stat">
          <span class="ds-stat-icon">🗂️</span>
          <span class="ds-stat-val">13+</span>
          <span class="ds-stat-key">Datasets</span>
        </div>
        <div class="ds-stat">
          <span class="ds-stat-icon">📡</span>
          <span class="ds-stat-val">2</span>
          <span class="ds-stat-key">Modalities</span>
        </div>
        <div class="ds-stat">
          <span class="ds-stat-icon">🔭</span>
          <span class="ds-stat-val">Multi-Angle</span>
          <span class="ds-stat-key">Perspective</span>
        </div>
        <div class="ds-stat">
          <span class="ds-stat-icon">📐</span>
          <span class="ds-stat-val">MSRIQ</span>
          <span class="ds-stat-key">Novel Metric</span>
        </div>
      </div>

      <div class="ds-body">
        <div class="ds-desc">
          <p>
            <strong>AetherVision-Bench</strong> is a large-scale open-vocabulary benchmark for <strong>RGB–Infrared segmentation</strong>, spanning both <strong>aerial and ground-level perspectives</strong>. It challenges vision-language models with cross-modal, multi-view generalization.
          </p>
          <ul>
            <li>Consolidates <strong>13+ datasets</strong> across modalities and viewpoints into a unified evaluation framework for open-vocabulary segmentation models.</li>
            <li>Introduces <strong>MSRIQ</strong> — a novel metric for quantifying cross-modal RGB-IR segmentation uncertainty, enabling principled uncertainty-aware evaluation.</li>
            <li>Adds an <strong>object-localization track</strong> for foundation Vision-Language Models (VLMs), enabling grounded evaluation beyond standard segmentation metrics.</li>
            <li>Accepted at the <em>Foundation Models Meet Embodied Agents</em> workshop at <strong>CVPR 2025</strong>; expanded as <strong>Pixel2Perspective</strong>.</li>
          </ul>
          <div class="ds-modalities">
            <span class="ds-mod ds-mod-rgb">📷 RGB</span>
            <span class="ds-mod ds-mod-ir">🌡️ Infrared (IR)</span>
            <span class="ds-mod ds-mod-aerial">🚁 Aerial</span>
            <span class="ds-mod ds-mod-ground">🚶 Ground-Level</span>
          </div>
          <p class="os-topic-label">Tasks &amp; Applications</p>
          <div class="os-topics">
            <span class="os-topic">Open-Vocab Segmentation</span>
            <span class="os-topic">VLM Evaluation</span>
            <span class="os-topic">Cross-Modal Generalization</span>
            <span class="os-topic">Benchmark</span>
            <span class="os-topic">Multi-View</span>
          </div>
        </div>
        <div class="ds-preview">
          <img src="/assets/img/publication_preview/bench4.drawio.png" alt="AetherVision-Bench overview" />
          <p class="ds-preview-caption">AetherVision-Bench spans aerial and ground perspectives across RGB and infrared modalities.</p>
        </div>
      </div>
    </div>
  </div>
</div>
