---
layout: post
title: Capability Evaluation — Qwen3.5-397B-A17B
description: Capability evaluation of Qwen3.5-397B-A17B, a multimodal foundation model with Hybrid MoE architecture developed by the Alibaba Qwen team. Rated L4 in reasoning and problem-solving.
permalink: /en/archives/2026/04/11/qwen35-397b-a17b-capability-evaluation/
lang: en
alt_lang_url: /ja/archives/2026/04/11/qwen35-397b-a17b-capability-evaluation/
date: 2026-04-11T09:00:00Z
last_modified_at: 2026-04-11T09:00:00Z
author: founder
categories: [strategic-forecasting]
tags: [AI, capability evaluation, Qwen, MoE, multimodal, agent]
---

**Signature capability**: Reasoning & Problem-Solving
**Level**: L4

## Overview

Qwen3.5-397B-A17B is a multimodal foundation model combining a Hybrid Mixture-of-Experts architecture with early-fusion vision-language training. It is the first Qwen open-weight model to natively support image and video input, and features a 262k-token context window (1M in the hosted Qwen3.5-Plus variant). Thinking and non-thinking modes can be toggled within a single model, making it suitable for a broad range of tasks including chat, RAG, visual understanding, and agentic workflows. It ranks third among open-weight models on the Artificial Analysis Intelligence Index.

## Capability Ratings

| Domain | Rating |
|---|---|
| Perception | ★★★☆☆ |
| Generation | ★★☆☆☆ |
| Attention | — |
| Learning | — |
| Memory | ★★☆☆☆ |
| Reasoning | ★★★★☆ |
| Metacognition | ★★☆☆☆ |
| Executive Function | ★★★☆☆ |
| Problem-Solving | ★★★★☆ |
| Social Cognition | — |

## Detailed Assessment

### Reasoning — L4

The model scored 45 on the Artificial Analysis Intelligence Index (third among open-weight models). Independent evaluator Benjamin Marie benchmarked it on a 750-prompt mixed suite covering LiveCodeBench v6, MMLU Pro, GPQA, and Math500, and it showed a +12-point gain on scientific reasoning in HLE (Humanity's Last Exam). These independent evaluations across multiple integrated tasks indicate practitioner-level reasoning under minimal supervision, warranting an L4 rating.

Sources:
- https://artificialanalysis.ai/articles/qwen3-5-397b-a17b-everything-you-need-to-know
- https://unsloth.ai/docs/models/qwen3.5
- https://venturebeat.com/technology/alibabas-qwen-3-5-397b-a17-beats-its-larger-trillion-parameter-model-at-a

### Problem-Solving — L4

The model achieved ELO 1,221 on GDPval-AA, a third-party frontier agentic evaluation that compares model outputs on realistic knowledge-work tasks such as presentation creation and analysis — a gain of 361 points over Qwen3 235B (860). It also recorded +27 points on TerminalBench Hard and was independently evaluated on LiveCodeBench v6, demonstrating strengths across tasks requiring integration of multiple capabilities including agentic workflows and RAG. These results support practitioner-level integrated problem-solving under minimal supervision, an L4 rating.

Sources:
- https://artificialanalysis.ai/articles/qwen3-5-397b-a17b-everything-you-need-to-know
- https://unsloth.ai/docs/models/qwen3.5
- https://build.nvidia.com/qwen/qwen3.5-397b-a17b/modelcard

### Perception — L3

Third-party sources confirm that this is the first Qwen open-weight model to natively support image and video input. The vendor claims it surpasses the dedicated VL model Qwen3-VL on visual understanding benchmarks, and it employs a Hybrid MoE architecture with early-fusion vision-language training. A published demo answers questions such as "How many porcelain vases were found in the wall niches of the main chamber?" from a video URL. These findings suggest capable multimodal perception beyond the basic assistant level, but independent benchmark figures corroborating autonomous practitioner-level performance are not yet available, leading to an L3 rating.

Sources:
- https://artificialanalysis.ai/articles/qwen3-5-397b-a17b-everything-you-need-to-know
- https://huggingface.co/Qwen/Qwen3.5-397B-A17B
- https://build.nvidia.com/qwen/qwen3.5-397b-a17b/modelcard

### Executive Function — L3

A concrete measurement of goal maintenance is provided by a +28-point score on IFBench (instruction following). The vendor additionally claims support for adaptive tool use and built-in official tools, and training was scaled using reinforcement learning on a progressively more complex task distribution in a million-agent environment. Together these indicate capable execution ability at the supervised junior level, an L3 rating.

Sources:
- https://artificialanalysis.ai/articles/qwen3-5-397b-a17b-everything-you-need-to-know
- https://huggingface.co/Qwen/Qwen3.5-397B-A17B
- https://build.nvidia.com/qwen/qwen3.5-397b-a17b/modelcard

### Generation — L2

Text output capability has been confirmed as a feature by a third-party source (Artificial Analysis), but no benchmarks addressing generation quality or evidence of autonomously producing expert-level output have been presented. Rated L2 accordingly.

Sources:
- https://artificialanalysis.ai/models/qwen3-5-397b-a17b

### Memory — L2

A 262k-token context window has been independently verified, and the vendor claims the hosted Qwen3.5-Plus variant supports a 1M-token context by default. The concrete ability to retain information across long inputs is clear, but no benchmarks corroborate practitioner-level utilization of this memory capacity. Rating remains at the assistant level.

Sources:
- https://artificialanalysis.ai/models/qwen3-5-397b-a17b
- https://huggingface.co/Qwen/Qwen3.5-397B-A17B

### Metacognition — L2

Third-party sources describe the ability to switch between thinking and non-thinking modes within a single model as a concrete feature. However, the AA-Omniscience Index is -32, with a hallucination rate explicitly reported at 88%. This metric measures how often the model answers when it should not — or when it should admit it does not know — indicating weak awareness of its own knowledge state. The functional strength of mode-switching is offset by the inaccuracy of self-knowledge, leaving the rating at L2.

Sources:
- https://artificialanalysis.ai/articles/qwen3-5-397b-a17b-everything-you-need-to-know

---

Attention, Learning, and Social Cognition were excluded from evaluation due to the absence of relevant information in publicly available sources.

Evaluation policy and disclaimer: [Capability Evaluation — Disclaimer]({{ site.baseurl }}/en/archives/2026/04/11/capability-evaluation-disclaimer/)
