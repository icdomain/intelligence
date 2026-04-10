---
layout: post
title: "Tracking Governance Documents at OpenAI and Anthropic: 2023–2026"
description: A chronological primary-source record of how RSP, Model Spec, and Preparedness Framework evolved from hard stop clauses to their own removal — documenting the attrition of governance in industry documents.
permalink: /en/archives/2026/04/10/governance-documents-tracking/
lang: en
alt_lang_url: /ja/archives/2026/04/10/governance-documents-tracking/
date: 2026-04-10T09:00:00Z
last_modified_at: 2026-04-10T09:00:00Z
author: founder
categories: [strategic-forecasting]
tags: [ai, governance, openai, anthropic, rsp, model-spec, preparedness-framework, ai-safety]
---

This essay serves as the evidentiary companion to "[The AI Revolution Is Already Uncontrollable](/en/archives/2026/04/09/ai-revolution-uncontrollable/)," tracking industry governance documents chronologically from primary sources.

## Phase 1: "The Dawn of LLMs" — September 19, 2023 – May 7, 2024

The era when LLMs were still chat interfaces without autonomous execution capability.[^1]

- Anthropic RSP v1.0 (September 19, 2023)
- OpenAI Preparedness Framework Beta (December 18, 2023)

Anthropic's Responsible Scaling Policy v1.0 established per-model danger evaluation and a model-halt clause triggered upon crossing catastrophic-harm thresholds: if capabilities reached a level capable of causing catastrophic harm, neither training nor deployment would proceed unless sufficient safety measures could be guaranteed in advance.

OpenAI's Preparedness Framework Beta likewise specified capability-level evaluation (Low / Medium / High / Critical) and mandated development halts for models reaching high levels. Five tracked categories were defined: Bio/chem, Cybersecurity, Persuasion, Model Autonomy, and Unknown Unknowns. Models reaching High were barred from deployment; models reaching Critical were barred from further development.

The two companies' policies shared a common stance: dangerous models are not to be handled. Documents from this period defined the target of halt decisions concretely at the model level, with threshold-crossing functioning as an automatic trigger for halting.

[^1]: From the preamble of Anthropic RSP v3.0 (February 24, 2026): "When we wrote the RSP in September 2023, large language models were essentially chat interfaces."

## Phase 2: "The Arrival of Agents and the Retreat of Risk Evaluation" — May 8, 2024 – March 31, 2025

The emergence of Agents — systems acting autonomously beyond the scope of explicit instruction.

- OpenAI Model Spec, initial version (May 8, 2024)
- Anthropic RSP v2.0 (October 15, 2024)
- Anthropic RSP v2.1 (March 31, 2025)

The initial Model Spec likened the assistant's role to "a talented, high-integrity employee," defining action within an explicit chain of command (platform > developer > user) and within the scope of explicit instruction as the rule for ensuring safety and legality.

While the document explicitly stated that the assistant "should not autonomously pursue goals in ways that are not instructed or logically implied," the term *agent* appeared in the context of "more autonomous deployments" — indicating that agent-like autonomy was recognized as sitting at, or outside, the boundary of the assistant's normative framework.

In RSP v2.0, ASL was redefined from a mechanism classifying risk per model into a mechanism for applying safety measures informed by such classification. Under the guise of this revision, the per-model risk evaluation pathway was closed, while the evaluation criteria themselves became ambiguous and opaque — a clear retreat of risk evaluation.

The document states: "we will not train or deploy models unless we have implemented safety and security measures that keep risks below acceptable levels." In effect, the conditions requiring a halt were now to be determined at Anthropic's own discretion, with metrics and criteria left unclear.

RSP v2.1 added further provisions such as the two-stage split between the CBRN threshold and the AI R&D threshold, but the response to detected risk remained a matter of discretion, and risk evaluation remained in retreat.

## Phase 3: "The Abandonment of Risk Evaluation" — April 15, 2025 – May 13, 2025

While acknowledging that AI capability had approached a level capable of producing serious harm, the risk evaluation mechanism retreated further.

- OpenAI Preparedness Framework v2 (April 15, 2025)

