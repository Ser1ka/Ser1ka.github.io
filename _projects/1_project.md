---
layout: page
title: "Hybrid Legged Locomotion: CPG + Deep RL"
description: An end-to-end framework integrating Central Pattern Generators with DRL for an 18-DOF Hexapod, successfully deployed via a custom low-bandwidth binary protocol.
img: assets/img/hexapod_thumb.jpg # The cover image shown on your main projects page
importance: 1
category: research
related_publications: false
---

<div class="row justify-content-sm-center">
    <div class="col-sm-10 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/hexapod_main.gif" title="Hexapod Locomotion Demo" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 1: The finalized Hybrid CPG-DRL locomotion policy deployed on the virtual environment (Isaac Gym/Gazebo) and transferred onto the physical 18-DOF bare-metal hexapod platform.
</div>

## Overview
Controlling an **18-degree-of-freedom (DOF) hexapod robot** in unstructured and unpredictable environments introduces severe high-dimensionality and control challenges. Traditional model-based predictive control requires heavy computational resources, while pure model-free reinforcement learning (RL) suffers from extreme sample inefficiency and often converges to erratic, unstable local minima.

To address these limitations, this project implements a novel **hybrid locomotion framework** that couples biologically inspired **Central Pattern Generators (CPG)** with a **Deep Reinforcement Learning (DRL)** agent. By injecting a structural biological prior, we reduce the required exploration space and guarantee mechanical stability during training.

---

## Technical Framework & Methodology

<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/hexapod_arch.jpg" title="System Architecture" class="img-fluid rounded z-depth-1" %}
        <div class="caption">System Architecture combining Hopf Oscillators and DRL Policy.</div>
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/hexapod_curriculum.jpg" title="Curriculum Learning Stages" class="img-fluid rounded z-depth-1" %}
        <div class="caption">Multi-stage curriculum learning environment setups.</div>
    </div>
</div>

1. **CPG Foundation (Hopf Oscillators):** Utilized a network of coupled differential equations to provide a structurally stable, rhythmic foundational walking pattern (tripod gait), avoiding the blind joint kinematics exploration typical of vanilla RL.
2. **DRL Policy Modulation:** Designed a policy network that observes a **29-dimensional state space** (including chassis attitude and oscillator phases) and outputs dynamic modulation signals to adjust the stepping rate and joint offsets.
3. **Multi-Stage Curriculum Learning:** Progressively trained the agent in virtual simulation across flat ground, undulating terrain, and fields populated with physical obstacles to guarantee smooth reward convergence.

---

## Key Performance Metrics (Simulation vs. Baseline)

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/hexapod_curves.jpg" title="Training Convergence Curves" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<br>

* **Convergence Rate:** Achieved **XX% faster reward convergence** compared to pure model-free RL baselines (PPO/SAC) by utilizing CPG priors.
* **Energy Efficiency:** Generated highly symmetrical and stable tripod gaits, reducing the mechanical cost of transport (CoT) by **XX%**.
* **Terrain Adaptability:** Maintained stable chassis velocity and orientation on uneven surfaces without stumbling.

---

## Sim-to-Real: Overcoming the Embedded Communication Bottleneck

Deploying a high-frequency control policy from virtual simulation onto a physical Arduino-driven hardware platform presented severe hardware limitations, most notably a **strict 9600-baud serial communication bottleneck** between the upper-level PC controller and the lower-level servo driver.

<div class="row justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/hexapod_hardware.jpg" title="Hardware Implementation" class="img-fluid rounded z-depth-1" %}
        <div class="caption">Real 18-DOF hardware testing platform with onboard IMU.</div>
    </div>
</div>

To achieve real-time, closed-loop control under these extreme physical constraints:
* **Custom Binary Protocol:** Engineered a highly optimized bidirectional binary communication protocol.
* **Aggressive Data Compression:** Compressed continuous sensor feedback and absolute 18-joint commands into a dense **40-byte data frame**.
* **Deterministic Execution:** Successfully maintained a stable, loss-free **10 Hz control loop** without data dropouts or buffer overflows, relying entirely on onboard IMU feedback.

Ultimately, physical testing validated that modulating rhythmic structural priors with deep reinforcement learning offers a highly viable, computationally efficient solution for complex legged locomotion in real-world scenarios.

---

```html
<div class="projects-tags">
    <strong>Technologies Used:</strong> 
    <span class="badge badge-primary">PyTorch</span>
    <span class="badge badge-secondary">Reinforcement Learning (PPO/SAC)</span>
    <span class="badge badge-success">Robot Locomotion</span>
    <span class="badge badge-warning">C++</span>
    <span class="badge badge-info">Arduino / Embedded C</span>
    <span class="badge badge-dark">Sim-to-Real</span>
</div>