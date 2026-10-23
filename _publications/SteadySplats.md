---
title: 'SteadySplats: Resampling of Low-Variance Gaussians for High-Fidelity Stochastic
  Rendering'
collection: publications
category: arxiv
permalink: /publication/SteadySplats
excerpt: Stochastic order-independent transparency enables efficient rendering for
  3D Gaussian Splatting, but suffers from visible noise and temporal flickering. We
  introduce history-based spatial resampling and temporal importance resampling alongside
  a variance-reducing training regularizer, boosting single-sample quality by 13 dB
  PSNR for real-time stochastic rendering.
date: '2026-10-20'
venue: ArXiv
paperurl: https://arxiv.org/pdf/2610.05576
projecturl: https://derthomy.github.io/SteadySplats/
citation: 'Felix Windisch*, Thomas Köhler*, Lukas Radl, Chris Wyman, Georgios Kopanas,
  Bernhard Kerbl, Markus Steinberger (2026). &quot;SteadySplats: Resampling of Low-Variance
  Gaussians for High-Fidelity Stochastic Rendering.&quot; <i>arXiv preprint arXiv:2610.05576</i>.'
header:
  teaser: publications/steadysplats.gif
authors: Felix Windisch*, <strong>Thomas Köhler*</strong>, Lukas Radl, Chris Wyman,
  Georgios Kopanas, Bernhard Kerbl, Markus Steinberger
---
Stochastic order-independent transparency enables efficient and elegant rendering of primitive-based radiance fields like 3D Gaussian Splatting models, but remains impractical due to the inherent visible noise in the output. We propose a principled approach to minimize high-frequency noise, addressing its sources at the representation and image synthesis level.

During stochastic rendering, our history-based spatial resampling scheme drastically accelerates image convergence, while temporal importance resampling ensures coherence under camera movement. During training, a color regularizer implicitly reduces the variance along view rays in the 3DGS models. With these properties, our optimized, Vulkan-based renderer effectively mitigates output noise at low and high sample counts, achieving a substantial 13 dB PSNR increase in quality over previous stochastic methods at 1 sample per pixel and quickly converging to sorted 3DGS with an average L1 error of less than $10^{-4}$.
