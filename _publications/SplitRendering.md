---
title: "Image-Based Spatio-Temporal Upsampling for Split Rendering"
collection: publications
category: manuscripts
permalink: /publication/SplitRendering
excerpt: 'Enables smooth, high-quality rendering on ultra low-powered mobile devices by generating intermediate frames entirely from images using a novel spatio-temporal interpolation split rendering pipeline—without needing geometry or real-time rasterization'
date: 2025-05-19    
venue: 'Computer Graphics Forum'
paperurl: 'https://derthomy.github.io/ImageBasedSpatioTemporalInterpolation/static/paper/Image_Based_Spatio_Temporal_Interpolation_for_Split_Rendering.pdf'
projecturl: https://derthomy.github.io/ImageBasedSpatioTemporalInterpolation
citation: 'Thomas Köhler, Michael Steiner, Lukas Radl, Brian Budge, Markus Steinberger (2025). &quot;Image-Based Spatio-Temporal Upsampling for Split Rendering.&quot; <i>Computer Graphics Forum</i>. 8(44).'
---
Low-powered devices -- such as small form factor head-mounted displays (HMDs) -- struggle to deliver a smooth and high-quality viewing experience, due to their limited power and rendering capabilities.
Cloud rendering attempts to solve the quality issue, but leads to prohibitive latency and bandwidth requirements, hindering use with HMDs over mobile connections or even over Wifi.
One solution -- split rendering -- where frames are partially rendered on the client device, often either requires geometry and rendering hardware, or struggles to generate frames faithfully under viewpoint changes and object motion.
Our method enables spatio-temporal interpolation via bidirectional reprojection to efficiently generate intermediate frames in a split rendering setting, while limiting the communication cost and relying purely on image-based rendering. Furthermore, our method is robust to modest connectivity issues and handles effects such as dynamic smooth shadows.