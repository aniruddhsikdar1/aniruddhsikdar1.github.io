---
layout: page
permalink: /teaching/
title: Academic Activities
description: Talks, paper presentations, conferences, and teaching activities.
nav: true
nav_order: 6
---

Paper presentations can also be found on the [AIRL YouTube Page](https://www.youtube.com/@airl_iisc).

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Academic Activities</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            padding: 20px;
            font-family: 'Poppins', sans-serif;
            background: #ffffff;
            color: #111111;
        }
        .container {
            max-width: 900px;
            margin: 0 auto;
        }
        h1 {
            color: #111111;
            font-size: 2rem;
            margin-bottom: 30px;
        }
        .card {
            padding: 20px 24px;
            border-radius: 12px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.07);
            margin-bottom: 25px;
            transition: all 0.3s ease;
        }
        .card h2 {
            margin-top: 0;
            font-weight: 700;
            font-size: 1.35rem;
            color: #111111;
        }
        .card p {
            color: #111111;
            line-height: 1.6;
            font-size: 1rem;
        }
        .card p strong {
            color: #1f6feb;
        }
        .card ul {
            padding-left: 20px;
            line-height: 1.6;
            color: #111111;
        }
        .card a.button {
            display: inline-block;
            margin-top: 12px;
            padding: 10px 20px;
            color: white;
            text-decoration: none;
            border-radius: 6px;
            font-weight: 600;
            font-size: 0.95rem;
            transition: background 0.3s;
        }
        .card-blue {
            background: #f0f4ff;
            border-left: 5px solid #1f6feb;
        }
        .card-blue a.button {
            background: #1f6feb;
        }
        .card-orange {
            background: #fff7f0;
            border-left: 5px solid #e36209;
        }
        .card-orange a.button {
            background: #e36209;
        }
        .section-title {
            margin-top: 40px;
            font-size: 1.8rem;
            font-weight: 700;
            color: #111111;
            border-bottom: 2px solid #1f6feb;
            padding-bottom: 8px;
            margin-bottom: 20px;
        }
        a {
            color: #1f6feb;
        }
    </style>
</head>
<body>
<div class="container">

    <h1>🏆 Competitions & Challenges</h1>

    <!-- ===== CARD 1 ===== -->
    <div class="card card-blue">
        <h2>📌 Multi-modal Domain Fusion for Multi-modal Aerial View Object Classification</h2>
        <p>
            <strong>Role:</strong> Participant <br>
            <strong>Event:</strong> MAVOC Challenge, CVPR-W PBVS 2022 <br>
            <strong>Team:</strong> 2 members
        </p>
        <ul>
            <li>Built a multi-modal aerial classification model using EO + SAR labeled and unlabeled data.</li>
            <li><strong>Track 1 (EO + SAR):</strong> Ranked <strong style="color:#1f6feb;">5th / 82</strong>.</li>
            <li><strong>Track 2 (SAR-only):</strong> Ranked <strong style="color:#1f6feb;">9th / 77</strong>.</li>
            <li>Published in <em>CVPR Workshops, PBVS 2022</em>.</li>
        </ul>
        <a href="https://arxiv.org/pdf/2212.07039" target="_blank" class="button">📄 View Paper (arXiv)</a>
    </div>

    <!-- ===== CARD 2 ===== -->
    <div class="card card-orange">
        <h2>🚁 UAV RGB–IR Slant Angle Object Detection Challenge</h2>
        <p>
            <strong>Role:</strong> Organizer <br>
            <strong>Event:</strong> International Conference on Emerging Technology in Autonomous Aerial Vehicles (ETAAV), IISc Bangalore <br>
            <strong>Sponsor:</strong> SwaYaan (MeitY)
        </p>
        <ul>
            <li>Organized India's first drone-based multi-spectral (RGB + IR) object detection competition.</li>
            <li>Designed and released the <strong>IndraEye</strong> dataset to accelerate multi-spectral perception research.</li>
            <li>Hosted as part of <strong>ETAAV 2025</strong> at IISc Bangalore.</li>
        </ul>
        <a href="https://www.kaggle.com/competitions/etaav-eo-ir/overview" target="_blank" class="button">🏆 View Challenge (Kaggle)</a>
    </div>

    <h2 class="section-title">🎤 Talks</h2>

    <!-- ===== TALKS CARDS ===== -->
    <div class="card card-blue">
        <h2>Tutorial: Advancing Drone Perception: Multi-Spectral Learning for Segmentation and Detection</h2>
        <p>
            <strong>Event:</strong> Faculty Development Program on AI-Driven Autonomous Drone, IISc Bangalore <br>
            <strong>Date:</strong> 12/02/2025
        </p>
    </div>

    <div class="card card-orange">
        <h2>Invited Talk: Domain generalization for autonomous navigation</h2>
        <p>
            <strong>Event:</strong> Lossfunk Residency (formerly Turing’s Dream), Bangalore, India <br>
            <strong>Date:</strong> 29/01/2025
        </p>
    </div>

    <div class="card card-blue">
        <h2>Tutorial: Target Recognition in Aerial Imagery: Current Trends and Challenges</h2>
        <p>
            <strong>Event:</strong> Faculty Development Program on Drone Perception, PES University, Karnataka, India <br>
            <strong>Date:</strong> 26/06/2024
        </p>
    </div>

    <div class="card card-orange">
        <h2>Talk: Deep Learning for Autonomous Navigation</h2>
        <p>
            <strong>Event:</strong> Industrial Workshop for Ashok Leyland, IISc Bangalore <br>
            <strong>Date:</strong> 22/02/2024
        </p>
    </div>

    <div class="card card-blue">
        <h2>Talk: Deep Learning for Drone Applications</h2>
        <p>
            <strong>Event:</strong> Faculty Development Program on Drone Applications, IISc Bangalore <br>
            <strong>Date:</strong> 09/01/2024
        </p>
    </div>

    <div class="card card-orange">
        <h2>Talk: AI Perception for Aerial Robotics</h2>
        <p>
            <strong>Event:</strong> Faculty Development Program on UAV Technology, IISc Bangalore <br>
            <strong>Date:</strong> 16/09/2023
        </p>
    </div>

    <h2 class="section-title">📄 Paper Presentations</h2>

    <!-- ===== PAPERS CARDS ===== -->
    <div class="card card-blue">
        <h2>SSL-RGB2IR: Semi-supervised RGB-to-IR Image-to-Image Translation for Enhancing Vision Task Training</h2>
        <p>
            <strong>Event:</strong> IROS 2024, Abu Dhabi, UAE <br>
            <strong>Date:</strong> 16/10/2024
        </p>
    </div>

    <div class="card card-orange">
        <h2>MRFP: Learning Generalizable Semantic Segmentation from Sim-2-Real with Multi-Resolution Feature Perturbation</h2>
        <p>
            <strong>Event:</strong> Cyber-Physical Systems Symposium (CyPhySS 2024), IISc, India <br>
            <strong>Date:</strong> 26/06/2024
        </p>
    </div>

    <div class="card card-blue">
        <h2>SKD-Net: Spectral-based Knowledge Distillation in Low-Light Thermal Imagery for Robotic Perception</h2>
        <p>
            <strong>Event:</strong> ICRA 2024, Yokohama, Japan <br>
            <strong>Date:</strong> 15/05/2024
        </p>
    </div>

    <h2 class="section-title">🎓 Courses</h2>

    <div class="card card-orange">
        <h2>Course: To be updated soon</h2>
        <p>
            Details will be added shortly.
        </p>
    </div>

</div>
</body>
</html>
