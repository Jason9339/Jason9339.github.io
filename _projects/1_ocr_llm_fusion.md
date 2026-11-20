---
layout: page
title: OCR–LLM Fusion for Traditional Chinese Historical Documents
description: 2024 – 2026 · Fusing an OCR model with a frozen language model at decoding time to reduce character errors on Traditional Chinese historical manuscripts (ICPR 2026).
importance: 1
category: research
---

**Undergraduate research** · Visual Information Processing Lab, NCCU · 2024 – 2026<br>
**Advisor:** Prof. Wen-Hung Liao · NSTC-funded project<br>
**Publication:** Zih-Ci Lin and Wen-Hung Liao. "Decoding-Time Fusion of OCR and Large Language Models for Traditional Chinese Historical Document Recognition." In _Proceedings of the 28th International Conference on Pattern Recognition (ICPR 2026)_, LNCS vol. 16819, pp. 48–62. Springer, 2026. [[DOI]](https://doi.org/10.1007/978-3-032-31404-8_4)

### Problem

OCR for Traditional Chinese historical documents must recognize characters that are often degraded, rare, or visually ambiguous.
This project investigates how linguistic context can help historical Chinese OCR: when a language model can correct the visual recognizer, and when it makes things worse.

### Approach

Extending Generative Fusion Decoding (GFD) to Traditional Chinese historical OCR, the system fuses TrOCR hypotheses with a frozen language model in a UTF-8 byte-aligned beam search, so linguistic context is applied at decoding time without retraining the language model.
To train and evaluate the system, I built a configurable synthetic-text generator that produces 4.1M historical-style image–text pairs, and assembled a manually annotated benchmark of 921 real-manuscript samples.

### Results

Decoding-time fusion reduced the character error rate (CER) by 10.00% (relative) on real manuscripts and by up to 15.37% on semantically structured text.
Ablation studies revealed failures caused by excessive language-model influence.

### My role

First author. Extended Generative Fusion Decoding (GFD) to Traditional Chinese historical OCR, built the synthetic data generator and the manually annotated benchmark, and conducted all experiments.

### Links

- Paper: [doi.org/10.1007/978-3-032-31404-8_4](https://doi.org/10.1007/978-3-032-31404-8_4)
- Code: [traditional-chinese-historical-document-ocr-llm-fusion](https://github.com/Jason9339/traditional-chinese-historical-document-ocr-llm-fusion)
- Synthetic data generator: [ocr-synth-generator](https://github.com/Jason9339/ocr-synth-generator)
- Datasets: [real-manuscript benchmark](https://huggingface.co/datasets/ZihCiLin/traditional-chinese-historical-ocr-lo-chia-luen) · [synthetic training data](https://huggingface.co/datasets/ZihCiLin/traditional-chinese-ocr-synthetic)
