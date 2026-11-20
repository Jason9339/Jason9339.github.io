---
layout: page
title: Reproducing SCConv for CNN Feature-Redundancy Reduction
description: 2025 · Reproducing SCConv (CVPR 2023) and testing whether fewer FLOPs actually mean faster, lighter training.
importance: 4
category: course projects
---

**Course:** Deep Learning: Fundamentals and Applications · 2025<br>
**Role:** Experiment Lead; report writing and presentation (team of four)

### Problem

SCConv (CVPR 2023) is a plug-in convolution that reduces spatial and channel redundancy in CNNs, promising smaller and cheaper models.
We wanted to check whether these savings hold up in practice.

### Approach

We reproduced SCConv and inserted it into ResNet50 and DenseNet121, then compared accuracy, model size, FLOPs, GPU memory, and training time against the original baselines on CIFAR-100 and Food-101.

### Results

Lower FLOPs did not translate into faster training or lower memory use in practice.

### My role

Experiment lead: I ran the experiments, analyzed the results, wrote the final report, and gave the presentation.
