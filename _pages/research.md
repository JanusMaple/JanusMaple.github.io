---
layout: page
title: research
permalink: /research/
nav: true
nav_order: 2
---

<style>
  .post-header {
    display: none;
  }

  .research-heading {
    display: block;
  }

  .research-badge {
    display: inline-block;
    white-space: nowrap;
    margin-left: 0.4rem;
    padding: 0.12rem 0.45rem;
    font-size: 0.78rem;
    font-weight: 500;
    line-height: 1.2;
    color: var(--global-theme-color) !important;
    border: 1px solid var(--global-theme-color);
    border-radius: 0.3rem;
    text-decoration: none !important;
    vertical-align: middle;
  }

  .research-badge:hover {
    color: white !important;
    background: var(--global-theme-color);
  }
</style>

<h2 class="research-heading">
  <span>FoMo-FD: Flow-Matching World Models for Surgical Robot Failure Detection</span>
  <a
    class="research-badge"
    href="https://arxiv.org/abs/2607.27511"
    target="_blank"
    rel="noopener noreferrer"
  >Preprint ↗</a>
</h2>

_Feb 2026 – Jul 2026_

<video
autoplay
muted
loop
playsinline
preload="metadata"
style="width: 48%; float: right; margin-left: 0.5rem; margin-bottom: 0.5rem; border-radius: 3px;"

>

  <source src="/assets/video/FoMoFD.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

This project studied **runtime detection of low-level execution failures in surgical robot imitation policies without requiring failure data for training**. Rather than assuming predefined failure types, we detect whether the realized visual dynamics over a recent execution window deviate from the nominal dynamics expected under the commanded actions.

I developed **FoMo-FD**, an action-conditioned flow-matching latent world model that predicts visual dynamics over temporal windows. Failure signals are obtained through **inverse transport** between expected and observed dynamics, with detection thresholds determined by **conformal calibration**.

<p style="font-size: 0.9rem; color: #666;">
  <strong>Z. Huang</strong>, Y. Cai, A. Patel, M. Hajiha, B. Browne, and Y. Chen,
  “Failure Detection for Surgical Robot Imitation Policies via Flow-Matching World Modeling,”
  <em>arXiv preprint arXiv:2607.27511</em>, 2026. 
</p>

<div style="clear: both;"></div>

<h2 class="research-heading">
  <span>Autonomous Self-Reconfiguration Planning for Continuum Modular Robots</span>
  <a
    class="research-badge"
    href="https://doi.org/10.1126/sciadv.aeg9191"
    target="_blank"
    rel="noopener noreferrer"
  >Paper ↗</a>
</h2>

_Apr 2025 – Jan 2026_

<video
autoplay
muted
loop
playsinline
preload="metadata"
style="width: 48%; float: right; margin-left: 0.5rem; margin-bottom: 0.5rem; border-radius: 3px;"

>

  <source src="/assets/video/MSRCR.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

This project studied **autonomous self-reconfiguration of modular self-reconfigurable continuum robots (MSRCR)**, where planning must jointly reason over discrete configuration changes and continuous deformation while maintaining physical feasibility.

I developed a **geometric and topological representation of robot configurations** and formulated self-reconfiguration as a task and motion planning problem over configuration manifolds and reconfiguration actions. Based on this formulation, I proposed **HEART-MCTS** for hierarchical task planning and integrated **Atlas-RRT\*** for motion planning within constriant manifolds.

