---
layout: page
title: "FG-CIDNet: Frequency-Guided Low-Light Image Enhancement"
description: 2025 · Extending CIDNet (CVPR 2025) with frequency-domain guidance for low-light image enhancement.
importance: 2
category: course projects
---

**Course:** Computer Vision Practice with Deep Learning (graduate-level) · 2025<br>
**Role:** Team Leader (team of five)

### Problem

Low-light images lose detail and contrast, which hurts both human viewing and downstream vision tasks.
We set out to improve HVI-based CIDNet (CVPR 2025), a recent low-light enhancement model.

### Approach

We proposed FG-CIDNet, which extends CIDNet with a frequency encoder, frequency-guided cross-attention, and a frequency-domain loss on luminance gradients.
We reproduced the CIDNet baseline and trained FG-CIDNet under an identical training budget on LOL-Blur, and also tested ensembling the outputs of DarkIR and CIDNet.

### Results

FG-CIDNet improved PSNR, SSIM, and LPIPS over the reproduced baseline.
We also tested enhancement as preprocessing for night-time object detection (YOLOv8 on BDD100K) and found that better image quality did not always improve detection.

### My role

Team leader of a five-person team.
