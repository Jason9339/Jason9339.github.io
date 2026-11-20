---
layout: page
permalink: /cv/
title: CV
nav: true
nav_order: 5
---

Taipei, Taiwan · [jasonlin930309@gmail.com](mailto:jasonlin930309@gmail.com) · [github.com/Jason9339](https://github.com/Jason9339)

<a href="{{ '/assets/pdf/Zih-Ci_Lin_CV.pdf' | relative_url }}" target="_blank" rel="noopener noreferrer"><i class="fa-solid fa-file-pdf"></i> Download CV (PDF)</a>

## Education

**National Chengchi University (NCCU)**, Taipei, Taiwan — _Sep 2022 – Jun 2026_

- _B.S. in Computer Science_ and _B.S. in Artificial Intelligence Applications_ (two B.S. degrees); Electrophysics Credit Program
- Cumulative GPA: 4.29/4.30 \| Department Rank: 1/49
- **Relevant Coursework:** Computer Vision Practice with Deep Learning, Image Processing, Natural Language Processing, Deep Learning: Fundamentals and Applications, Human–Computer Interaction

## Honors and Awards

- **College Student Research Creativity Award**, National Science and Technology Council (NSTC), Taiwan — _2026_<br>
  Awarded to 200 of 4,377 funded undergraduate research projects nationwide (top 4.6%)
- **Dean's List Awards**, NCCU (top 5% of class; 7 semesters) — _2022 – 2026_
- **Academic Excellence Award**, top 3 in 10 required CS courses — _2023 – 2024_<br>
  Algorithms, Data Structures, Operating Systems, Computer Architecture and Organization, Discrete Mathematics, Linear Algebra, Probability, Object-Oriented Programming, Digital Systems, Computer Programming II
- **Collegiate Programming Examination (CPE), Professional Level:** ranked 61/2586 (top 2.4%) in C/C++ — _2024_

## Publications

- **Zih-Ci Lin** and Wen-Hung Liao. "Decoding-Time Fusion of OCR and Large Language Models for Traditional Chinese Historical Document Recognition." In _Proceedings of the 28th International Conference on Pattern Recognition (ICPR 2026)_, LNCS vol. 16819, pp. 48–62. Springer, 2026. [[DOI]](https://doi.org/10.1007/978-3-032-31404-8_4)

## Research Experience

**Undergraduate Researcher, Visual Information Processing Lab, NCCU** — _Sep 2024 – Jun 2026_<br>
Advisor: Prof. Wen-Hung Liao \| Project: OCR–LLM Fusion for Traditional Chinese Historical Documents (NSTC-funded)

- Investigated how linguistic context aids historical Chinese OCR by fusing TrOCR hypotheses with a frozen language model in UTF-8 byte-aligned beam search.
- Reduced character error rate (CER) by 10.00% (relative) on real manuscripts and up to 15.37% on semantically structured text; ablations revealed failures from excessive language-model influence.
- Built configurable synthetic-text generator producing 4.1M historical-style image–text pairs; assembled manually annotated benchmark of 921 real-manuscript samples.

**Part-time Research Assistant, NCCU Library** — _Sep 2025 – Jun 2026_<br>
Project: Library Digital Transformation

- Built offline AI-assisted annotation system for character-level labels and transcriptions, now used by library staff.
- Added automatic reading order, variant-character mapping, and batch metadata entry based on staff feedback.

**Research Assistant, Chinese Knowledge and Information Processing Lab, Academia Sinica** — _Jul 2025 – Nov 2025_<br>
Advisor: Prof. Wei-Yun Ma \| Project: JEPA-Based Diagram Understanding and Diagram-to-Code Generation

- Designed diagram-to-code pipeline in which a vision-language model (VLM) with an I-JEPA vision encoder predicts a unified JSON intermediate representation, then converts it into TikZ, Mermaid, or Graphviz code.
- Proposed JEPA variants masking diagram elements (nodes, edges, text) instead of random image patches.
- Built rule-based TikZ/Mermaid/Graphviz-to-JSON converters; curated 36K diagram–code pairs from CoSyn-400K.

## Work Experience

**Full-Time Research Personnel, Department of Computer Science, NCCU** — _Jul 2026 – Present_<br>
Project: Solar Photovoltaic (PV) Development — AI Document Parsing & Aerial Imagery Analysis

- Develop AI pipelines parsing solar PV permit PDFs, engineering layout drawings, and their legends.
- Combine VLMs with image segmentation to read drawing legends and locate PV facilities.
- Adapt rooftop and solar-panel detection models to Taiwanese aerial orthophotos, bridging domain gap to estimate installable rooftop area and current PV installation ratio.

## Selected Projects

**Moojidle — Course Management System** [GitLab](https://gitlab.com/jingxiang0405/moojidle) · [GitHub (k8s)](https://github.com/Jason9339/moojidle-k8s) — _2025 – 2026_<br>
**Courses:** Introduction to Software Engineering; Distributed Systems<br>
**Role:** Co-Lead (one of three); Course-Feature Subteam Lead; Frontend Reviewer<br>
**Tools:** Express.js, React.js, MongoDB, Nginx, Docker, GitLab CI/CD, GitHub Actions, AWS, Kubernetes (k3s), Terraform, k6

_Initial Development_ (2025)

- Co-led 9-person Agile team, coordinating Jira sprint planning and task breakdown across subteams.
- Led course-feature subteam building course pages and features; reviewed frontend code for all subteams.
- Deployed on AWS behind Nginx reverse proxy with MongoDB Atlas, gated by GitLab CI/CD build and test checks.
- Reduced task completion time for common course operations by 40–70% compared with Moodle.

_Infrastructure Upgrade_ (2026, 6-person team)

- Migrated single-EC2 monolith to 5-node high-availability k3s cluster on AWS, storing files in MongoDB GridFS.
- Codified infrastructure with Terraform and Bash, cutting full deployment from 0.5–1 hour to about 10 minutes.
- Configured horizontal pod autoscaling, rolling updates, and CloudWatch/SNS alerting; validated resilience with k6 stress tests, ranking first in final class presentation.

**FG-CIDNet: Frequency-Guided Low-Light Image Enhancement** — _2025_<br>
**Course:** Computer Vision Practice with Deep Learning (graduate-level)<br>
**Role:** Team Leader (team of five)

- Proposed FG-CIDNet, extending HVI-based CIDNet (CVPR 2025) with frequency encoder, frequency-guided cross-attention, and frequency-domain loss on luminance gradients.
- Reproduced CIDNet baseline and trained FG-CIDNet under identical budget on LOL-Blur, improving PSNR, SSIM, and LPIPS; also tested ensembling DarkIR and CIDNet outputs.
- Tested enhancement as preprocessing for night-time object detection (YOLOv8, BDD100K), finding that better image quality did not always improve detection.

**Reproducing SCConv for CNN Feature-Redundancy Reduction** — _2025_<br>
**Course:** Deep Learning: Fundamentals and Applications<br>
**Role:** Experiment Lead; report writing and presentation (team of four)

- Reproduced SCConv (CVPR 2023), a plug-in convolution that reduces spatial and channel redundancy in CNNs.
- Ran experiments with SCConv in ResNet50 and DenseNet121, comparing accuracy, model size, FLOPs, GPU memory, and training time against baselines on CIFAR-100 and Food-101.
- Analyzed results and wrote final report, showing that lower FLOPs did not translate into faster training or lower memory use in practice.

**AESOP Loss on a Lightweight Super-Resolution Transformer (ESRT)** [GitHub](https://github.com/Thirvin/ImageProcessFinal) — _2025_<br>
**Course:** Image Processing (graduate-level)<br>
**Role:** Experiments; led report writing and presentation (team of two)

- Trained lightweight Transformer ESRT with AESOP loss (CVPR 2025) in place of L1, without perceptual losses.
- Compared with L1 baseline on Set14 and BSD100: sharper textures and better LPIPS/DISTS at minor PSNR cost.

**Prompting Strategies for Chinese Logical Reasoning with LLMs** — _2025_<br>
**Course:** Natural Language Processing<br>
**Role:** Team Leader (team of four)

- Curated 80 Chinese logic puzzles graded by difficulty; compared six prompting strategies (e.g., chain-of-thought).
- Found prompting gains limited and unstable on hard problems, while reasoning-oriented models stayed accurate, suggesting structural changes beyond prompt engineering are needed.

## Skills

- **Programming Languages:** Python, C/C++, JavaScript, SQL
- **Machine Learning & Vision:** PyTorch, Hugging Face Transformers, OpenCV, NumPy
- **Web & Infrastructure:** React, Express.js, Django, MongoDB, Nginx, Docker, Kubernetes, Terraform, AWS, GitLab CI/CD, GitHub Actions, k6
