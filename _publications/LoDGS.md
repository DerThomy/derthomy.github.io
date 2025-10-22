---
title: "LoD of Gaussians: Unified Training and Rendering for Ultra-Large Scale Reconstruction with External Memory"
collection: publications
category: arxiv
permalink: /publication/LOD-Gaussians
excerpt: 'Enables abitrary scene scale for Gaussian Splatting reconstruction on single consumer GPU.'
date: 2025-07-01
venue: 'ArXiv'
paperurl: 'https://arxiv.org/pdf/2507.01110'
citation: 'Felix Windisch, Thomas Köhler, Lukas Radl, Michael Steiner, Dieter Schmalstieg, Markus Steinberger (2025). &quot;LoD of Gaussians: Unified Training and Rendering for Ultra-Large Scale Reconstruction with External Memory.&quot; <i>ArXiv</i>.'
---
Gaussian Splatting has emerged as a high-performance technique for novel view synthesis, enabling real-time rendering and high-quality reconstruction of small scenes. However, scaling to larger environments has so far relied on partitioning the scene into chunks -- a strategy that introduces artifacts at chunk boundaries, complicates training across varying scales, and is poorly suited to unstructured scenarios such as city-scale flyovers combined with street-level views. Moreover, rendering remains fundamentally limited by GPU memory, as all visible chunks must reside in VRAM simultaneously. We introduce A LoD of Gaussians, a framework for training and rendering ultra-large-scale Gaussian scenes on a single consumer-grade GPU -- without partitioning. Our method stores the full scene out-of-core (e.g., in CPU memory) and trains a Level-of-Detail (LoD) representation directly, dynamically streaming only the relevant Gaussians. A hybrid data structure combining Gaussian hierarchies with Sequential Point Trees enables efficient, view-dependent LoD selection, while a lightweight caching and view scheduling system exploits temporal coherence to support real-time streaming and rendering. Together, these innovations enable seamless multi-scale reconstruction and interactive visualization of complex scenes -- from broad aerial views to fine-grained ground-level details.