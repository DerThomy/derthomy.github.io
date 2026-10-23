---
title: Efficient Confidence-Aware Densification for 3DGS
collection: publications
category: arxiv
permalink: /publication/EfficientConfidenceDensification
excerpt: Standard 3DGS-MCMC relies on opacity-based sampling under fixed primitive
  budgets, often oversaturating foregrounds while leaving backgrounds under-reconstructed.
  We propose a confidence-aware densification strategy that places primitives guided
  by image errors and learned confidence weights, outperforming 3DGS-MCMC across PSNR,
  SSIM, and LPIPS across all primitive budgets.
date: 2026-10-09
venue: ArXiv
paperurl: https://arxiv.org/pdf/2610.13541
citation: Manuel Hofer, Thomas Köhler, Felix Windisch, Bernhard Kerbl, Markus Steinberger,
  Lukas Radl (2026). &quot;Efficient Confidence-Aware Densification for 3DGS.&quot;
  <i>arXiv preprint arXiv:2610.13541</i>.
authors: Manuel Hofer, <strong>Thomas Köhler</strong>, Felix Windisch, Bernhard Kerbl,
  Markus Steinberger, Lukas Radl
---
3DGS-MCMC has replaced the gradient-driven density control of 3D Gaussian Splatting with opacity-based sampling and relocation, and is now the de facto standard for prior-free densification under a fixed primitive budget. Because opacity stays high where the scene is already well reconstructed, this sampling sends most new primitives to the foreground and leaves the background under-reconstructed. At low budgets, prior-based methods such as ConeGS and EDGS outperform it, at the cost of a pre-trained radiance field or dense image matches and a separate initialization stage.

We argue for a comeback of error-driven densification within the fixed-budget MCMC framework. Our confidence-aware densification keeps the fixed budget and gradual growth of 3DGS-MCMC, but places primitives by the image error instead of the opacity. New primitives are drawn mostly where screen-space gradients are large. We favor primitives with a low learned confidence, which marks regions the reconstruction still explains poorly, and relocate the primitives that contribute least to the rendered images to these places. Averaged over 24 scenes, our method outperforms 3DGS-MCMC in PSNR, SSIM and LPIPS at every budget from 100k to 2M primitives.
