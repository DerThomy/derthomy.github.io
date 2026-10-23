---
title: 'AAA-Gaussians: Anti-Aliased and Artifact-Free 3D Gaussian Rendering'
collection: publications
category: conferences
permalink: /publication/AAA-Gaussians
excerpt: Standard 3D Gaussian Splatting relies on screen-space 2D approximations that
  suffer from severe aliasing, popping, and projection distortions during dynamic
  camera motion. We introduce a fully 3D evaluation and filtering pipeline with adaptive
  3D smoothing, view-space bounding, and efficient 3D culling, delivering artifact-free
  real-time rendering even under extreme zoom levels and out-of-distribution views.
date: 2025-10-23
venue: Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV)
paperurl: https://derthomy.github.io/AAA-Gaussians/static/paper/AAA-Gaussians.pdf
projecturl: https://derthomy.github.io/AAA-Gaussians/
citation: 'Michael Steiner, Thomas Köhler, Lukas Radl, Felix Windisch, Dieter Schmalstieg,
  Markus Steinberger (2025). &quot;AAA-Gaussians: Anti-Aliased and Artifact-Free 3D
  Gaussian Rendering.&quot; In <i>Proceedings of the IEEE/CVF International Conference
  on Computer Vision (ICCV)</i>. <a href="https://doi.org/10.1109/iccv51701.2025.02567">doi:10.1109/iccv51701.2025.02567</a>'
header:
  teaser: publications/AAA.mp4
authors: Michael Steiner*, <strong>Thomas Köhler*</strong>, Lukas Radl, Felix Windisch,
  Dieter Schmalstieg, Markus Steinberger
---
Although 3D Gaussian Splatting (3DGS) has revolutionized 3D reconstruction, it still faces challenges such as aliasing, projection artifacts, and view inconsistencies, primarily due to the simplification of treating splats as 2D entities. We argue that incorporating full 3D evaluation of Gaussians throughout the 3DGS pipeline can effectively address these issues while preserving rasterization efficiency. Specifically, we introduce an adaptive 3D smoothing filter to mitigate aliasing and present a stable view-space bounding method that eliminates popping artifacts when Gaussians extend beyond the view frustum. Furthermore, we promote tile-based culling to 3D with screen-space planes, accelerating rendering and reducing sorting costs for hierarchical rasterization. Our method achieves state-of-the-art quality on in-distribution evaluation sets and significantly outperforms other approaches for out-of-distribution views. Our qualitative evaluations further demonstrate the effective removal of aliasing, distortions, and popping artifacts, ensuring real-time, artifact-free rendering.