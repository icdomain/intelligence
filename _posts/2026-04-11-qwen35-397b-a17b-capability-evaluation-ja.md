---
layout: post
title: Qwen3.5-397B-A17B の能力評価
description: Alibaba Qwen チームが開発した Hybrid MoE マルチモーダル基盤モデル Qwen3.5-397B-A17B の AI 能力評価。推論・問題解決で L4 と評価。
permalink: /ja/archives/2026/04/11/qwen35-397b-a17b-capability-evaluation/
lang: ja
alt_lang_url: /en/archives/2026/04/11/qwen35-397b-a17b-capability-evaluation/
date: 2026-04-11T09:00:00Z
last_modified_at: 2026-04-11T09:00:00Z
author: founder
categories: [strategic-forecasting]
tags: [AI, 能力評価, Qwen, MoE, マルチモーダル, エージェント]
---

**特徴的な能力**: 推論・問題解決
**レベル**: L4

## 概要

Qwen3.5-397B-A17B は、Hybrid Mixture-of-Experts アーキテクチャと early fusion による視覚言語学習を採用したマルチモーダル基盤モデルである。Qwen のオープンウェイトモデルとして初めてネイティブな画像・動画入力に対応し、262k トークンのコンテキストウィンドウ(ホスト版 Qwen3.5-Plus では 1M)を備える。推論モードと非推論モードを単一モデル内で切り替え可能で、チャット、RAG、視覚理解、エージェント型ワークフローなど幅広い用途で最先端性能を狙って設計されている。Artificial Analysis Intelligence Index ではオープンウェイトモデル中 3 位にランクされている。

## 能力評価

| 領域 | 評価 |
|---|---|
| 知覚 | ★★★☆☆ |
| 生成 | ★★☆☆☆ |
| 注意 | — |
| 学習 | — |
| 記憶 | ★★☆☆☆ |
| 推論 | ★★★★☆ |
| メタ認知 | ★★☆☆☆ |
| 実行機能 | ★★★☆☆ |
| 問題解決 | ★★★★☆ |
| 社会的認知 | — |

## 詳細解説

### 推論 — L4

第三者評価である Artificial Analysis Intelligence Index で 45 を獲得し、オープンウェイトモデル中 3 位にランクされている。さらに独立評価者 Benjamin Marie による 750 プロンプトの混合スイート(LiveCodeBench v6、MMLU Pro、GPQA、Math500)でのベンチマーキングが行われており、HLE(Humanity's Last Exam)での科学的推論スコアも +12 ポイントの伸びを示している。これら複数の統合タスクにおける独立評価から、最小限の監督下で実務家レベルの推論を行える水準と判断され、L4 に位置付けられる。

Sources:
- https://artificialanalysis.ai/articles/qwen3-5-397b-a17b-everything-you-need-to-know
- https://unsloth.ai/docs/models/qwen3.5
- https://venturebeat.com/technology/alibabas-qwen-3-5-397b-a17-beats-its-larger-trillion-parameter-model-at-a

### 問題解決 — L4

第三者評価である GDPval-AA で ELO 1,221 を達成しており、これは Qwen3 235B(860)から 361 ポイントもの大幅な向上にあたる。GDPval-AA はプレゼン作成や分析といった現実的な知識労働タスクでモデル出力を比較するフロンティアのエージェント評価である。加えて TerminalBench Hard で +27 ポイント、LiveCodeBench v6 でも独立評価が行われており、エージェント型ワークフローや RAG など複数能力の統合を要するタスク全般で強みを示す。これらから最小限の監督下で実務家レベルの統合的問題解決が可能と判断し、L4 と評価した。

Sources:
- https://artificialanalysis.ai/articles/qwen3-5-397b-a17b-everything-you-need-to-know
- https://unsloth.ai/docs/models/qwen3.5
- https://build.nvidia.com/qwen/qwen3.5-397b-a17b/modelcard

### 知覚 — L3

第三者によって、Qwen のオープンウェイトモデルとして初めてネイティブに画像・動画入力をサポートすることが確認されている。ベンダーは視覚理解ベンチマークにおいて専用 VL モデルである Qwen3-VL を上回ると主張しており、early fusion による視覚言語学習を採用した Hybrid MoE アーキテクチャを備える。動画 URL を入力として「主室の壁龕で発見された磁器の壺はいくつか」といった問いに答えるデモも公開されている。これらは基本的なアシスタントレベルを超えた有能なマルチモーダル知覚を示唆するが、自律的な実務家レベルを裏付ける独立ベンチマーク数値が揃っていないため、L3 と評価した。

Sources:
- https://artificialanalysis.ai/articles/qwen3-5-397b-a17b-everything-you-need-to-know
- https://huggingface.co/Qwen/Qwen3.5-397B-A17B
- https://build.nvidia.com/qwen/qwen3.5-397b-a17b/modelcard

### 実行機能 — L3

IFBench(指示追従)で +28 ポイントというベンチマークスコアにより、目標維持に関する具体的な測定がなされている。これに加えてベンダーは適応的ツール利用と公式組み込みツールへの対応を主張しており、訓練面では million-agent 環境において段階的に複雑化するタスク分布上で強化学習がスケールされている。これらから、監督下のジュニアレベルに相当する有能な実行能力を示すと判断し、L3 とした。

Sources:
- https://artificialanalysis.ai/articles/qwen3-5-397b-a17b-everything-you-need-to-know
- https://huggingface.co/Qwen/Qwen3.5-397B-A17B
- https://build.nvidia.com/qwen/qwen3.5-397b-a17b/modelcard

### 生成 — L2

第三者ソース(Artificial Analysis)によってテキスト出力能力が機能として確認されているものの、生成品質に関するベンチマークや自律的に専門家水準のアウトプットを出せる証拠は提示されていないため、L2 と評価した。

Sources:
- https://artificialanalysis.ai/models/qwen3-5-397b-a17b

### 記憶 — L2

第三者によって 262k トークンのコンテキストウィンドウが確認されており、ベンダーはホスト版 Qwen3.5-Plus でデフォルト 1M コンテキストに対応すると主張している。長大な入力にわたる情報保持の具体的能力は明らかだが、実務家レベルでの記憶活用を裏付けるベンチマークはなく、アシスタントレベルにとどめた。

Sources:
- https://artificialanalysis.ai/models/qwen3-5-397b-a17b
- https://huggingface.co/Qwen/Qwen3.5-397B-A17B

### メタ認知 — L2

第三者により、推論モードと非推論モードを単一モデル内で切り替えられることが具体的機能として記述されている。一方で AA-Omniscience Index は -32 で、ハルシネーション率が 88% と高水準であることが明示的に示されている。この指標は「答えるべきでないとき・知らないと認めるべきときに回答してしまう頻度」を測るもので、自己の知識状態を把握する能力(メタ認知)が弱いことを意味する。モード切替という機能面の強みはあるものの、自己知識の不正確さがそれを相殺するため、L2 にとどめた。

Sources:
- https://artificialanalysis.ai/articles/qwen3-5-397b-a17b-everything-you-need-to-know

---

注意、学習、社会的認知の 3 領域については、公開情報で言及が見当たらず評価対象外とした。

能力評価の方針・免責事項: [能力評価 — 免責事項]({{ site.baseurl }}/ja/archives/2026/04/11/capability-evaluation-disclaimer/)
