---
title: "NeuralPVS: Learned Estimation of Potentially Visible Sets"
collection: publications
category: conferences
permalink: /publication/NeuralPVS
excerpt: 'Provides state of the art from region PVS calculation using deep neural networks.'
date: 2025-09-29
venue: 'SIGGRAPH Asia'
paperurl: 'https://arxiv.org/pdf/2509.24677'
projecturl: https://windingwind.github.io/neuralpvs/index.html
citation: 'Xiangyu Wang, Thomas Köhler, Jun Lin Qiu, Shohei Mori, Markus Steinberger, Dieter Schmalstieg (2025). &quot;NeuralPVS: Learned Estimation of Potentially Visible Sets.&quot; <i>SIGGRAPH Asia</i>.'
---
Real-time visibility determination in expansive or dynamically changing environments has long posed a significant challenge in computer graphics. Existing techniques are computationally expensive and often applied as a precomputation step on a static scene. We present NeuralPVS, the first deep-learning approach for visibility computation that efficiently determines from-region visibility in a large scene, running at approximately 100 Hz processing with less than  missing geometry. This approach is possible by using a neural network operating on a voxelized representation of the scene. The network's performance is achieved by combining sparse convolution with a 3D volume-preserving interleaving for data compression. Moreover, we introduce a novel repulsive visibility loss that can effectively guide the network to converge to the correct data distribution. This loss provides enhanced robustness and generalization to unseen scenes. Our results demonstrate that NeuralPVS outperforms existing methods in terms of both accuracy and efficiency, making it a promising solution for real-time visibility computation.