This was a really fun collaboration with [Yilin Cai](https://missinglight.github.io/) that led to our [paper](https://doi.org/10.1126/sciadv.aeg9191) in _Science Advances_.

<p style="font-size: 0.9rem; color: #666;">
  Y. Cai*, <strong>Z. Huang*</strong>, Y. Wang, H. Xu, and Y. Chen,
  “Evolutionary Diversification via Modular Compliance for Self-Reconfigurable Continuum Robots,”
  <em>Science Advances</em>, vol. 12, eaeg9191, 2026.
  *These authors contributed equally to this work.
</p>

<div style="clear: both;"></div>

<h2 class="research-heading">
  Teleoperated Mobile Nursing Robot in the Intensive Care Unit
</h2>

_Apr 2024 – Oct 2024_

<video
autoplay
muted
loop
playsinline
preload="metadata"
style="width: 40%; float: right; margin-left: 2rem; margin-bottom: 1rem; border-radius: 6px;"

>

  <source src="/assets/video/icu_robot.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

This project explored the use of a **mobile manipulator for assisting nursing tasks in an intensive care unit (ICU)**. We deployed a Stretch 2 robot in a clinical environment and recorded demonstrations of representative nursing workflows for an HRI study.

I developed a **custom teleoperation interface** and conducted teleoperated task demonstrations in the ICU. The study investigated **nurses’ perceptions and acceptance of robotic assistance** in workflows.

<div style="clear: both;"></div>

<h2 class="research-heading">
  Ultrasound-Guided Robotic Needle Insertion
</h2>

_Sep 2023 – Jan 2024_

<video
autoplay
muted
loop
playsinline
preload="metadata"
style="width: 42%; float: right; margin-left: 2rem; margin-bottom: 1rem; border-radius: 6px;"

>

  <source src="/assets/video/Ultrasound_Guided_Needle_Insertion_square.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

Ultrasound-guided robotic needle insertion can improve targeting in minimally invasive procedures. This preliminary study explored the **feasibility of integrating robotic needle insertion, ultrasound imaging, and respiratory motion simulation** in a single experimental setup.

I built a **dual-arm robotic needle insertion system** together with an XY motion platform to emulate respiratory motion, and conducted insertion experiments during periods of relative target quiescence. The prototype was used to validate the overall experimental workflow.

<div style="clear: both;"></div>

<h2 class="research-heading">
  <span>Body-Mounted MR-Conditional Robot for Minimally Invasive Liver Intervention</span>
  <a
    class="research-badge"
    href="https://doi.org/10.1007/s10439-024-03503-2"
    target="_blank"
    rel="noopener noreferrer"
  >Paper ↗</a>
</h2>

_Jan 2023 – Sep 2023_

<img src="/assets/img/research/mr_liver_robot.jpg"
     alt="Body-mounted MR-conditional robot"
     style="width: 42%; float: right; margin-left: 2rem; margin-bottom: 1rem;">

MRI-guided liver interventions require accurate needle positioning within the highly constrained bore of a closed-bore MRI scanner. This project developed a **body-mounted four-DOF MR-conditional robot** for minimally invasive liver intervention.

I designed and integrated the **mechanical structure and mechatronic control system**, including a two-layer positioning mechanism and pneumatic actuation. I also performed kinematic modeling, workspace analysis, and experimental validation of the system.

<p style="font-size: 0.9rem; color: #666;">
  <strong>Z. Huang</strong>, A. L. Gunderman, S. E. Wilcox, S. Sengupta, J. Shah, A. Lu, D. Woodrum, and Y. Chen,
  “Body-Mounted MR-Conditional Robot for Minimally Invasive Liver Intervention,”
  <em>Annals of Biomedical Engineering</em>, vol. 52, no. 8, pp. 2065–2075, 2024.
</p>

<div style="clear: both;"></div>

<h2 class="research-heading">
  <span>Optimal Geometric Design of Concentric Tube Robots for Intracerebral Hemorrhage Removal</span>
  <a
    class="research-badge"
    href="https://doi.org/10.1115/1.4063979"
    target="_blank"
    rel="noopener noreferrer"
  >Paper ↗</a>
</h2>

_Sep 2022 – Jan 2023_

<img src="/assets/img/research/optimal_ctr_design.png"
     alt="Optimal concentric tube robot design"
     style="width: 36%; float: right; margin-left: 2rem; margin-bottom: 1rem;">

Intracerebral hemorrhage evacuation requires reaching deep targets while avoiding critical anatomical structures. This project investigated the **optimal geometric design of concentric tube robots** for safe access to hemorrhage regions.

I developed **geometric models and optimization methods** for concentric-tube robot design, representing tube shapes using parameterized helices and optimizing robot configurations under anatomical constraints.

<p style="font-size: 0.9rem; color: #666;">
  <strong>Z. Huang</strong>, H. Alkhars, A. Gunderman, D. Sigounas, K. Cleary, and Y. Chen,
  “Optimal Concentric Tube Robot Design for Safe Intracerebral Hemorrhage Removal,”
  <em>Journal of Mechanisms and Robotics</em>, vol. 16, no. 8, 081005, 2024.
</p>

<div style="clear: both;"></div>
