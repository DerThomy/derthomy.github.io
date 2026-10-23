---
title: 'Pi-GS: Sparse-View Gaussian Splatting with Dense π³ Initialization'
collection: publications
category: conferences
permalink: /publication/Pi-GS
excerpt: 3D Gaussian Splatting struggles in sparse-view settings where Structure-from-Motion
  point clouds are incomplete and camera poses are uncertain. We integrate dense,
  reference-free point cloud initialization from π³ with uncertainty-guided depth
  supervision, normal consistency loss, and depth warping, achieving state-of-the-art
  sparse reconstruction across multiple benchmark datasets.
date: 2026-02-09
venue: Proceedings of the 29th Computer Vision Winter Workshop (CVWW 2026)
paperurl: https://arxiv.org/pdf/2602.03327
citation: 'Manuel Hofer, Markus Steinberger, Thomas Köhler (2026). &quot;Pi-GS: Sparse-View
  Gaussian Splatting with Dense &pi;<sup>3</sup> Initialization.&quot; In <i>Proceedings
  of the 29th Computer Vision Winter Workshop (CVWW)</i>.'
authors: Manuel Hofer, Markus Steinberger, <strong>Thomas Köhler</strong>
---
Novel view synthesis has evolved rapidly, advancing from Neural Radiance Fields to 3D Gaussian Splatting (3DGS), which offers real-time rendering and rapid training without compromising visual fidelity. However, 3DGS relies heavily on accurate camera poses and high-quality point cloud initialization, which are difficult to obtain in sparse-view scenarios. While traditional Structure from Motion (SfM) pipelines often fail in these settings, existing learning-based point estimation alternatives typically require reliable reference views and remain sensitive to pose or depth errors.

In this work, we propose a robust method utilizing $\pi^3$, a reference-free point cloud estimation network. We integrate dense initialization from $\pi^3$ with a regularization scheme designed to mitigate geometric inaccuracies. Specifically, we employ uncertainty-guided depth supervision, normal consistency loss, and depth warping. Experimental results demonstrate that our approach achieves state-of-the-art performance on the Tanks and Temples, LLFF, DTU, and MipNeRF360 datasets.
