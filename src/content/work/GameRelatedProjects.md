---
title: Game Related Projects
publishDate: 2019-10-02 00:00:00
img: /assets/EcoPars.gif
img_alt: Economy parser gif
description: |
  I’ve developed several tools and utilities to support gameplay analytics and content generation.
tags:
  - C++
  - Python
  - Emscripten
  - Parsing
---

### Overview

These game-related tools and parsers were developed as personal projects during my studies to support game balancing, data visualization, and server management.

I created a **player stats parser** that reads Minecraft’s stats.json files, translates raw data into readable French names, and generates **leaderboards** with emoji-based **ranking and tie handling**.

To better understand and analyze the economy of custom Minecraft minigames, I developed a **sales and economy parser** in **C++**, a less conventional choice for this type of project, but a valuable challenge which I compiled to **WebAssembly using Emscripten** for web deployment. To optimize loading times and reduce the overall project size, I implemented an **image atlas generator** in **Python** that batch-packs assets and generates metadata for use in real-time applications.

### How it looks like

##### Economy Parser

Here is a gif:

<img alt="Small gif" width="100%" src="/assets/EcoPars.gif" />

Try it out on itch.io

<iframe frameborder="0" src="https://itch.io/embed/3534450?bg_color=838383&amp;fg_color=000000&amp;link_color=FFD700&amp;border_color=000000" width="100%" height="200"><a href="https://cochta.itch.io/economy-parser">Economy Parser by Cochta</a></iframe>

##### Image atlas generator

<img alt="input folder" width="100%" src="/assets/ressources/ressourceGameRelated/ImgFolder.PNG" />
<p style="text-align:center">Input folder</p>
</br>
<img alt="input folder" width="100%" src="/assets/ressources/ressourceGameRelated/atlas.png" />
<p style="text-align:center">Output file</p>

##### Player stats parser

<img alt="input file" width="100%" src="/assets/ressources/ressourceGameRelated/StatBrut.PNG" />
<p style="text-align:center">Input .json file</p>
</br>
<img alt="input discord message" width="100%" src="/assets/ressources/ressourceGameRelated/StatFinal.PNG" />
<p style="text-align:center">Output discord message sent via webhook</p>

### What did I learn

- **Practical experience with data parsing and transformation**, especially from JSON and CSV formats.

- **Improved understanding of game telemetry and balancing**, through hands-on analysis of in-game statistics and economic data.

- **Deepened my C++ skills** by applying them to an unconventional context (web-based tooling) and adapting code for WebAssembly using Emscripten.

- **Learned about asset optimization techniques**, such as packing sprites into image atlases to reduce project size and improve load times.

### Source Code & Links

- [Economy Parser GitHub Repository](https://github.com/Cochta/Economy-Parser)
- [Economy Parser itch.io Link](https://cochta.itch.io/economy-parser)