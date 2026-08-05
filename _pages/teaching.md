---
layout: page
permalink: /teaching/
title: Academic Activities
description: Talks, paper presentations, conferences, and teaching activities.
nav: true
nav_order: 6
---

<style>
  .ac-section { margin: 2.5rem 0 1.2rem; }
  .ac-section h2 {
    font-size: 1.2rem;
    font-weight: 700;
    border-left: 4px solid var(--global-theme-color);
    padding-left: 0.75rem;
    margin-bottom: 0.25rem;
    color: var(--global-text-color);
  }
  .ac-section-desc {
    font-size: 0.81rem;
    color: var(--global-text-color-light);
    margin: 0 0 0.9rem 1rem;
  }

  /* Cards */
  .ac-card {
    border: 1px solid var(--global-divider-color);
    border-radius: 8px;
    padding: 1rem 1.2rem;
    margin-bottom: 1rem;
    background: var(--global-card-bg-color);
  }
  .ac-card-title {
    font-size: 0.95rem;
    font-weight: 600;
    color: var(--global-text-color);
    margin: 0 0 0.25rem;
  }
  .ac-card-meta {
    font-size: 0.77rem;
    color: var(--global-text-color-light);
    margin-bottom: 0.6rem;
  }
  .ac-card p, .ac-card li { font-size: 0.84rem; margin-bottom: 0.3rem; }
  .ac-card ul { padding-left: 1.2rem; margin: 0.4rem 0; }

  /* Badges */
  .ac-badge {
    display: inline-block;
    font-size: 0.68rem;
    font-weight: 600;
    padding: 2px 8px;
    border-radius: 20px;
    margin-right: 0.3rem;
    margin-bottom: 0.3rem;
  }
  .badge-gold   { background: #fff3cd; color: #856404; border: 1px solid #ffc107; }
  .badge-silver { background: #e9ecef; color: #495057; border: 1px solid #adb5bd; }
  .badge-org    { background: #d1ecf1; color: #0c5460; border: 1px solid #bee5eb; }
  .badge-venue  { background: #eef2ff; color: var(--global-theme-color); border: 1px solid var(--global-theme-color); }
  .badge-role-copi { background: #d4edda; color: #155724; border: 1px solid #28a745; font-weight: 700; }
  .badge-role-ta   { background: #fff3cd; color: #856404; border: 1px solid #ffc107; font-weight: 700; }

  /* Scrollable container for talks */
  .ac-scroll-box {
    max-height: 420px;
    overflow-y: auto;
    border: 1px solid var(--global-divider-color);
    border-radius: 8px;
    padding: 0 0.8rem;
    background: var(--global-card-bg-color);
  }
  .ac-scroll-box::-webkit-scrollbar { width: 5px; }
  .ac-scroll-box::-webkit-scrollbar-thumb { background: var(--global-divider-color); border-radius: 4px; }

  /* Timeline */
  .ac-timeline { list-style: none; padding: 0; margin: 0; }
  .ac-timeline li {
    display: flex;
    gap: 1rem;
    padding: 0.7rem 0;
    border-bottom: 1px solid var(--global-divider-color);
  }
  .ac-timeline li:last-child { border-bottom: none; }
  .ac-tl-date {
    min-width: 88px;
    font-size: 0.71rem;
    color: var(--global-text-color-light);
    font-family: monospace;
    padding-top: 3px;
    flex-shrink: 0;
  }
  .ac-tl-title { font-size: 0.86rem; font-weight: 600; margin: 0 0 0.1rem; }
  .ac-tl-venue { font-size: 0.77rem; color: var(--global-text-color-light); margin: 0; }
  .ac-tl-paper { font-size: 0.77rem; font-style: italic; color: var(--global-text-color-light); margin: 0.12rem 0 0; }

  /* Course cards */
  .ac-course {
    border: 1px solid var(--global-divider-color);
    border-radius: 8px;
    overflow: hidden;
    margin-bottom: 1rem;
  }
  .ac-course-header {
    background: var(--global-theme-color);
    color: #fff;
    padding: 0.55rem 1.1rem;
    display: flex;
    align-items: center;
    gap: 0.8rem;
  }
  .ac-course-num {
    font-size: 0.65rem;
    font-weight: 700;
    opacity: 0.8;
    letter-spacing: 0.06em;
    white-space: nowrap;
  }
  .ac-course-header h3 { font-size: 0.93rem; font-weight: 700; margin: 0; color: #fff; }
  .ac-course-body { padding: 0.85rem 1.1rem; }
  .ac-course-body p, .ac-course-body li { font-size: 0.83rem; margin-bottom: 0.3rem; }
  .ac-course-body ul { padding-left: 1.2rem; margin: 0.4rem 0 0; }
  .ac-course-placeholder { font-size: 0.83rem; color: var(--global-text-color-light); font-style: italic; }
</style>

<!-- ═══════════════════════════════════════ -->
<!--  COMPETITIONS & CHALLENGES              -->
<!-- ═══════════════════════════════════════ -->
<div class="ac-section">
  <h2>🏆 Competitions &amp; Challenges</h2>
  <p class="ac-section-desc">Competition participations and organised challenges.</p>

  <div class="ac-card">
    <div class="ac-card-title">Multi-modal Domain Fusion for Multi-modal Aerial View Object Classification</div>
    <div class="ac-card-meta">
      MAVOC Challenge &nbsp;·&nbsp; CVPR-W PBVS 2022 &nbsp;·&nbsp;
      <span class="ac-badge badge-org">Participant</span>
      <a href="https://arxiv.org/pdf/2212.07039" target="_blank">arXiv ↗</a>
    </div>
    <ul>
      <li>Participated as a two-member team in the <strong>Multi-modal Aerial View Imagery Classification (MAVOC)</strong> Challenge.</li>
      <li>Developed a multi-modal deep learning framework learning domain-invariant features from Electro-Optical (EO) and SAR data.</li>
      <li>
        <span class="ac-badge badge-gold">🥇 Track 1 — 5th / 82 teams</span>
        <span class="ac-badge badge-silver">Track 2 — 9th / 77 teams</span>
      </li>
      <li>Methodology published in <em>"Multi-modal aerial view object classification challenge results – PBVS 2022."</em> CVPR Workshops, 2022.</li>
    </ul>
  </div>

  <div class="ac-card">
    <div class="ac-card-title">UAV RGB–IR Slant Angle Object Detection Challenge</div>
    <div class="ac-card-meta">
      ETAAV &nbsp;·&nbsp; IISc Bangalore &nbsp;·&nbsp;
      <span class="ac-badge badge-org">Organiser</span>
      <a href="https://www.kaggle.com/competitions/etaav-eo-ir" target="_blank">Kaggle ↗</a>
    </div>
    <ul>
      <li>Organised <strong>India's first drone-based object detection competition</strong> using RGB and IR imagery on the <strong>Indraeye dataset</strong>.</li>
      <li>Hosted at the <em>International Conference on Emerging Technology in Autonomous Aerial Vehicles (ETAAV)</em>, IISc Bangalore.</li>
      <li>Sponsored by <strong>SwaYaan (MeitY, Government of India)</strong>.</li>
    </ul>
  </div>
</div>

<!-- ═══════════════════════════════════════ -->
<!--  PAPER PRESENTATIONS                    -->
<!-- ═══════════════════════════════════════ -->
<div class="ac-section">
  <h2>🎓 Paper Presentations</h2>
  <p class="ac-section-desc">Also available on the <a href="https://www.youtube.com/@airl_iisc" target="_blank">AIRL YouTube Page</a>.</p>
  <ul class="ac-timeline">
    <li>
      <span class="ac-tl-date">16 Oct 2024</span>
      <div>
        <p class="ac-tl-title"><span class="ac-badge badge-venue">IROS 2024</span> Abu Dhabi, UAE</p>
        <p class="ac-tl-paper">"SSL-RGB2IR: Semi-supervised RGB-to-IR Image-to-Image Translation for Enhancing Vision Task Training in Semantic Segmentation and Object Detection."</p>
        <p class="ac-tl-venue">Oral &amp; Poster Presentation</p>
      </div>
    </li>
    <li>
      <span class="ac-tl-date">26 Jun 2024</span>
      <div>
        <p class="ac-tl-title"><span class="ac-badge badge-venue">CyPhyss 2024</span> IISc, India</p>
        <p class="ac-tl-paper">"MRFP: Learning Generalizable Semantic Segmentation from Sim-2-Real with Multi-Resolution Feature Perturbation."</p>
        <p class="ac-tl-venue">Oral Presentation</p>
      </div>
    </li>
    <li>
      <span class="ac-tl-date">15 May 2024</span>
      <div>
        <p class="ac-tl-title"><span class="ac-badge badge-venue">ICRA 2024</span> Yokohama, Japan</p>
        <p class="ac-tl-paper">"SKD-Net: Spectral-based Knowledge Distillation in Low-Light Thermal Imagery for Robotic Perception."</p>
        <p class="ac-tl-venue">Oral Presentation</p>
      </div>
    </li>
  </ul>
</div>

<!-- ═══════════════════════════════════════ -->
<!--  TALKS & TUTORIALS                      -->
<!-- ═══════════════════════════════════════ -->
<div class="ac-section">
  <h2>🎤 Talks &amp; Tutorials</h2>
  <div class="ac-scroll-box">
  <ul class="ac-timeline">
    <li>
      <span class="ac-tl-date">30 Jan 2026</span>
      <div>
        <p class="ac-tl-title"><span class="ac-badge badge-venue">IIT Bombay</span> Maharashtra, India</p>
        <p class="ac-tl-paper">"Development of Robust Perception Systems for Real-World Applications."</p>
        <p class="ac-tl-venue">Machine Learning for Remote Sensing II</p>
      </div>
    </li>
    <li>
      <span class="ac-tl-date">20 Aug 2025</span>
      <div>
        <p class="ac-tl-title"><span class="ac-badge badge-venue">ETAAV 2025</span> IISc Bangalore, India</p>
        <p class="ac-tl-paper">"AI-Driven Perception for UAVs under Adverse Weather."</p>
      </div>
    </li>
    <li>
      <span class="ac-tl-date">21 Aug 2025</span>
      <div>
        <p class="ac-tl-title"><span class="ac-badge badge-venue">Atria Institute of Technology</span> Bangalore, India</p>
        <p class="ac-tl-paper">"AI-Driven Personalized Learning: Transforming Education with Generative Models."</p>
        <p class="ac-tl-venue">Faculty Development Program – Exploring Generative AI</p>
      </div>
    </li>
    <li>
      <span class="ac-tl-date">12 Feb 2025</span>
      <div>
        <p class="ac-tl-title"><span class="ac-badge badge-venue">Dept. of Aerospace Engg., IISc</span> Bangalore, India</p>
        <p class="ac-tl-paper">"Advancing Drone Perception: Multi-Spectral Learning for Segmentation and Detection."</p>
        <p class="ac-tl-venue">Faculty Development Program – AI-Driven Autonomous Drone</p>
      </div>
    </li>
    <li>
      <span class="ac-tl-date">29 Jan 2025</span>
      <div>
        <p class="ac-tl-title"><span class="ac-badge badge-venue">Lossfunk Residency</span> Bangalore, India</p>
        <p class="ac-tl-paper">"Domain Generalization for Autonomous Navigation."</p>
        <p class="ac-tl-venue">Invited Talk (formerly Turing's Dream)</p>
      </div>
    </li>
    <li>
      <span class="ac-tl-date">26 Jun 2024</span>
      <div>
        <p class="ac-tl-title"><span class="ac-badge badge-venue">PES University</span> Karnataka, India</p>
        <p class="ac-tl-paper">"Target Recognition in Aerial Imagery: Current Trends and Challenges."</p>
        <p class="ac-tl-venue">Faculty Development Program – Drone Perception</p>
      </div>
    </li>
    <li>
      <span class="ac-tl-date">22 Feb 2024</span>
      <div>
        <p class="ac-tl-title"><span class="ac-badge badge-venue">Dept. of Aerospace Engg., IISc</span> Bangalore, India</p>
        <p class="ac-tl-paper">"Deep Learning for Autonomous Navigation."</p>
        <p class="ac-tl-venue">Industrial Workshop for Ashok Leyland – Autonomous Navigation</p>
      </div>
    </li>
    <li>
      <span class="ac-tl-date">09 Jan 2024</span>
      <div>
        <p class="ac-tl-title"><span class="ac-badge badge-venue">Dept. of Aerospace Engg., IISc</span> Bangalore, India</p>
        <p class="ac-tl-paper">"Deep Learning for Drone Applications."</p>
        <p class="ac-tl-venue">Faculty Development Program – Drone Applications</p>
      </div>
    </li>
    <li>
      <span class="ac-tl-date">16 Sep 2023</span>
      <div>
        <p class="ac-tl-title"><span class="ac-badge badge-venue">Dept. of Aerospace Engg., IISc</span> Bangalore, India</p>
        <p class="ac-tl-paper">"AI Perception for Aerial Robotics."</p>
        <p class="ac-tl-venue">Faculty Development Program – UAV Technology and Applications</p>
      </div>
    </li>
  </ul>
  </div>
</div>

<!-- ═══════════════════════════════════════ -->
<!--  TEACHING ACTIVITIES                    -->
<!-- ═══════════════════════════════════════ -->
<div class="ac-section">
  <h2>📚 Teaching Activities</h2>
  <p class="ac-section-desc">Courses where I served as Co-Principal Investigator or Teaching Assistant.</p>

  <!-- NPTEL Courses -->
  <h3 style="font-size:1rem; font-weight:600; margin: 1.2rem 0 0.6rem; color: var(--global-text-color);">NPTEL Courses</h3>

  <div class="ac-course">
    <div class="ac-course-header">
      <span class="ac-course-num">COURSE 01</span>
      <h3>AI-Driven Perception, Learning and Mapping for Drones</h3>
    </div>
    <div class="ac-course-body">
      <p>
        <span class="ac-badge badge-role-copi">Co-Principal Investigator</span>
        <a href="https://onlinecourses.nptel.ac.in/e-learning/preview/noc26_ee96" target="_blank">NPTEL ↗</a>
        &nbsp;·&nbsp;
        <a href="https://www.youtube.com/watch?v=tQ7kX5Xpf70&list=PLgMDNELGJ1CZZLI8nL0sDXJ6vPOj5p4Hv&index=15" target="_blank">YouTube ↗</a>
      </p>
      <ul>
        <li>Co-developed and delivered this NPTEL course on AI-driven perception and mapping for autonomous drones.</li>
        <li>Covered multi-spectral perception, domain adaptation, semantic segmentation, object detection, and SLAM for UAVs.</li>
        <li>Managed content preparation, assignments, and learner engagement.</li>
      </ul>
    </div>
  </div>

  <div class="ac-course">
    <div class="ac-course-header">
      <span class="ac-course-num">COURSE 02</span>
      <h3>Advanced Perception for Autonomous Systems</h3>
    </div>
    <div class="ac-course-body">
      <p><span class="ac-badge badge-role-copi">Co-Principal Investigator</span></p>
      <p class="ac-course-placeholder">Details coming soon. This course will cover advanced topics in visual perception, multi-modal sensing, and deep learning for autonomous robotic systems.</p>
    </div>
  </div>

  <!-- TA Course -->
  <h3 style="font-size:1rem; font-weight:600; margin: 1.4rem 0 0.6rem; color: var(--global-text-color);">Graduate Courses</h3>

  <div class="ac-card">
    <div class="ac-card-title">Neural Computation</div>
    <div class="ac-card-meta">
      <span class="ac-badge badge-role-ta">Teaching Assistant</span>
      Department of Aerospace Engineering, IISc &nbsp;·&nbsp; Aug 2023 – 2024
    </div>
    <ul>
      <li>TA for the graduate-level course on <strong>Neural Computation</strong>.</li>
      <li>Conducted tutorials on deep learning, backpropagation, optimization, and neural architectures.</li>
      <li>Assisted with assignments, project mentoring, and evaluation.</li>
    </ul>
  </div>
</div>
