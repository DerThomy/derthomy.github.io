---
title: 'NeuralPVS: Learned Estimation of Potentially Visible Sets'
collection: publications
category: conferences
permalink: /publication/NeuralPVS
excerpt: Real-time visibility determination and Potentially Visible Set (PVS) computation
  in expansive environments is essential for occlusion culling, but offline precomputation
  is notoriously expensive. We introduce NeuralPVS, replacing costly geometric visibility
  tests with deep neural inference over volumetric scene cells to predict conservative
  visibility sets in real time with less than 1% missed geometry.
date: 2025-12-14
venue: Proceedings of the SIGGRAPH Asia 2025 Conference Papers
paperurl: https://arxiv.org/pdf/2509.24677
projecturl: https://windingwind.github.io/neuralpvs/index.html
citation: 'Xiangyu Wang, Thomas Köhler, Jun Lin Qiu, Shohei Mori, Markus Steinberger,
  Dieter Schmalstieg (2025). &quot;NeuralPVS: Learned Estimation of Potentially Visible
  Sets.&quot; In <i>Proceedings of the SIGGRAPH Asia 2025 Conference Papers</i>. <a
  href="https://doi.org/10.1145/3757377.3763822">doi:10.1145/3757377.3763822</a>'
header:
  teaser: publications/neuralpvs.png
authors: Xiangyu Wang, <strong>Thomas Köhler</strong>, Jun Lin Qiu, Shohei Mori, Markus
  Steinberger, Dieter Schmalstieg
---
Real-time visibility determination in expansive or dynamically changing environments has long posed a significant challenge in computer graphics. Existing techniques are computationally expensive and often applied as a precomputation step on a static scene. We present NeuralPVS, the first deep-learning approach for visibility computation that efficiently determines from-region visibility in a large scene, running at approximately 100 Hz processing with less than 1% missing geometry. This approach is possible by using a neural network operating on a voxelized representation of the scene. The network's performance is achieved by combining sparse convolution with a 3D volume-preserving interleaving for data compression. Moreover, we introduce a novel repulsive visibility loss that can effectively guide the network to converge to the correct data distribution. This loss provides enhanced robustness and generalization to unseen scenes. Our results demonstrate that NeuralPVS outperforms existing methods in terms of both accuracy and efficiency, making it a promising solution for real-time visibility computation.