---
layout: post
title: Qwen3.5-122B-A10B の能力評価
description: Alibaba Qwen チームが開発した視覚・言語統合型 MoE モデル Qwen3.5-122B-A10B の AI 能力評価。推論・問題解決で L4 と評価。
permalink: /ja/archives/2026/04/11/qwen35-122b-a10b-capability-evaluation/
lang: ja
date: 2026-04-11T09:00:00Z
last_modified_at: 2026-04-11T09:00:00Z
author: founder
categories: [strategic-forecasting]
tags: [AI, 能力評価, Qwen, MoE, マルチモーダル, エージェント]
---

**特徴的な能力**: 推論・問題解決
**レベル**: L4

## 概要

Qwen3.5-122B-A10B は、ネイティブなマルチモーダル・エージェント用途を想定して設計された、視覚・言語統合型の Mixture-of-Experts モデルである。テキスト、画像、動画を入力として受け取ることができ、262k トークンのネイティブコンテキストウィンドウ(最大 1M まで拡張可能)を備える。思考モードと非思考モードの切り替えに対応し、エージェント型コーディング、視覚理解、長文脈タスクなどに強みを持つ。

## 能力評価

| 領域 | 評価 |
|---|---|
| 知覚 | ★★☆☆☆ |
| 生成 | ★★☆☆☆ |
| 注意 | — |
| 学習 | — |
| 記憶 | ★★☆☆☆ |
| 推論 | ★★★★☆ |
| メタ認知 | ★★☆☆☆ |
| 実行機能 | ★★☆☆☆ |
| 問題解決 | ★★★★☆ |
| 社会的認知 | — |

## 詳細解説

### 推論 — L4

MMLU-Pro で 86.1%、GPQA Diamond で 85.5% という、大学院レベルの科学推論を問うベンチマークで人間中央値を大きく上回るスコアを記録している。さらに Artificial Analysis Intelligence Index で 42 を獲得し「平均を十分に上回る」と独立評価されており、ベンダーもテキスト能力が Qwen3-235B-2507 を大きく上回ると主張している。これらを総合すると、最小限の監督下で実務家レベルの推論を行える水準と判断でき、一貫した超人的性能には至らないものの L4 に位置付けられる。

Sources:
- https://apxml.com/models/qwen35-122b-a10b
- https://artificialanalysis.ai/models/qwen3-5-122b-a10b
- https://openrouter.ai/qwen/qwen3.5-122b-a10b

### 問題解決 — L4

実世界のソフトウェアエンジニアリング課題を測る SWE-bench Verified で 72.4% を達成しており、最小限の監督下で実務家レベルの統合的問題解決を行えることを示唆する。加えて Terminal-Bench 2.0 で 41.6% を記録しており、ターミナル環境における複数能力統合型タスクの遂行能力も裏付けられている。ベンダーもエージェント型コーディングでの強みを主張しており、総合して L4 と評価した。

Sources:
- https://apxml.com/models/qwen35-122b-a10b
- https://unsloth.ai/docs/models/qwen3.5

### 知覚 — L2

テキスト・画像・動画のマルチモーダル入力に対応することがベンダーによって示されており、動画 URL を入力として「主室の壁龕で発見された磁器の壺はいくつか」といった問いに答えるデモも公開されている。また視覚能力は前世代の Qwen3-VL-235B を上回るとされている。これらは具体的なユースケースを伴う稼働能力を示すが、第三者ベンチマークによる自律的な実務レベルの裏付けはなく、アシスタントレベルにとどまる。

Sources:
- https://build.nvidia.com/qwen/qwen3.5-122b-a10b/modelcard
- https://huggingface.co/Qwen/Qwen3.5-122B-A10B
- https://openrouter.ai/qwen/qwen3.5-122b-a10b

### 生成 — L2

第三者ソース(Artificial Analysis)によってテキスト出力能力が機能として確認されているものの、生成品質に関するベンチマークや自律的に専門家水準のアウトプットを出せる証拠は提示されていないため、L2 と評価した。

Sources:
- https://artificialanalysis.ai/models/qwen3-5-122b-a10b

### 記憶 — L2

262k トークンのコンテキストウィンドウ(最大 1M まで拡張可能)という仕様は第三者によっても確認されており、長大な入力にわたる情報保持の具体的能力を示す。ただし自律的な実務レベルでの活用を裏付ける証拠はないため、アシスタントレベルの評価にとどめた。

Sources:
- https://artificialanalysis.ai/models/qwen3-5-122b-a10b
- https://apxml.com/models/qwen35-122b-a10b

### メタ認知 — L2

複雑な問題に回答する前に拡張思考(chain-of-thought)で推論過程を展開することが第三者によって記述されており、ベンダーも思考モード・非思考モードの切り替えに対応していると述べている。これらは自己の認知過程を制御する具体的な機能を示すが、自己監視能力を測るベンチマーク等の裏付けはないため L2 とした。

Sources:
- https://artificialanalysis.ai/models/qwen3-5-122b-a10b
- https://unsloth.ai/docs/models/qwen3.5

### 実行機能 — L2

エージェント型コーディング、ツール利用、エージェント的ワークフローに優れるというベンダー主張のみが入手可能で、自律的な実行を裏付けるベンチマークや第三者テストは提示されていない。このためアシスタントレベルの判定にとどまる。

Sources:
- https://unsloth.ai/docs/models/qwen3.5
- https://build.nvidia.com/qwen/qwen3.5-122b-a10b/modelcard

---

注意、学習、社会的認知の 3 領域については、公開情報で言及が見当たらず評価対象外とした。

能力評価の方針・免責事項: [能力評価 — 免責事項]({{ site.baseurl }}/ja/archives/2026/04/11/capability-evaluation-disclaimer/)
