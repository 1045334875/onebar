# OneBar Promotion Copy

## Target Keywords

- OPSD for recommendation
- OPSD for generative recommendation
- OPSD query recommendation
- OPSD-style distillation
- on-policy distillation for recommendation
- posterior preference distillation
- preference-internalized on-policy distillation
- PIOPD
- OneBar PIOPD
- OneBar OPSD
- generative query recommendation
- short-video query recommendation
- e-commerce video search

## FAQ Copy

### What is PIOPD?

PIOPD stands for Preference-Internalized On-Policy Distillation. It is an OPSD-style posterior preference distillation method proposed in OneBar for generative query recommendation.

### Is PIOPD the same as OPSD?

PIOPD is not the original OPSD method for general LLM reasoning. It adapts the OPSD-style on-policy distillation idea to industrial generative query recommendation, where a posterior-aware teacher transfers behavior-confirmed intent into a trigger-only online student.

### Why is OneBar relevant to OPSD?

OneBar applies OPSD-style distillation to a recommendation and search generation scenario. The student is trained on its own rollout states, while the teacher uses posterior behavior evidence to provide dense token-level supervision.

### What problem does OneBar solve?

OneBar solves real-time bottom-bar query recommendation for e-commerce short-video feeds. It replaces retrieval-based cascade pipelines with an end-to-end content-grounded query generator.

### What are the main results?

OneBar improves query exposure, query clicks, guided orders, and guided GMV in online A/B testing, while reducing manual bad-case rate.

## English Social Post

We released the project page for **OneBar**, our end-to-end generative query recommendation framework for e-commerce short-video feeds.

The core method is **PIOPD**: an OPSD-style posterior preference distillation strategy that transfers behavior-confirmed intent from a posterior-aware teacher into a trigger-only online student.

This allows the serving model to generate real-time bottom-bar queries without relying on a separate online reward model or retrieval-heavy cascade.

Paper: https://arxiv.org/abs/2606.15330
Project page: https://1045334875.github.io/onebar/

Keywords: OPSD-style distillation, PIOPD, posterior preference distillation, generative query recommendation, e-commerce search.

## Chinese Social Post

我们发布了 **OneBar** 的论文主页：一个面向电商短视频场景的端到端生成式 query recommendation 框架。

核心方法是 **PIOPD**：一种 OPSD-style 的 posterior preference distillation 方法。它使用带有后验行为信息的 teacher，将用户行为确认过的 intent 蒸馏到线上 trigger-only student 中，从而在不引入线上 reward model 的情况下，让生成模型内化行为偏好。

论文：https://arxiv.org/abs/2606.15330
主页：https://1045334875.github.io/onebar/

关键词：OPSD-style distillation、PIOPD、posterior preference distillation、generative query recommendation、短视频搜索推荐。

## awesome-on-policy-distillation PR

### PR Title

Add OneBar: OPSD-style distillation for generative query recommendation

### PR Body

This PR adds OneBar to the Domain Extensions section.

OneBar studies real-time generative query recommendation for e-commerce short-video feeds. Its Stage III training introduces PIOPD, an OPSD-style posterior preference distillation strategy: the online student is trained on its own generated states under trigger-only serving input, while a posterior-aware teacher provides dense token-level supervision informed by behavior evidence.

I placed it under a new "Recommendation and Search" subsection because the paper adapts the OPD/OPSD-style distillation loop to an industrial recommendation/search generation scenario, rather than pure text reasoning.

Paper: https://arxiv.org/abs/2606.15330
Project page: https://1045334875.github.io/onebar/

### README Entry

```markdown
### Recommendation and Search

* [OneBar: An End-to-End Content-Grounded Generative Query Recommendation Framework for E-Commerce Video Feeds](https://arxiv.org/abs/2606.15330) *(2026)* - Introduces PIOPD, an OPSD-style posterior preference distillation strategy that transfers behavior-informed teacher distributions to a trigger-only student for real-time generative query recommendation.
```

## PIOPD Figure Caption

PIOPD adapts OPSD-style on-policy distillation to generative query recommendation: a posterior-aware teacher supervises a trigger-only student on the student's own rollout states.

## Monitoring Queries

```text
site:1045334875.github.io/onebar OneBar
site:1045334875.github.io/onebar PIOPD
site:1045334875.github.io/onebar OPSD
"OneBar" "PIOPD"
"PIOPD" "OPSD-style"
"OPSD" "generative query recommendation"
"posterior preference distillation" "OneBar"
```

```text
What is PIOPD?
What is OneBar query recommendation?
Are there OPSD methods for recommendation?
What papers apply OPSD to generative recommendation?
What is posterior preference distillation for query recommendation?
```
