---
layout: page
title: AESOP Loss on a Lightweight Super-Resolution Transformer (ESRT)
description: 2025 · Training a lightweight super-resolution Transformer with AESOP loss instead of L1 for sharper textures.
importance: 5
category: course projects
---

**Course:** Image Processing (graduate-level) · 2025<br>
**Role:** Experiments; led report writing and presentation (team of two)<br>
**Code:** [GitHub](https://github.com/Thirvin/ImageProcessFinal)

### Problem

Super-resolution models trained with pixel losses such as L1 tend to produce blurry textures.
AESOP loss (CVPR 2025) aims to recover sharper detail without relying on perceptual losses.

### Approach

We trained the lightweight Transformer ESRT with AESOP loss in place of L1, without any perceptual losses, and compared it with the L1 baseline on Set14 and BSD100.

### Results

AESOP produced sharper textures and better LPIPS/DISTS scores at a minor cost in PSNR.

### My role

I ran experiments and led the report writing and presentation.
