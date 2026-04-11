---
layout: post
title: Capability Evaluation — Qwen3.5-122B-A10B
description: Capability evaluation of Qwen3.5-122B-A10B, a vision-language MoE model developed by the Alibaba Qwen team. Rated L4 in reasoning and problem-solving.
permalink: /en/archives/2026/04/11/qwen35-122b-a10b-capability-evaluation/
lang: en
alt_lang_url: /ja/archives/2026/04/11/qwen35-122b-a10b-capability-evaluation/
date: 2026-04-11T09:00:00Z
last_modified_at: 2026-04-11T09:00:00Z
author: founder
categories: [strategic-forecasting]
tags: [AI, capability evaluation, Qwen, MoE, multimodal, agent]
---

**Signature capability**: Reasoning & Problem-Solving
**Level**: L4

## Overview

Qwen3.5-122B-A10B is a vision-language Mixture-of-Experts model designed natively for multimodal and agentic use cases. It accepts text, image, and video inputs, and features a 262k-token native context window (extensible up to 1M). It supports switching between thinking and non-thinking modes, with particular strengths in agentic coding, visual understanding, and long-context tasks.

## Capability Ratings

| Domain | Rating |
|---|---|
| Perception | ★★☆☆☆ |
| Generation | ★★☆☆☆ |
| Attention | — |
| Learning | — |
| Memory | ★★☆☆☆ |
| Reasoning | ★★★★☆ |
| Metacognition | ★★☆☆☆ |
| Executive Function | ★★☆☆☆ |
| Problem-Solving | ★★★★☆ |
| Social Cognition | — |

## Detailed Assessment

### Reasoning — L4

The model records scores well above the human median on graduate-level science reasoning benchmarks: 86.1% on MMLU-Pro and 85.5% on GPQA Diamond. It also achieved 42 on the Artificial Analysis Intelligence Index, rated "well above average" by independent evaluators, and the vendor claims its text capabilities substantially exceed those of Qwen3-235B-2507. Taken together, these results indicate practitioner-level reasoning under minimal supervision. While consistent superhuman performance has not been demonstrated, an L4 rating is warranted.

Sources:
- https://apxml.com/models/qwen35-122b-a10b
- https://artificialanalysis.ai/models/qwen3-5-122b-a10b
- https://openrouter.ai/qwen/qwen3.5-122b-a10b

### Problem-Solving — L4

The model achieves 72.4% on SWE-bench Verified, a benchmark measuring real-world software engineering tasks, suggesting practitioner-level integrated problem-solving under minimal supervision. It also records 41.6% on Terminal-Bench 2.0, corroborating the ability to execute multi-capability tasks in terminal environments. The vendor highlights agentic coding as a key strength. Combined, these results support an L4 rating.

Sources:
- https://apxml.com/models/qwen35-122b-a10b
- https://unsloth.ai/docs/models/qwen3.5

### Perception — L2

The vendor demonstrates multimodal input support for text, image, and video, including a published demo answering questions such as "How many porcelain vases were found in the wall niches of the main chamber?" from a video URL. Visual capabilities are reported to exceed those of the prior-generation Qwen3-VL-235B. These findings demonstrate operational capability with concrete use cases, but independent benchmark evidence of autonomous practitioner-level performance is absent; the rating remains at the assistant level.

Sources:
- https://build.nvidia.com/qwen/qwen3.5-122b-a10b/modelcard
- https://huggingface.co/Qwen/Qwen3.5-122B-A10B
- https://openrouter.ai/qwen/qwen3.5-122b-a10b

### Generation — L2

Text output capability has been confirmed as a feature by a third-party source (Artificial Analysis), but no benchmarks addressing generation quality or evidence of autonomously producing expert-level output have been presented. Rated L2 accordingly.

Sources:
- https://artificialanalysis.ai/models/qwen3-5-122b-a10b

### Memory — L2

The 262k-token context window (extensible to 1M) has been independently verified and represents a concrete capability for retaining information across long inputs. However, evidence supporting autonomous practitioner-level utilization of this capacity is absent, so the rating remains at the assistant level.

Sources:
- https://artificialanalysis.ai/models/qwen3-5-122b-a10b
- https://apxml.com/models/qwen35-122b-a10b

### Metacognition — L2

Third-party sources describe the model expanding its reasoning process via extended thinking (chain-of-thought) before answering complex questions, and the vendor confirms support for toggling between thinking and non-thinking modes. These represent concrete mechanisms for controlling one's own cognitive process, but no benchmarks measuring self-monitoring ability have been provided. Rated L2.

Sources:
- https://artificialanalysis.ai/models/qwen3-5-122b-a10b
- https://unsloth.ai/docs/models/qwen3.5

### Executive Function — L2

Only vendor claims are available regarding strengths in agentic coding, tool use, and agentic workflows; no benchmarks or third-party tests corroborating autonomous execution have been presented. The rating remains at the assistant level.

Sources:
- https://unsloth.ai/docs/models/qwen3.5
- https://build.nvidia.com/qwen/qwen3.5-122b-a10b/modelcard

---

Attention, Learning, and Social Cognition were excluded from evaluation due to the absence of relevant information in publicly available sources.

Evaluation policy and disclaimer: [Capability Evaluation — Disclaimer]({{ site.baseurl }}/en/archives/2026/04/11/capability-evaluation-disclaimer/)
