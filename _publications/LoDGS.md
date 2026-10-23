---
title: 'A LoD of Gaussians: Out-of-Core Training and Rendering for Seamless Ultra-Large
  Scene Reconstruction'
collection: publications
category: conferences
permalink: /publication/LOD-Gaussians
excerpt: Scaling 3D Gaussian Splatting to ultra-large environments typically requires
  spatial chunking, creating visible boundary seams and memory bottlenecks. We present
  an out-of-core Level-of-Detail (LoD) framework combining hierarchical Gaussians
  with Sequential Point Trees, enabling dynamic streaming and real-time rendering
  from broad aerial overviews to street-level details on a single consumer GPU.
date: 2026-07-19
venue: ACM SIGGRAPH 2026 Conference Papers
paperurl: https://arxiv.org/pdf/2507.01110
projecturl: https://felixwindisch.github.io/ALoDOfGaussians/
citation: 'Felix Windisch, Thomas Köhler, Lukas Radl, Mattia D&#39;Urso, Michael Steiner,
  Dieter Schmalstieg, Markus Steinberger (2026). &quot;A LoD of Gaussians: Out-of-Core
  Training and Rendering for Seamless Ultra-Large Scene Reconstruction.&quot; In <i>ACM
  SIGGRAPH 2026 Conference Papers</i>. <a href="https://doi.org/10.1145/3799902.3811076">doi:10.1145/3799902.3811076</a>'
header:
  teaser: publications/lodgs.mp4
authors: Felix Windisch, <strong>Thomas Köhler</strong>, Lukas Radl, Mattia D'Urso,
  Michael Steiner, Dieter Schmalstieg, Markus Steinberger
---
Gaussian Splatting has emerged as a high-performance technique for novel view synthesis, enabling real-time rendering and high-quality reconstruction of small scenes. However, scaling to larger environments has so far relied on partitioning the scene into chunks -- a strategy that introduces artifacts at chunk boundaries, complicates training across varying scales, and is poorly suited to unstructured scenarios such as city-scale flyovers combined with street-level views. Moreover, rendering remains fundamentally limited by GPU memory, as all visible chunks must reside in VRAM simultaneously. We introduce A LoD of Gaussians, a framework for training and rendering ultra-large-scale Gaussian scenes on a single consumer-grade GPU -- without partitioning. Our method stores the full scene out-of-core (e.g., in CPU memory) and trains a Level-of-Detail (LoD) representation directly, dynamically streaming only the relevant Gaussians. A hybrid data structure combining Gaussian hierarchies with Sequential Point Trees enables efficient, view-dependent LoD selection, while a lightweight caching and view scheduling system exploits temporal coherence to support real-time streaming and rendering. Together, these innovations enable seamless multi-scale reconstruction and interactive visualization of complex scenes -- from broad aerial views to fine-grained ground-level details.