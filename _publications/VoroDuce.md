---
title: 'VoroDuce: Massively Parallel 3D Voronoi Simplification with Volume-Aware Edge
  Collapse'
collection: publications
category: arxiv
permalink: /publication/VoroDuce
excerpt: Simplifying large 3D Voronoi diagrams is vital across materials science and
  simulation, but traditional decimation struggles with GPU scalability. We introduce
  a massively parallel GPU simplification framework operating on dual Delaunay tetrahedralization
  using volume-aware edge collapses, compressing million-cell models while preserving
  volume, shape fidelity, and topology.
date: 2026-10-15
venue: ArXiv
paperurl: https://arxiv.org/pdf/2610.21811
citation: 'Felix Windisch, Lukas Radl, Thomas Köhler, Shrisudhan Govindarajan, Marcel
  Pur, Andrea Tagliasacchi, Markus Steinberger (2026). &quot;VoroDuce: Massively Parallel
  3D Voronoi Simplification with Volume-Aware Edge Collapse.&quot; <i>arXiv preprint
  arXiv:2610.21811</i>.'
authors: Felix Windisch, Lukas Radl, <strong>Thomas Köhler</strong>, Shrisudhan Govindarajan,
  Marcel Pur, Andrea Tagliasacchi, Markus Steinberger
---
3D Voronoi diagrams provide a powerful mathematical framework for representing volumetric functions and geometry with applications to Materials Science, Biology, Simulation and Astrophysics. However, accurately resolving fine structures often requires millions of cells, imposing severe computational and memory constraints. Traditional mesh decimation or point cloud simplification techniques fail to account for the effects re-meshing has on neighbouring cells.

In this work, we formalize the Voronoi reduction problem and propose a greedy edge-collapsing algorithm on the dual Delaunay tetrahedralisation that accounts for changes in the local geometry. Further, we demonstrate a novel volumetric error approximation technique that models convex cell intersections as truncated prismatoids, circumventing computationally prohibitive exact volume calculations and enabling massive GPU parallelization. Evaluations across Synthetic, Medicine and Material Science data demonstrate that VoroDuce decimates models with up to a million primitives, successfully compressing the representation while preserving the underlying data better than naive decimation approaches.
