---
title: Bark Physics Engine
publishDate: 2023-12-01 00:00:00
img: /assets/bark.gif
img_alt: Image of the collision scene
description: |
  I developed a 2D physics engine from scratch with triggers, collisions and space subdivision
tags:
  - C++
  - Physics
  - Quadtree
  - Optimisation
---

### Overview

This **physics engine** was **developed** as part of a module covering **physics**, **mathematics**, **optimization**, **CPU architecture**, and **profiling** during the **second year of a Bachelor's degree** in **Games Programming** at SAE Institute Geneva.

The primary objective was to design the **engine** as a **user-friendly API** while **optimizing** its **performance**. A key requirement was ensuring that the engine could **run a sample scene** with 1,000 colliders in trigger mode at a minimum of **60 FPS**.

To achieve this, **I implemented a custom mathematics library** (done with the help of my classmates) and **developed essential C++ utilities**, including **smart pointers**, allowing me to **integrate custom memory allocators** for **profiling** and **optimizing memory management**.

Later, I extended the engine to support **3D physics** and rendering, transitioning from my custom math library to **DirectXMath** for better performance and **SIMD-optimized** vector operations.

### How it looks like

Here is video of both 2D and 3D physics engine

<iframe width="100%" height="460" src="/assets/bark.mp4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

**Here is demo of the 2D physics engine you can test.**

<iframe frameborder="0" src="https://itch.io/embed-upload/9975414?color=bababa" allowfullscreen="" width="100%" height="820"><a href="https://cochta.itch.io/bark-demo">Play Bark Demo on itch.io</a></iframe>

### What did I learn

- Basics of **Calculus**
- Basics of **Linear Algebra**
- Basics of **Physics**
- Choose and use the right **C++ data structures** in a given context
- **Low level C++ API** programming
- Template programming
- Writing **custom allocators**
- **Profiling** code and **memory management**
- **Optimisation** tricks
  - Padding
  - Memory layout
  - Cache hit
  - **Quadtree** then **Octree**
- How a **modern CPU works**

### Source Code & Download

- [2D Physics Engine GitHub Repository](https://github.com/Cochta/Bark)
- [3D Physics Engine GitHub Repository](https://github.com/Cochta/Bark3D)
- [2D Physics Engine Download link](https://github.com/Cochta/Bark/releases/download/1.0/SamplesRelease.zip)
- [Test it on my Itch.io page](https://cochta.itch.io/bark-demo)