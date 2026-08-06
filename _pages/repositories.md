---
layout: page
permalink: /repositories/
title: Service
nav: true
nav_order: 4
---

<style>
  /* ── Section headers ── */
  .sv-section { margin: 2.4rem 0 0.9rem; }
  .sv-section h2 {
    font-size: 1.15rem;
    font-weight: 800;
    border-left: 4px solid var(--global-theme-color);
    padding-left: 0.75rem;
    margin-bottom: 0.2rem;
    color: var(--global-text-color);
  }
  .sv-section-desc {
    font-size: 0.86rem;
    color: var(--global-text-color-light);
    margin: 0 0 0.85rem 1rem;
  }

  /* ── Sub-section label ── */
  .sv-label {
    font-size: 0.68rem;
    font-weight: 800;
    text-transform: uppercase;
    letter-spacing: 0.1em;
    color: var(--global-theme-color);
    margin: 1.4rem 0 0.55rem;
    padding-left: 2px;
  }

  /* ── Venue badge cloud ── */
  .sv-venues {
    display: flex;
    flex-wrap: wrap;
    gap: 0.45rem;
    margin-bottom: 0.6rem;
  }
  .sv-venue {
    display: inline-flex;
    align-items: center;
    gap: 0.3rem;
    font-size: 0.78rem;
    font-weight: 600;
    padding: 4px 12px;
    border-radius: 7px;
    border: 1px solid var(--global-divider-color);
    background: var(--global-card-bg-color);
    color: var(--global-text-color);
    box-shadow: 0 1px 3px rgba(0,0,0,0.05);
    transition: border-color 0.15s, box-shadow 0.15s;
  }
  .sv-venue:hover {
    border-color: var(--global-theme-color);
    box-shadow: 0 2px 8px rgba(0,0,0,0.09);
  }
  .sv-venue-year {
    font-size: 0.68rem;
    font-weight: 400;
    color: var(--global-text-color-light);
    margin-left: 2px;
  }

  /* ── Award callout cards ── */
  .sv-awards { display: flex; flex-direction: column; gap: 0.75rem; margin: 0.9rem 0 0.4rem; }
  .sv-award-card {
    display: flex;
    align-items: flex-start;
    gap: 0.85rem;
    border: 1px solid var(--global-divider-color);
    border-left: 4px solid #f59e0b;
    border-radius: 9px;
    padding: 0.8rem 1.1rem;
    background: var(--global-card-bg-color);
    box-shadow: 0 1px 5px rgba(0,0,0,0.05);
    transition: box-shadow 0.2s;
  }
  .sv-award-card:hover { box-shadow: 0 3px 14px rgba(0,0,0,0.09); }
  .sv-award-card.gold   { border-left-color: #eab308; }
  .sv-award-card.silver { border-left-color: #94a3b8; }
  .sv-award-icon { font-size: 1.5rem; line-height: 1; flex-shrink: 0; margin-top: 2px; }
  .sv-award-body { flex: 1; min-width: 0; }
  .sv-award-title {
    font-size: 0.93rem;
    font-weight: 700;
    color: var(--global-text-color);
    margin: 0 0 0.15rem;
  }
  .sv-award-meta {
    font-size: 0.81rem;
    color: var(--global-text-color-light);
    margin: 0;
    line-height: 1.5;
  }
  .sv-award-badge {
    display: inline-block;
    font-size: 0.65rem;
    font-weight: 700;
    padding: 2px 8px;
    border-radius: 20px;
    letter-spacing: 0.04em;
    margin-left: 0.4rem;
    vertical-align: middle;
  }
  .badge-gold-pill   { background: #fef9c3; color: #854d0e; border: 1px solid #fbbf24; }
  .badge-silver-pill { background: #f1f5f9; color: #475569; border: 1px solid #94a3b8; }

  /* ── Plain role card (Area Chair, Program Committee) ── */
  .sv-role-card {
    border: 1px solid var(--global-divider-color);
    border-left: 4px solid var(--global-theme-color);
    border-radius: 9px;
    padding: 0.75rem 1.1rem;
    background: var(--global-card-bg-color);
    margin-bottom: 0.6rem;
    box-shadow: 0 1px 4px rgba(0,0,0,0.05);
  }
  .sv-role-name {
    font-size: 0.92rem;
    font-weight: 700;
    color: var(--global-text-color);
    margin: 0 0 0.15rem;
  }
  .sv-role-meta {
    font-size: 0.82rem;
    color: var(--global-text-color-light);
    margin: 0;
  }

  /* ── Journal cards ── */
  .sv-journal-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 0.85rem;
    margin-top: 0.5rem;
  }
  @media (max-width: 640px) { .sv-journal-grid { grid-template-columns: 1fr; } }

  .sv-journal-card {
    border: 1px solid var(--global-divider-color);
    border-radius: 10px;
    padding: 0.85rem 1rem;
    background: var(--global-card-bg-color);
    box-shadow: 0 1px 5px rgba(0,0,0,0.05);
    transition: box-shadow 0.2s, transform 0.2s;
  }
  .sv-journal-card:hover {
    box-shadow: 0 4px 16px rgba(0,0,0,0.10);
    transform: translateY(-2px);
  }
  .sv-journal-name {
    font-size: 0.88rem;
    font-weight: 700;
    color: var(--global-text-color);
    margin: 0 0 0.4rem;
    line-height: 1.4;
  }
  .sv-journal-meta {
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    gap: 0.4rem;
  }
  .sv-if {
    font-size: 0.7rem;
    font-weight: 700;
    padding: 2px 9px;
    border-radius: 6px;
    background: #dbeafe;
    color: #1e40af;
    border: 1px solid #93c5fd;
  }
  .sv-year-tag {
    font-size: 0.7rem;
    color: var(--global-text-color-light);
    border: 1px solid var(--global-divider-color);
    padding: 2px 7px;
    border-radius: 6px;
  }

  /* ── Divider ── */
  .sv-divider {
    border: none;
    border-top: 1px solid var(--global-divider-color);
    margin: 2rem 0 0;
  }
</style>

<!-- ══════════════════════════════════════════
     CONFERENCE REVIEWER
     ══════════════════════════════════════════ -->
<div class="sv-section">
  <h2>🧑‍⚖️ Conference Reviewer</h2>
  <p class="sv-section-desc">Peer reviewed submissions across top-tier venues in computer vision, robotics, and machine learning.</p>

  <div class="sv-venues">
    <span class="sv-venue">CVPR <span class="sv-venue-year">2024 · 2025 · 2026</span></span>
    <span class="sv-venue">ICCV <span class="sv-venue-year">2025</span></span>
    <span class="sv-venue">ECCV <span class="sv-venue-year">2026</span></span>
    <span class="sv-venue">ICML <span class="sv-venue-year">2026</span></span>
    <span class="sv-venue">NeurIPS <span class="sv-venue-year">2026</span></span>
    <span class="sv-venue">AAAI <span class="sv-venue-year">2026</span></span>
    <span class="sv-venue">ICRA <span class="sv-venue-year">2025 · 2026</span></span>
    <span class="sv-venue">IROS <span class="sv-venue-year">2026</span></span>
    <span class="sv-venue">WACV <span class="sv-venue-year">2026</span></span>
    <span class="sv-venue">IJCNN <span class="sv-venue-year">2025</span></span>
    <span class="sv-venue">ICASSP <span class="sv-venue-year">2024 · 2025</span></span>
    <span class="sv-venue">BMVC <span class="sv-venue-year">2026</span></span>
    <span class="sv-venue">ETAAV <span class="sv-venue-year">2025</span></span>
    <span class="sv-venue">AeroCON <span class="sv-venue-year">2024</span></span>
  </div>

  <p class="sv-label">Reviewer Recognition</p>
  <div class="sv-awards">
    <div class="sv-award-card gold">
      <div class="sv-award-icon">🥇</div>
      <div class="sv-award-body">
        <p class="sv-award-title">
          Gold Reviewer Award — ICML 2026
          <span class="sv-award-badge badge-gold-pill">Top Reviewers</span>
        </p>
        <p class="sv-award-meta">Placed among the top reviewers; awarded complimentary conference registration in recognition of the contribution.</p>
      </div>
    </div>
    <div class="sv-award-card silver">
      <div class="sv-award-icon">🏅</div>
      <div class="sv-award-body">
        <p class="sv-award-title">
          Outstanding Reviewer Award — CVPR 2025
          <span class="sv-award-badge badge-silver-pill">Top 711 / 12,593</span>
        </p>
        <p class="sv-award-meta">Recognised in the top 5.6% of all reviewers at CVPR 2025.</p>
      </div>
    </div>
    <div class="sv-award-card silver">
      <div class="sv-award-icon">🏅</div>
      <div class="sv-award-body">
        <p class="sv-award-title">Outstanding Reviewer Award — ICCV 2025</p>
        <p class="sv-award-meta">Recognised as an outstanding reviewer at ICCV 2025.</p>
      </div>
    </div>
  </div>
</div>

<hr class="sv-divider">

<!-- ══════════════════════════════════════════
     AREA CHAIR
     ══════════════════════════════════════════ -->
<div class="sv-section">
  <h2>🧭 Area Chair</h2>
  <div class="sv-role-card">
    <p class="sv-role-name">AI for Drones Track — ETAAV, IISc Bangalore</p>
    <p class="sv-role-meta">Emerging Technology in Autonomous Aerial Vehicles (ETAAV) · Indian Institute of Science</p>
  </div>
</div>

<hr class="sv-divider">

<!-- ══════════════════════════════════════════
     PROGRAM COMMITTEE
     ══════════════════════════════════════════ -->
<div class="sv-section">
  <h2>🧾 Program Committee</h2>
  <div class="sv-role-card">
    <p class="sv-role-name">Program Committee Member — AAAI 2026</p>
    <p class="sv-role-meta">AAAI Conference on Artificial Intelligence, 2026</p>
  </div>
</div>

<hr class="sv-divider">

<!-- ══════════════════════════════════════════
     JOURNAL REVIEWER
     ══════════════════════════════════════════ -->
<div class="sv-section">
  <h2>📘 Journal Reviewer</h2>
  <p class="sv-section-desc">Regular peer review for high-impact international journals.</p>

  <div class="sv-journal-grid">

    <div class="sv-journal-card">
      <p class="sv-journal-name">IEEE Robotics and Automation Letters (RAL)</p>
      <div class="sv-journal-meta">
        <span class="sv-if">IF 5.2</span>
        <span class="sv-year-tag">2024</span>
        <span class="sv-year-tag">2025</span>
      </div>
    </div>

    <div class="sv-journal-card">
      <p class="sv-journal-name">ISPRS Journal of Photogrammetry and Remote Sensing</p>
      <div class="sv-journal-meta">
        <span class="sv-if">IF 12.7</span>
        <span class="sv-year-tag">2023</span>
      </div>
    </div>

    <div class="sv-journal-card">
      <p class="sv-journal-name">IEEE Transactions on Image Processing</p>
      <div class="sv-journal-meta">
        <span class="sv-if">IF 13.7</span>
        <span class="sv-year-tag">2025</span>
      </div>
    </div>

  </div>
</div>