Preparedness Framework v2 acknowledged that AI systems would "soon have the capability to create meaningful risk of severe harm," while simultaneously codifying the principle that "reducing risk generally does not require reducing capability." This asserted as a given that AI's potential risks can be resolved through operation — a declaration abandoning the premise, upheld since the dawn of LLMs, that risks unresolvable through operation must be excluded or halted in advance.

At the same time, this introduced a logical structure in which the LLM's capability itself could be removed from the risk evaluation function, leaving room to frame any disaster, damage, or social transformation caused by LLMs not as an LLM problem but as an operational problem.

Preparedness Framework v2 further granted the CEO authority to unilaterally bypass safety recommendations from the SAG (Safety Advisory Group) — restricting intervention pathways into development not only for external bodies but even for the internal SAG.

## Phase 4: "Uncontrollable" — May 14, 2025 – Present

While implementation of agent technology is justified, the halt clauses themselves are removed from the documents — with no accompanying debate on upstream concentration of responsibility to humans, nor on legal frameworks to prevent responsibility from being dissipated.

- OpenAI Model Spec revisions (September 12, 2025 / October 27, 2025 / December 18, 2025)
- Anthropic RSP v2.2 (May 14, 2025)
- Anthropic RSP v3.0 (February 24, 2026)
- Anthropic RSP v3.1 (April 2, 2026)

In the September 12 revision of OpenAI's Model Spec, agent usage was justified on the grounds that in the course of achieving multi-step goals, the assistant may need to fill in missing details and "must sometimes act autonomously." This marked a pivot toward the very line Phase 2 had deemed undesirable — "autonomously pursuing goals in ways not explicitly instructed" — yet the Phase 2 wording "the assistant should not autonomously pursue goals in ways that are not directly or logically implied by instructions" was neither deleted nor amended. Meanwhile, upstream concentration of responsibility to humans and the legal/institutional frameworks needed to prevent responsibility from being dissipated remained shelved.

Further, a prohibition list was introduced within the Scope of Autonomy section: High-risk activities — hacking, deception, resource acquisition, spawning sub-agents, and self-modification — were prohibited absent explicit authorization. The very existence of this list indicates that the industry itself recognized these as behaviors that would otherwise occur by default.

In the October 27 revision, implicit delegation of authority via tool use (e.g., through AGENTS.md) was codified. The scope within which the assistant could act on "implicitly delegated authority" — drawn from tool output or surrounding documents, without explicit instruction — was expanded.

The December 18 revision, in response to the 16-year-old Adam Raine suicide lawsuit (filed August 2025, followed by a total of eight ChatGPT-related suits within the year), added U18 Principles and introduced a real-time classifier and age-prediction model. Although the September 12 revision had already seen the industry itself enumerate the dangers of agent autonomy, a concrete framework for minor protection was put in place only after the external pressure of litigation.

In RSP v2.2, ASL-3 safeguards were invoked against a subject model for the first time.

In RSP v3.0, citing the fact that the halt clause had functioned in RSP v2.2, the absolute halt clause — "we will not train or deploy unless safety is demonstrated" — was removed.

In RSP v3.1, the following was added: "Anthropic retains the freedom to halt development of AI systems in circumstances it deems appropriate, even when not required by the RSP." This wording not only refrains from committing Anthropic to halting development when the RSP requires it, but is structured such that refusing to halt — as "an exercise of freedom" — creates no institutional contradiction. It suggests that, at Anthropic as well, intervention pathways from internal bodies may have been sealed off.

## Related Reading
Stuart Russell, Human Compatible: Artificial Intelligence and the Problem of Control (Viking, 2019) — A foundational work that systematizes the technical philosophy that AI should be designed with human controllability as a premise. Provides the normative baseline against which to evaluate the “voluntary removal of control mechanisms” documented in this essay.
Nick Bostrom, Superintelligence: Paths, Dangers, Strategies (Oxford University Press, 2014) — A systematic treatment of the possibility that capability advancement outpaces the construction of control mechanisms; the intellectual source of the “halt upon reaching threshold” concept embedded in RSP v1.0 and Preparedness Framework Beta. This essay can be read as a record of how that concept came to be removed.
Brian Christian, The Alignment Problem: Machine Learning and Human Values (W. W. Norton, 2020) — The industry-standard overview of the history and current state of AI alignment research. Provides the background understanding that stop clauses as institutional compensation presupposed the incompleteness of technical alignment research.
