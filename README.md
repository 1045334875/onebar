# OneBar

This repository is the official project page and code repository for the paper:

**OneBar: An End-to-End Content-Grounded Generative Query Recommendation Framework for E-Commerce Video Feeds**

- Paper: https://arxiv.org/abs/2606.15330
- Project page: https://1045334875.github.io/onebar/

## Overview

OneBar is an end-to-end generative framework for real-time query recommendation in e-commerce video feeds. Instead of relying on a retrieval-based candidate cascade, OneBar directly generates bottom-bar queries from content-grounded evidence, including cleaned textual metadata, multimodal video understanding, collaborative query anchors, and trigger-relevant user-side evidence.

The paper also introduces **PIOPD** (Preference-Internalized On-Policy Distillation), a posterior preference distillation strategy that transfers behavior-confirmed intent into a deployable trigger-only online generator.

## Highlights

- End-to-end generative query recommendation for e-commerce short-video feeds
- Content-grounded generation with multimodal and collaborative evidence
- Preference internalization through posterior-aware on-policy distillation
- Online deployment under strict bottom-bar latency constraints
- Large-scale online A/B improvements in exposure, click, order, and GMV metrics

## Code Release

The training and inference codebase is **currently being prepared** and will be released in this repository.

Planned release contents:

- model training pipeline
- inference and serving-related components
- data preprocessing and prompt construction scripts
- documentation for reproducing the main framework

For now, this repository primarily contains the public project page and release metadata for the paper.

## Repository Contents

- `index.html`: project page
- `assets/`: figures used by the project page
- `robots.txt`, `sitemap.xml`: project page indexing metadata
- `PROMOTION_COPY.md`: reusable outreach and announcement copy

## Method Summary

OneBar is built around three main ideas:

1. **Collaborative-multimodal intent grounding**
   The framework combines textual metadata, multimodal summaries, collaborative query anchors, and relevant user evidence to build robust generation context.

2. **Unified low-latency end-to-end generation**
   A compact encoder-decoder generator replaces a traditional multi-stage retrieval and ranking cascade.

3. **Progressive preference internalization**
   PIOPD distills posterior behavior preferences from a teacher with privileged evidence into a trigger-only student that matches the real online serving interface.

## Citation

If you find this work useful, please cite:

```bibtex
@article{tang2026onebar,
  title   = {OneBar: An End-to-End Content-Grounded Generative Query Recommendation Framework for E-Commerce Video Feeds},
  author  = {Tang, Yao and Yang, Ying and Chen, Ben and Ma, Yufei and Liang, Zihan and Lei, Chenyi and Ou, Wenwu and Liu, Jian},
  journal = {arXiv preprint arXiv:2606.15330},
  year    = {2026}
}
```
