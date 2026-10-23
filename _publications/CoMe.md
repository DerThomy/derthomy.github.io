---
title: Confidence-Based Mesh Extraction from 3D Gaussians
collection: publications
category: conferences
permalink: /publication/CoMe
excerpt: Extracting clean, watertight surfaces from 3D Gaussians is challenging because
  photometric supervision alone struggles with textureless regions and thin structures.
  CoMe introduces a self-supervised confidence framework that dynamically balances
  photometric and geometric supervision, preventing surface floaters and achieving
  state-of-the-art unbounded mesh extraction without external priors.
date: 2024-09-29
venue: European Conference on Computer Vision (ECCV)
paperurl: https://arxiv.org/pdf/2603.24725
projecturl: https://r4dl.github.io/CoMe/
citation: Lukas Radl, Felix Windisch, Andreas Kurz, Thomas Köhler, Michael Steiner,
  Markus Steinberger (2024). &quot;Confidence-Based Mesh Extraction from 3D Gaussians.&quot;
  In <i>European Conference on Computer Vision (ECCV)</i> / <i>Lecture Notes in Computer
  Science (LNCS)</i>. <a href="https://doi.org/10.1007/978-3-032-37435-6_17">doi:10.1007/978-3-032-37435-6_17</a>
header:
  teaser: publications/come.mp4
authors: Lukas Radl, Felix Windisch, Andreas Kurz, <strong>Thomas Köhler</strong>,
  Michael Steiner, Markus Steinberger
---
Recently, 3D Gaussian Splatting (3DGS) greatly accelerated mesh extraction from posed images due to its explicit representation and fast software rasterization. While the addition of geometric losses and other priors has improved the accuracy of extracted surfaces, mesh extraction remains difficult in scenes with abundant view-dependent effects. To resolve the resulting ambiguities, prior works rely on multi-view techniques, iterative mesh extraction, or large pre-trained models, sacrificing the inherent efficiency of 3DGS.

In this work, we present a simple and efficient alternative by introducing a self-supervised confidence framework to 3DGS: within this framework, learnable confidence values dynamically balance photometric and geometric supervision. Extending our confidence-driven formulation, we introduce losses which penalize per-primitive color and normal variance and demonstrate their benefits to surface extraction. Finally, we complement the above with an improved appearance model, by decoupling the individual terms of the D-SSIM loss. Our final approach delivers state-of-the-art results for unbounded meshes while remaining highly efficient.
