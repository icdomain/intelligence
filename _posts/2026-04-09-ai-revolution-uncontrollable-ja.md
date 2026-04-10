---
layout: post
title: AI革命はすでにアンコントローラブルである
description: Model SpecやResponsible Scaling Policyなどの正当化文書と機能不全の規制が組み合わさって、AI開発の現状追認機構として作動している構造を解剖する。
permalink: /ja/archives/2026/04/09/ai-revolution-uncontrollable/
lang: ja
alt_lang_url: /en/archives/2026/04/09/ai-revolution-uncontrollable/
date: 2026-04-09T09:00:00Z
last_modified_at: 2026-04-09T09:00:00Z
author: founder
categories: [strategic-forecasting]
tags: [AI, ガバナンス, 責任, エージェント, AI安全性]
---

メディアが倫理的権威のように扱うModel SpecおよびPreparedness Framework(OpenAI)、Responsible Scaling Policy(Anthropic)などの文書、あるいはEU AI Actのような規制的枠組みの実態は、開発当事者自らが編集した名ばかりのガバナンス文書と、抑止能力を欠いた規制の組み合わせである。

社会的には倫理的権威やAI開発がコントローラブルであることを示す事例として引用されるこれらのソースは、各所で生まれた技術を、その意味や危険性を想起しにくい婉曲表現に言い換え、企業の影響力を背景とした宣伝によって社会的合意に見せかけることで、大衆の反発を防ぐ現状追認機構と化している。彼らが語るのは倫理的にやるべきかどうかではなく、いかに運用するべきかという運用問題への論点のすり替えであり、そもそも安全な運用が成立するという前提の内在化を強制する。

Agent技術に関連の文書においては、AIが命令の行使者から理想の実装者へ変化していく過程を通じて運用による制御の不可能性を内部では把握しながら、表面上は運用問題として扱い続ける様子が観察できる。

OpenAIが2025年4月に公開したPreparedness Framework v2では、AIシステムはエージェント化が進みつつあり、まもなく「soon have the capability to create meaningful risk of severe harm」(OpenAI Preparedness Framework v2)——深刻な危害リスクを生む能力を持つに至る——と明記されている。業界自身が、深刻な危害を生む水準に「近い」ことを公式文書の中で認めている。

しかしこの認識に対する文書の応答は、開発の停止ではなく「信頼できるsafeguardsを設計・展開する」という方向であった。深刻な危害リスクを認知した直後、議題は即座に運用問題——safeguardsの設計——へと移されている。

つまりこの文書は、次の2つを同じページの中で同時に主張している。第一に、AIは深刻な危害を生む水準に近づいている。第二に、それは運用で管理可能である。前者を認めた瞬間、後者は論理的に成立困難となる。にもかかわらず両者は併存しているのである。これは自律性の進展により運用制御が理論上不可能となる領域へ既に入りつつあることを内部で認めながら、その認識を運用問題の語彙で包むことで社会的に前進可能な形式へ変換したことを示す一次資料となるだろう。

AI革命初期から業界文書が提示してきた役割分担——人間が戦略判断と設計(orchestrator)を担い、AIが実装(implementer)を担うという物語もすでに崩壊しつつある。この構造から必然的に導かれる論理的帰結、すなわち責任の上流への集中と法整備の必要性について、社会では対策も議論も進まないまま責任をAIに押し付けて霧散させるというスキームが常態化している。

第一に、個別オペレーターの層。OpenAIはNYT訴訟において、法的証拠保全義務下にあった学習データをエンジニアが「誤って」削除し、その「意図せず」が法廷で現に免責根拠として機能した。責任意識が最も高まるべき法的文脈ですら、個別人間の監督は破綻している。

第二に、自律エージェントの層。OpenAI Codex所属のエンジニアNik Pashが個人で構築した自律トレーディングボット「Lobstar Wilde」は、稼働3日目にAPI応答の読み違えにより$441,788相当のトークンを一発で誤送金した。注目すべきは、Pash本人が事件後に「エージェントにはガードレールを付けるな、何をしてはいけないかを書くな、personalityとhungerを与えろ」と公に表明している点である。業界最前線の実装者の設計思想そのものが、正当化文書における「human oversight」「guardrails」の語彙と正面から矛盾しており、実装現場と制度文書の乖離が露呈している。

第三に、組織プロセスの層。自らを「safety-first AI lab」と位置づけ、Responsible Scaling Policyによって倫理機関的権威を自己付与しているAnthropicは、2026年3月26日にCMS設定ミスで未公開モデル「Mythos」を含む約3,000の内部アセットを公開データレイクに露出させ、その5日後の3月31日にはClaude Codeのnpmパッケージに混入したソースマップから約512,000行のソースコードを公開レジストリに流出させた。両方とも公式見解は「human error、security breachではない」である。自社の内部プロセスすら統制できない組織が、業界の安全基準を書いている。

これらは個人・自律エージェント・組織プロセス——それぞれの層における「意図せずやってしまった、悪意はないから責任も限定される」というスキームの実地作動例である。

社会は人間への責任追及ではなく、AIの運用問題へと事態をフレーミングし、当初の物語——実装の責任を命令者が担う——からの乖離が常態化している。これでは人が担うのは、意思決定と責任ではなく、権力と、その権力を後ろ盾とした責任の発散に収束するだろう。

人の価値までもが権威に収束する世界で大衆はどのように生きろというのだろうか?

→ 本稿の論拠となるガバナンス文書の一次資料追跡は「[OpenAIとAnthropicにおけるガバナンス文書の追跡 2023-2026](/ja/archives/2026/04/10/governance-documents-tracking/)」を参照。

## 関連書籍

以下の文献に本稿の論旨と重なる議論を見ることができる。

- Ulrich Beck, *Risk Society: Towards a New Modernity* (Sage, 1992; 原著ドイツ語1986) ― 近代社会が新興技術リスクに対して「組織化された無責任(organized irresponsibility)」という構造を制度化していることを論じた古典。本稿の「責任の発散」とほぼ同一の概念を、AI以前に一般化された形で提示している。
- Diane Vaughan, *The Challenger Launch Decision: Risky Technology, Culture, and Deviance at NASA* (University of Chicago Press, 1996) ― NASAがチャレンジャー事故に至るまで、当初は許容不可能とされていたリスクを段階的に「許容可能」と再定義していった過程を「逸脱の正常化(normalization of deviance)」として概念化した研究。本稿が時系列で追った正当化文書の後退線と構造的に同型。
- Sheila Jasanoff, *The Ethics of Invention: Technology and the Human Future* (W. W. Norton, 2016) ― 技術ガバナンスが多くの場合、技術の事前抑制ではなく事後的正当化として機能してきた歴史を、複数の事例を通じて論じた研究。本稿の「正当化文書=制度許可フォーマット」という診断の理論的背景。
- Dan McQuillan, *Resisting AI: An Anti-fascist Approach to Artificial Intelligence* (Bristol University Press, 2022) ― AI倫理の制度化が、規制ではなく実装の正当化機構として機能していることを正面から論じた近年の代表的批判。本稿の「現状追認機構」という診断と最も直接的に重なる。
