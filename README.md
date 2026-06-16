# OneBar / PIOPD

This repository hosts the project page and minimal materials for:

**OneBar: An End-to-End Content-Grounded Generative Query Recommendation Framework for E-Commerce Video Feeds**

- Paper: https://arxiv.org/abs/2606.15330
- Project page: https://1045334875.github.io/onebar/

GitHub Pages serves the root URL from `index.html`; this repository keeps the project page at the repository root for that reason.

## What is OneBar?

OneBar is an end-to-end generative framework for real-time query recommendation in e-commerce short-video feeds. Instead of retrieving queries from a fixed candidate pool, OneBar directly generates bottom-bar queries from content-grounded evidence, including textual metadata, multimodal video understanding, collaborative query anchors, and user-side evidence.

## What is PIOPD?

**PIOPD**, or **Preference-Internalized On-Policy Distillation**, is the central training contribution in OneBar. It is an OPSD-style posterior preference distillation strategy for turning behavior-confirmed posterior signals into the deployable generator's model weights.

The key idea is:

- the online student generates under the same trigger-only input available at serving time;
- the teacher has access to posterior behavior evidence;
- the student is trained on its own generated states;
- dense teacher distributions transfer behavior preferences into the serving-time generator;
- after training, the teacher and posterior evidence are discarded, so online serving still uses the same trigger-only interface.

In this sense, PIOPD adapts the OPD/OPSD-style distillation loop to industrial generative recommendation, where the goal is to internalize hierarchical behavior preferences into a low-latency query generation policy.

## Keywords

OPSD, On-Policy Self-Distillation, OPD, On-Policy Distillation, PIOPD, Posterior Distillation, Preference Distillation, Generative Query Recommendation, E-Commerce Search, Short-Video Search, Query Recommendation.

## Citation

```bibtex
@article{tang2026onebar,
  title   = {OneBar: An End-to-End Content-Grounded Generative Query Recommendation Framework for E-Commerce Video Feeds},
  author  = {Tang, Yao and Yang, Ying and Chen, Ben and Ma, Yufei and Liang, Zihan and Lei, Chenyi and Ou, Wenwu and Liu, Jian},
  journal = {arXiv preprint arXiv:2606.15330},
  year    = {2026}
}
````

