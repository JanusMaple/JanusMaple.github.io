---
layout: page
title: fun
permalink: /fun/
nav: true
nav_order: 3
---

<style>
  .post-header {
    display: none;
  }

  .fun-project-heading {
    display: block;
  }

  .fun-badge {
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

  .fun-badge:hover {
    color: white !important;
    background: var(--global-theme-color);
  }

  .fun-section-title {
    font-size: 1.3rem;
    font-weight: 600;
    color: #666;
    margin-top: 1.5rem;
    margin-bottom: 1rem;
    letter-spacing: 0.02em;
  }

    .fun-project-heading {
    font-size: 1.9rem;
    margin-top: 0;
    margin-bottom: 0.6rem;
  }
</style>

<h2 class="fun-section-title">Some Fun Projects</h2>

<h3 class="fun-project-heading">
  Local MCTS Motion Planning
  <a
    class="fun-badge"
    href="https://github.com/JanusMaple/MCTSMP"
    target="_blank"
    rel="noopener noreferrer"
  >Code ↗</a>
</h3>

<video
autoplay
muted
loop
playsinline
preload="metadata"
style="width: 48%; float: right; margin-left: 0.8rem; margin-bottom: 0.5rem; border-radius: 3px;"

>

  <source src="/assets/video/MCTS_Plan.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

A small project I built for my Robotics Ph.D. qualifying exam. I explored **local motion planning with passively deformable obstacles**, where limited contact may be useful rather than treated as an immediate collision.

I implemented an **MCTS-based local planner for a non-holonomic mobile robot**. In the simplified prototype, the robot can push an obstacle while exploring a route, continue if the path opens, or **retreat and replan when the deformation limit is reached**. The idea was motivated by settings such as ICUs, where objects like tubing may tolerate limited contact but hazardous deformation should be avoided.

<div style="clear: both;"></div>

<h3 class="fun-project-heading">
  Procedural Trees & Creatures
</h3>

_[CS 8803: Procedural Content Generation](https://faculty.cc.gatech.edu/~turk/pcg/index.html) · [Prof. Greg Turk](https://faculty.cc.gatech.edu/~turk/)_

<video
autoplay
muted
loop
playsinline
preload="metadata"
style="width: 24%; float: right; margin-left: 1rem; margin-bottom: 0.5rem; border-radius: 3px;"

>

  <source src="/assets/video/PCG.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

Two course projects exploring **procedural content generation** in **Unity**. For trees, I implemented randomized growth rules supporting **willow-like, plagiotropic, and orthotropic structures**, with controllable branching, tropism, leaf layouts, and age-dependent growth. I also added **obstacle-aware generation**, allowing branches to adapt their growth around geometric obstacles.

For creatures, I used the **Marching Cubes algorithm** to generate continuous meshes with shared vertices for smooth normals and color transitions. Random seeds vary body proportions, colors, eyes, and accessories, including animated halos, horns, and eye styles. The torso and legs form a single mesh. And I do think they are very cute.

<div style="clear: both;"></div>

<h2 class="fun-section-title">A Few Other Things</h2>

More coming soon.
