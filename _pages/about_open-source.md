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

  /* ── Topic tags ── */
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

  @media (max-width: 600px) {
    .os-card-img-wrap { width: 100%; }
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
<!--  DATASET CONTRIBUTIONS (coming soon)    -->
<!-- ═══════════════════════════════════════ -->
<!--
<div class="os-section">
  <h2>🗄️ Dataset Contributions</h2>

  <div style="display: flex; align-items: flex-start; margin-bottom: 1em;">
    <img src="prof_pic.jpg" alt="IndraEye" style="width: 120px; margin-right: 1em;"/>
    <div>
      <strong>IndraEye</strong>: A large-scale ophthalmic imaging dataset designed to support automated diagnosis and research in medical imaging.
      [Dataset Link](https://example.com)
    </div>
  </div>

  <div style="display: flex; align-items: flex-start; margin-bottom: 1em;">
    <img src="prof_pic.jpg" alt="Side Scan Sonar" style="width: 120px; margin-right: 1em;"/>
    <div>
      <strong>Side Scan Sonar</strong>: Provides sonar imagery for underwater mapping and object detection, useful for marine robotics and exploration tasks.
      [Dataset Link](https://example.com)
    </div>
  </div>

  <div style="display: flex; align-items: flex-start; margin-bottom: 1em;">
    <img src="prof_pic.jpg" alt="IR Imagery" style="width: 120px; margin-right: 1em;"/>
    <div>
      <strong>IR Imagery</strong>: Infrared imagery dataset for research in thermal perception, multi-modal learning, and robotics in low-light conditions.
      [Dataset Link](https://example.com)
    </div>
  </div>
</div>
-->
