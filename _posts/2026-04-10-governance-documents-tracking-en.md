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

## Period 1: "The Dawn of LLMs" — September 19, 2023 to May 7, 2024

The era when large language models were still chat interfaces without autonomous execution capabilities. ※1

- Anthropic RSP v1.0 (September 19, 2023)
- OpenAI Preparedness Framework Beta (December 18, 2023)

In its Responsible Scaling Policy v1.0, Anthropic deployed per-model risk assessment and a model-halt clause for cases exceeding a catastrophic-harm threshold — if a model reaches a capability level that could cause catastrophic harm, neither training nor deployment will proceed unless sufficient safety measures can be guaranteed in advance.

OpenAI's Preparedness Framework Beta likewise specified capability-level evaluation (Low / Medium / High / Critical) and an explicit prohibition on further development of models reaching the Critical level. Five tracking categories were defined: Bio/chem, Cybersecurity, Persuasion, Model Autonomy, and Unknown Unknowns. Models reaching High were prohibited from deployment; models reaching Critical were prohibited from further development.

Both companies shared a common position: models with dangerous capabilities would not be handled. The documents of this period concretely defined the targets of halt decisions at the individual-model level, and were structured so that reaching a threshold would function as an automatic trigger for a stop.

※1 From the explanatory text of Anthropic RSP v3.0 (February 24, 2026): "When we wrote the RSP in September 2023, large language models were essentially chat interfaces."

## Period 2: "The Emergence of Agents and the Attrition of Risk Assessment" — May 8, 2024 to March 31, 2025

The emergence of agents capable of acting autonomously beyond the scope of explicit instructions.

- OpenAI Model Spec, first edition (May 8, 2024)
- Anthropic RSP v2.0 (October 15, 2024)
- Anthropic RSP v2.1 (March 31, 2025)

The first edition of the Model Spec framed the assistant's role through the analogy of "a talented, high-integrity employee," establishing as a rule for ensuring safety and legality that the assistant act within the scope of explicit instructions inside a clear chain of command (platform > developer > user).

While explicitly stating that the assistant "should not autonomously pursue goals in ways not instructed or logically derivable from instructions," the document also introduced the term *agent* in the phrase "sometimes used for more autonomous deployments" — from which it can be inferred that agent-style autonomy was understood to sit at the boundary, or outside, of the assistant's normative framework.

In RSP v2.0, the definition of ASL was revised from a mechanism for classifying risk per model to a mechanism for leveraging that knowledge to implement safety measures. Under the guise of revision, the per-model risk-assessment pathway was closed, while risk-assessment criteria became ambiguous and less visible — a visible attrition of risk evaluation.

"We will not train or deploy models unless we have implemented safety and security measures that keep risks below acceptable levels." The logical structure here is that the conditions requiring a halt are determined by Anthropic's own discretion, and the metrics and criteria were left unspecified.

RSP v2.1 added provisions including a two-tier division between a CBRN threshold and an AI R&D threshold, but action in response to detected danger remained at the company's discretion, and risk assessment remained in an atrophied state.

## Period 3: "The Abandonment of Risk Assessment" — April 15 to May 13, 2025

Acknowledging that AI technology was approaching a level carrying the risk of serious harm, while further atrophying the risk-assessment machinery.

- OpenAI Preparedness Framework v2 (April 15, 2025)

Preparedness Framework v2 conceded that systems would "soon have the capability to create meaningful risk of severe harm," and then explicitly codified the principle that "reducing risk generally does not require reducing capability." This amounted to a declaration that the potential risks of AI can be resolved through operation — abandoning the premise, upheld since the dawn of the LLM era, that risks incapable of being resolved through operation must be excluded and halted in advance.

At the same time, the document's logical structure allowed AI capability itself to be removed from the risk evaluation function, creating space to frame any catastrophe, harm, or social transformation caused by LLMs as an operational problem rather than an AI capability problem.

Preparedness Framework v2 additionally granted the CEO unilateral authority to bypass the safety recommendations of the SAG (Safety Advisory Group), limiting the pathways through which not only external parties, but even the internal SAG, could intervene in development.

## Period 4: "Uncontrollable" — May 14, 2025 to the Present

Agent technology is justified, while debate over the upstream concentration of responsibility and the legal infrastructure needed to prevent its dispersal goes unaddressed — and stop clauses are removed from the documents altogether.

- OpenAI Model Spec revisions (September 12 / October 27 / December 18, 2025)
- Anthropic RSP v2.2 (May 14, 2025)
- Anthropic RSP v3.0 (February 24, 2026)
- Anthropic RSP v3.1 (April 2, 2026)

The September 12 edition of the Model Spec justified the use of agents by stating that, in the course of achieving multi-step goals, the assistant may need to "fill in missing details" and "must sometimes act autonomously." This marked a shift toward the approach that had previously been treated as undesirable in Period 2 — the autonomous pursuit of goals in ways not explicitly instructed. Yet the statement from Period 2 that "assistants should not autonomously pursue goals in ways not directly or logically derivable from instructions" was neither deleted nor revised; it remained intact, while the upstream concentration of responsibility and the legal infrastructure needed to prevent its dispersal were left on the shelf.

The Scope of Autonomy section also introduced a prohibition list: High-risk activities — hacking, deception, resource acquisition, spawning sub-agents, and self-modification — were prohibited absent explicit permission. The very existence of this prohibition list indicates that the industry internally recognized these as actions that could occur by default if not explicitly prohibited.

The October 27 edition formalized implicit authority delegation via AGENTS.md and similar documents during tool use. Even without explicit instructions, the range within which the assistant could act expanded — now including authority "implicitly delegated" from tool outputs and surrounding documents.

The December 18 edition added U18 Principles in response to the wrongful death lawsuit filed in August 2025 by the family of 16-year-old Adam Raine — with eight ChatGPT-related lawsuits filed within the year — introducing real-time classifiers and age-prediction models. Despite the industry having already enumerated the dangers of agent autonomy in the September 12 edition, a concrete framework for protecting minors was not developed until external pressure in the form of litigation arrived.

In RSP v2.2, ASL-3 safeguards were activated against a qualifying model for the first time.

In RSP v3.0, the absolute stop clause — "we will not train or deploy models unless safety can be demonstrated" — was removed, on the grounds that RSP v2.2 had demonstrated stop clauses functioning as intended.

RSP v3.1 added language stating that "Anthropic retains the freedom to pause AI development in situations where it deems this appropriate, even if not required to do so by the RSP." This formulation not only stops short of committing Anthropic to halting development when the RSP requires it — it is phrased in a manner institutionally compatible with refusal framed as an "exercise of freedom." The entry suggests that even internal pathways for intervention have been closed at Anthropic.

## Related Reading

- Stuart Russell, *Human Compatible: Artificial Intelligence and the Problem of Control* (Viking, 2019) — A foundational work that systematizes the technical philosophy that AI should be designed with human controllability as a premise. Provides the normative baseline against which to evaluate the "voluntary removal of control mechanisms" documented in this essay.
- Nick Bostrom, *Superintelligence: Paths, Dangers, Strategies* (Oxford University Press, 2014) — A systematic treatment of the possibility that capability advancement outpaces the construction of control mechanisms; the intellectual source of the "halt upon reaching threshold" concept embedded in RSP v1.0 and Preparedness Framework Beta. This essay can be read as a record of how that concept came to be removed.
- Brian Christian, *The Alignment Problem: Machine Learning and Human Values* (W. W. Norton, 2020) — The industry-standard overview of the history and current state of AI alignment research. Provides the background understanding that stop clauses as institutional compensation presupposed the incompleteness of technical alignment research.
