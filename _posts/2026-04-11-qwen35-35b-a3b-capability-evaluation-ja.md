---
layout: post
title: Qwen3.5-35B-A3B の能力評価
description: Alibaba Qwen チームが開発したマルチモーダル MoE モデル Qwen3.5-35B-A3B の AI 能力評価。知覚・推論・問題解決で L3 と評価。
permalink: /ja/archives/2026/04/11/qwen35-35b-a3b-capability-evaluation/
lang: ja
alt_lang_url: /en/archives/2026/04/11/qwen35-35b-a3b-capability-evaluation/
date: 2026-04-11T09:00:00Z
last_modified_at: 2026-04-11T09:00:00Z
author: founder
categories: [strategic-forecasting]
tags: [AI, 能力評価, Qwen, MoE, マルチモーダル, エージェント]
---

**特徴的な能力**: 知覚・推論・問題解決
**レベル**: L3

## 概要

Qwen3.5-35B-A3B は、マルチモーダルトークンに対する early fusion 訓練を採用した統合型ビジョン言語基盤モデルである。201 言語と画像・動画を含むマルチモーダル入力に対応し、ネイティブで 262,144 トークンのコンテキスト長をサポートする(ホスト版 Qwen3.5-Flash ではデフォルト 1M)。思考モードと非思考モードの切替に対応し、エージェント型コーディング、視覚理解、長文脈タスクで強みを示す。Artificial Analysis Intelligence Index では 37 を獲得し、比較対象モデル中で平均を十分に上回る位置にある。

## 能力評価

| 領域 | 評価 |
|---|---|
| 知覚 | ★★★☆☆ |
| 生成 | ★★☆☆☆ |
| 注意 | — |
| 学習 | — |
| 記憶 | ★★☆☆☆ |
| 推論 | ★★★☆☆ |
| メタ認知 | ★★☆☆☆ |
| 実行機能 | ★★☆☆☆ |
| 問題解決 | ★★★☆☆ |
| 社会的認知 | — |

## 詳細解説

### 知覚 — L3

第三者によって、201 言語と画像・動画を含むマルチモーダル入力への対応が確認されている。さらに Overshoot というデプロイ事例では、連続するライブ動画に対して 200ms 未満で推論を実行している実例があり、実用環境における具体的な知覚処理能力が裏付けられている。ベンダーは early fusion 訓練による統合型ビジョン言語基盤として、視覚理解ベンチマークで専用 VL モデルである Qwen3-VL を上回ると主張している。これらから基本的なアシスタントレベルを超える実用的な知覚能力を示すと判断し、L3 と評価した。

Sources:
- https://huggingface.co/Qwen/Qwen3.5-35B-A3B/discussions/43
- https://www.millstoneai.com/inference-benchmark/qwen3-5-35b-a3b-fp8
- https://huggingface.co/Qwen/Qwen3.5-35B-A3B

### 推論 — L3

第三者評価である Artificial Analysis Intelligence Index で 37 を獲得し、比較可能なモデル中で平均を十分に上回る位置にある。また数学・コーディング・多言語ベンチマークにおいて、Qwen3-235B-A22B のようなはるかに大規模なモデルと競合する性能を示すとの第三者評価もある。これらから訓練生からジュニアレベルに相当する推論能力を有すると判断し、L3 とした。

Sources:
- https://artificialanalysis.ai/models/qwen3-5-35b-a3b
- https://www.millstoneai.com/inference-benchmark/qwen3-5-35b-a3b-fp8

### 問題解決 — L3

単一のアーキテクチャ仕様書を Claude Code 経由で渡したところ、10 ファイル・3,483 行のコードを足場組みし、衝突判定のバグを自己デバッグして、初回読み込みで動作するゲームをサーブしたというデモ事例がある。これは推論・計画・コーディング・自己修正を統合した、現実的タスクにおける具体的な問題解決を示している。複数ファイルにまたがる自律的エージェント型コーディングの事例として、訓練生からジュニアレベルに相当する統合的問題解決能力を裏付けるが、独立したベンチマークによる自律的実務家水準の確認はないため L3 にとどめた。

Sources:
- https://agentnativedev.medium.com/qwen-3-5-35b-a3b-why-your-800-gpu-just-became-a-frontier-class-ai-workstation-63cc4d4ebac1

### 生成 — L2

第三者ソース(Artificial Analysis)によってテキスト出力能力が機能として確認されているものの、生成品質に関するベンチマークや専門家水準のアウトプットを示す証拠は提示されていないため、L2 と評価した。

Sources:
- https://artificialanalysis.ai/models/qwen3-5-35b-a3b

### 記憶 — L2

ベンダーはネイティブで 262,144 トークンのコンテキスト長に対応すると主張しており、ホスト版 Qwen3.5-Flash ではデフォルトで 1M トークンまで拡張できるとしている。長大な入力にわたる情報保持の具体的能力は明らかだが、独立した実務家レベルの記憶活用ベンチマークはなく、アシスタントレベルにとどめた。

Sources:
- https://lmstudio.ai/models/qwen/qwen3.5-35b-a3b
- https://huggingface.co/Qwen/Qwen3.5-35B-A3B

### メタ認知 — L2

ベンダーは思考モードと非思考モードの切替に対応していると述べており、また自身のコードの衝突判定バグを検知して修正したというデモ事例も存在する。これらは認知過程の制御と自己出力の評価という具体的な機能を示すが、自己知識を測る第三者テストやベンチマークによる裏付けはないため L2 とした。

Sources:
- https://unsloth.ai/docs/models/qwen3.5
- https://agentnativedev.medium.com/qwen-3-5-35b-a3b-why-your-800-gpu-just-became-a-frontier-class-ai-workstation-63cc4d4ebac1

### 実行機能 — L2

エージェント型コーディングでの優位性、million-agent 環境における強化学習、ツール呼び出し性能の改善というベンダー主張のみが入手可能で、自律的な実行を裏付けるベンチマークや第三者テストは提示されていない。このためアシスタントレベルの判定にとどめた。

Sources:
- https://unsloth.ai/docs/models/qwen3.5
- https://huggingface.co/unsloth/Qwen3.5-35B-A3B-GGUF
- https://lmstudio.ai/models/qwen/qwen3.5-35b-a3b

---

注意、学習、社会的認知の 3 領域については、公開情報で言及が見当たらず評価対象外とした。

能力評価の方針・免責事項: [能力評価 — 免責事項]({{ site.baseurl }}/ja/archives/2026/04/11/capability-evaluation-disclaimer/)
