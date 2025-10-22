---
title: "Frustum Volume Caching for Accelerated NeRF Rendering"
collection: publications
category: manuscripts
permalink: /publication/FruVoCA
excerpt: 'Speeds up NeRF rendering by caching non view dependent MLP features in a froxel grid.'
date: 2009-09-08    
venue: 'Proceedings of the ACM on Computer Graphics and Interactive Techniques'
paperurl: 'https://steimich96.github.io/FrustumVolumeCaching/assets/paper/FrustumVolumeCaching.pdf'
projectpage: https://steimich96.github.io/FrustumVolumeCaching/
citation: 'Michael Steiner, Thomas Köhler, Lukas Radl, Markus Steinberger (2024). &quot;Frustum Volume Caching for Accelerated NeRF Rendering.&quot; <i>PACMGIT</i>. 7(3).'
---
Neural Radiance Fields (NeRFs) have revolutionized the field of inverse rendering due to their ability to synthesize high-quality novel views and applicability in practical contexts. NeRFs leverage volume rendering, evaluating view-dependent color at each sample with an expensive network, where a high computational burden is placed on extracting an informative, view-independent latent code. We propose a temporal coherence method to accelerate NeRF rendering by caching the latent codes of all samples in an initial viewpoint and reusing them in consecutive frames. By utilizing a sparse frustum volume grid for caching and performing lookups via backward reprojection, we enable temporal reuse of NeRF samples while maintaining the ability to re-evaluate view-dependent effects efficiently. To facilitate high-fidelity rendering from our cache with interactive framerates, we propose a novel cone encoding and explore a training scheme to induce local linearity into the latent information. Extensive experimental evaluation demonstrates that these choices enable high-quality real-time rendering from our cache, even when reducing latent code size significantly. Our proposed method scales exceptionally well for large networks, and our highly optimized real-time implementation allows for cache initialization at runtime. For offline rendering of high-quality video sequences with expensive supersampled effects like motion blur or depth of field, our approach provides speed-ups of up to 2×.