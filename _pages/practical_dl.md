---
layout: archive
title: "Practical tips to Deep Learning training"
permalink: /practical_dl/
author_profile: false
---

### Practical tips:

- To overfitting and beyond: Always train until the learning behavior is stable. Its impossible to fully understand your model otherwise. Overfitting only happens when performance drops for untrained for samples (i.e., validation or test). If it stays flat it may be doing something useful [1].

- The best for transfer: The best performing model in validation for a given problem, may not be the best for transfer learning. Models trained for longer, at the cost of a slight drop in performance, may work better.

- Start small and go deep: (This process is long, and requires lots of training experiments. Is not appropriate for all cases) Start your network design with a relatively small network (as in, with low capacity). See what results you can get with it, and how far it will go before overfitting (assuming it will eventually do). After that, you may try to increase width. That most likely wont change the overall training behavior, but a mild jump in performance may happen. Once we consider the performance of the network with its depth is close to its optimal, we increase depth (at this point we may want to find the width of the new layer through experimentation). If performance increased with the added layer, add another one. Once performance drops from the previous version, start applying regularization methods. 

- Kernels, from small to large: Convolutional neurons from low-level layers (i.e., close to the output) may benefit from large kernels, since very small patterns in terms of pixels are usually of little use (this os a weaker case for high resolution images).On the other hand, convolutional neurons from high-level layers may benefit from small kernels, as a "pixel" feature already contains a large amount of information.

- 

- 

- 

- 

## References
[1] [Saxe, Andrew M., et al. "On the information bottleneck theory of deep learning." International Conference on Learning Representations. 2018.](https://openreview.net/forum?id=ry_WPG-A-)
