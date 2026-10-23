---
title: Frustum Volume Caching for Accelerated NeRF Rendering
collection: publications
category: manuscripts
permalink: /publication/FruVoCA
excerpt: Evaluating coordinate-based MLPs at every sample point along camera rays
  creates a primary bottleneck for real-time NeRF rendering. We present a view-frustum
  volume (froxel) caching technique that stores non-view-dependent MLP features directly
  in a camera-aligned grid, accelerating ray marching and achieving substantial rendering
  speedups with negligible visual loss.
date: 2024-08-09
venue: Proceedings of the ACM on Computer Graphics and Interactive Techniques (PACMGIT)
paperurl: https://steimich96.github.io/FrustumVolumeCaching/assets/paper/FrustumVolumeCaching.pdf
projecturl: https://steimich96.github.io/FrustumVolumeCaching/
citation: Michael Steiner, Thomas Köhler, Lukas Radl, Markus Steinberger (2024). &quot;Frustum
  Volume Caching for Accelerated NeRF Rendering.&quot; <i>Proceedings of the ACM on
  Computer Graphics and Interactive Techniques (PACMGIT / EGSR 2024)</i>. 7(3). <a
  href="https://doi.org/10.1145/3675370">doi:10.1145/3675370</a>
header:
  teaser: publications/FruVoCA.mp4
authors: Michael Steiner, <strong>Thomas Köhler</strong>, Lukas Radl, Markus Steinberger
---
Neural Radiance Fields (NeRFs) have revolutionized the field of inverse rendering due to their ability to synthesize high-quality novel views and applicability in practical contexts. NeRFs leverage volume rendering, evaluating view-dependent color at each sample with an expensive network, where a high computational burden is placed on extracting an informative, view-independent latent code. We propose a temporal coherence method to accelerate NeRF rendering by caching the latent codes of all samples in an initial viewpoint and reusing them in consecutive frames. By utilizing a sparse frustum volume grid for caching and performing lookups via backward reprojection, we enable temporal reuse of NeRF samples while maintaining the ability to re-evaluate view-dependent effects efficiently. To facilitate high-fidelity rendering from our cache with interactive framerates, we propose a novel cone encoding and explore a training scheme to induce local linearity into the latent information. Extensive experimental evaluation demonstrates that these choices enable high-quality real-time rendering from our cache, even when reducing latent code size significantly. Our proposed method scales exceptionally well for large networks, and our highly optimized real-time implementation allows for cache initialization at runtime. For offline rendering of high-quality video sequences with expensive supersampled effects like motion blur or depth of field, our approach provides speed-ups of up to 2×.