---
title: Image-Based Spatio-Temporal Upsampling for Split Rendering
collection: publications
category: manuscripts
permalink: /publication/SplitRendering
excerpt: Split rendering distributes graphics workloads between cloud servers and
  mobile devices, but network latency causes stuttering and frame drops. We propose
  an image-based spatio-temporal upsampling pipeline that synthesizes intermediate
  display frames entirely from transmitted 2D color and motion data, delivering smooth
  high-framerate playback without on-device geometry processing.
date: 2025-05-19
venue: Computer Graphics Forum
paperurl: https://derthomy.github.io/ImageBasedSpatioTemporalInterpolation/static/paper/Image_Based_Spatio_Temporal_Interpolation_for_Split_Rendering.pdf
projecturl: https://derthomy.github.io/ImageBasedSpatioTemporalInterpolation
citation: Michael Steiner, Thomas Köhler, Lukas Radl, Brian Budge, Markus Steinberger
  (2025). &quot;Image-Based Spatio-Temporal Interpolation for Split Rendering.&quot;
  <i>Computer Graphics Forum</i>. 44(8). <a href="https://doi.org/10.1111/cgf.70215">doi:10.1111/cgf.70215</a>
header:
  teaser: publications/splitrendering.mp4
authors: Michael Steiner*, <strong>Thomas Köhler*</strong>, Lukas Radl, Brian Budge,
  Markus Steinberger
---
Low-powered devices -- such as small form factor head-mounted displays (HMDs) -- struggle to deliver a smooth and high-quality viewing experience, due to their limited power and rendering capabilities.
Cloud rendering attempts to solve the quality issue, but leads to prohibitive latency and bandwidth requirements, hindering use with HMDs over mobile connections or even over Wifi.
One solution -- split rendering -- where frames are partially rendered on the client device, often either requires geometry and rendering hardware, or struggles to generate frames faithfully under viewpoint changes and object motion.
Our method enables spatio-temporal interpolation via bidirectional reprojection to efficiently generate intermediate frames in a split rendering setting, while limiting the communication cost and relying purely on image-based rendering. Furthermore, our method is robust to modest connectivity issues and handles effects such as dynamic smooth shadows.