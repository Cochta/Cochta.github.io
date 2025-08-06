---
title: SPH Fluid Simulation
publishDate: 2025-06-05 00:00:00
img: /assets/SPH.gif
img_alt: Prototype iamge
description: |
  I developed an SPH Fluid Simulation for my Bachelor Project
tags:
  - Bachelor
  - SPH
  - C++
  - Compute Shader
---

### Overview

This project is a **real-time 3D fluid simulation** using the **Smoothed Particle Hydrodynamics (SPH)** method. Implemented **from scratch** in **C++**, the simulation models fluid behavior by representing water as a collection of particles that interact through **pressure**, **viscosity**, and **external forces**. Particles are accelerated using **force computations** derived from SPH equations and integrated over time using a stable numerical solver.

To optimize neighbor searches, the simulation uses a **Spatial Hash Grid**, enabling efficient retrieval of nearby particles per frame. The simulation runs at **60 FPS with 1000 particles** on a **single-threaded CPU**. The simulation is integrated into "[**Bark**](/work/nested/bark)" my own **physics engine**.

The simulation now runs on a **compute shader**, offloading particle computations to the **GPU** for a massive **performance boost**. This upgrade enables **real-time** performance with **thousands of particles**, opening the door to more complex and visually rich fluid behavior.

The **compute shader implementation** was developed with the support of **fellow Games Programming student at SAE Institute Geneva Olivier Pachoud**, who specialized in raytraced rendering and used my fluid simulation. 
[Click here to view his project](https://chocolive24.github.io/project/bachelors-project-fluid-simulation-raytracing-rendering/)

### How it looks like

Here is a gif of the **monothreaded CPU** simulation with 1'200 particles:

<img alt="gif cpu 1200 particles" width="100%" src="/assets/SPH.gif" />

Here is a gif of the **compute shader** simulation with 40'000 particles:

<img alt="gif gpu 40k particles" width="100%" src="/assets/40k.gif" />

### Bachelor's thesis

  <iframe src="/assets/ConstantinVerineBachelorOfScience.pdf#navpanes=0&toolbar=1&statusbar=1&view=Fit" width="100%" height="800px"></iframe>


### What did I learn

- **Smoothed Particle Hydrodynamics (SPH)**: Gained a deep understanding of SPH principles, including **density estimation**, **pressure** and **viscosity** forces.

- **Spatial Hash Grid**: Implemented an efficient **spatial partitioning system** to accelerate neighbor searches in large particle sets.

- **Numerical Stability**: Learned to prevent instability in particle simulations by carefully tuning parameters and using stable integration methods.

- **Performance Profiling**: Analyzed and optimized CPU performance to maintain real-time frame rates.

- **Parallel Computation**: Transitioned physics computations to GPU via **compute shaders** to support larger-scale simulations.

- **Engine Integration**: Embedded the simulation within my **own physics engine** "[**Bark**](/work/nested/bark)", improving modularity and system-level understanding of engine architecture.

### Source Code & Download

- [Download my CPU SPH Fluid simulation ](https://github.com/Cochta/Bark3D/releases/download/SPH_V1.0/SPHFluidSimulationScene.zip)
- [GitHub Repository of the 3D physics engine](https://github.com/Cochta/Bark3d)