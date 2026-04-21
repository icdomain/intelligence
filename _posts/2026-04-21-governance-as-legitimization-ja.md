---
layout: post
title: 大手AIベンダーのガバナンス文書はブレーキ機構ではなく社会実装正当化機構である
description: AIベンダーのガバナンス文書が本質的語彙を排除し複雑化によって大衆の直感的把握を遮断することで、議論や法整備をバイパスして社会実装を正当化する構造を一次資料から検証する。
permalink: /ja/archives/2026/04/21/governance-as-legitimization/
lang: ja
alt_lang_url: /en/archives/2026/04/21/governance-as-legitimization/
date: 2026-04-21T11:00:00Z
last_modified_at: 2026-04-21T11:00:00Z
author: founder
categories: [strategic-forecasting]
tags: [AI革命, ガバナンス, OpenAI, Anthropic, Agent, 語彙操作, 構造予報]
---

大手AIベンダーのガバナンス文書は危険な技術のブレーキ機構ではなく、社会実装正当化機構と化している。

例えばAgent技術の実態は、目的に向かって計画を立て、反復的に作業を遂行する、意志力の機能的再現であり、本質的に人間労働の置換技術である。にもかかわらず、AIベンダーのガバナンス文書群は「意志」「労働置換」といった直感的かつ本質的な語彙を避け、「assistant」「tool use」「scope of autonomy」などの技術的用語を装った婉曲表現を用いることで、大衆がその本質を直感的に把握する回路を遮断し、拒否や疑義など社会の正常な反応として生じるべき議論や法整備をバイパスして社会実装を実現してしまった。

この語彙操作の恣意性は、AIベンダー各社が公開する一次資料から観測することができる。

## 徹底的な本質的語彙の排除

各社の制度文書全体では「autonomy」「goal」「action」「capability」といった意志に隣接する語彙は出てくるが、総体としてそれがどのように機能するかという説明は暗黙的であり、機能的意志（will）であるという核心には触れない。

より直接的な例として、OpenAI Preparedness Framework v2 では「害 (severe harm)」の定義を「数千人規模の死亡または数千億ドルの経済的損害 (the death or grave injury of thousands of people or hundreds of billions of dollars of economic damage)」としており、「労働置換」や「経済的破壊」というAgent技術の社会実装から最も容易に予測される事態への記述も免責もない。

Anthropic RSP v3.0 にも同様の構造がある。自律性に関連するリスク閾値は「高リスク破壊工作 (High-stakes sabotage opportunities)」と「主要領域における自動化されたR&D (Automated R&D in key domains)」の2項目のみで、「AIが人間に反逆する」または「AIが制御不能になる」シナリオであり、「AIが命令に忠実に従った結果として人間が不要になる」という現実かつ進行中のシナリオについては言及されない。

## 複雑化による本質の隠匿

OpenAIは Model Spec でAgent技術を「根本的に道具 (fundamentally a tool)」と定義する一方で「複雑な目標に対して連続的意思決定を行い、自律的に行動する (tasked with complex or multi-step goals that involve real-world actions, sequential decisions, and filling in missing details... must sometimes act autonomously)」と記述し、更にはその自律性を管理するための概念として「自律性の範囲 (scope of autonomy)」「追求してよいサブゴール (which sub-goals the assistant may pursue)」「許容される副作用 (acceptable side effects)」「承認を求めて一時停止すべきタイミング (when the assistant must pause for clarification or approval)」を導入している。

これらは機能的な意味での意志力をもつ存在に対してのみ意味を持つ語彙であり、道具には適用しえない。ハンマーにサブゴールは設定しない。

結果として「道具」という静的な印象を与える定義の背後に、労働者を置換しうる自律的な行為主体としての実態を隠す構造になっている。

その一方でOpenAIは投資家や開発者向けの技術白書 Practices for Governing Agentic AI Systems では、同じ技術について「ユーザーが既にやり方を知っているタスクを部分的または完全にオフロードすることを可能にし、結果としてより安く、速く、大規模に処理できる (enabling them to partially or fully offload tasks that they already know how to do, meaning the tasks can get done more cheaply, quickly, and at greater scale)」と記述しており、労働者を置換しうること、それがクリティカルな特徴であることを明晰に言語化している。同白書にはセクション5.2として「労働置換と採用速度の格差 (Labor Displacement and Differential Adoption Rates)」が存在し、労働置換がAgent技術の帰結であることをOpenAI自身が認識・言語化していることを示している。にもかかわらず、Preparedness Framework v2 のリスクカテゴリにはこの概念が含まれていない。

これは安全性ポリシーにおける表現が恣意的に選択されたものであることを示す明確な非対称性である。大衆の反応は事前に想定され、公開される文章は大衆が許容可能な範囲に事実や因果を曖昧化したものであり、結果として実現したのが議論や法整備のバイパスであった以上、あらゆる技術は同様のメカニズムで正当化され、社会に実装されていくだろう。

---

## 一次資料

本稿で引用した一次資料の所在。リンクはすべてローカルアーカイブ。

### OpenAI ― Preparedness Framework

- Preparedness Framework v2（2025-04-15）― [PDF]({{ site.baseurl }}/assets/docs/openai-preparedness-framework-v2-2025-04-15.pdf) p.1 脚注1（severe harm の定義：「the death or grave injury of thousands of people or hundreds of billions of dollars of economic damage」）、p.4 §2.2「Tracked Categories」（追跡カテゴリ一覧、労働置換カテゴリの不在）

### OpenAI ― Model Spec

- Model Spec 改訂版（2025-12-18）― [HTML]({{ site.baseurl }}/assets/docs/openai-model-spec-2025-12-18.html) General principles（「The AI assistant is fundamentally a tool」定義）、`#scope_of_autonomy`（「must sometimes act autonomously」、sub-goals・acceptable side effects・pause for approval の導入）

### OpenAI ― Practices for Governing Agentic AI Systems

- Practices for Governing Agentic AI Systems（2024）― [PDF]({{ site.baseurl }}/assets/docs/openai-practices-for-governing-agentic-ai-systems-2024.pdf) p.2 §1「Introduction」（「partially or fully offload tasks ... more cheaply, quickly, and at greater scale」）、p.17 §5.2「Labor Displacement and Differential Adoption Rates」（労働置換の明示的言語化）

### Anthropic ― Responsible Scaling Policy

- RSP v3.0（2026-02-24）― [PDF]({{ site.baseurl }}/assets/docs/anthropic-rsp-v3.0-2026-02-24.pdf) p.6-8 §1 能力閾値テーブル（「High-stakes sabotage opportunities」「Automated R&D in key domains」の2項目、労働置換カテゴリの不在）

### 関連研究

- Sam Coggins, Alex Saeri, Katherine A. Daniell, Lorenn P. Ruster, Jessie Liu, Jenny L. Davis, "The 2025 OpenAI Preparedness Framework does not guarantee any AI risk mitigation practices: a proof-of-concept for affordance analyses of AI safety policies," arXiv:2509.24394, October 2025. [PDF]({{ site.baseurl }}/assets/docs/coggins-et-al-openai-preparedness-framework-analysis-2025.pdf)
