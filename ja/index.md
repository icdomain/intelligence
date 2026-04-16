---
layout: default
title: Independent Compute Domain
description: Independent Compute Domain 公式サイト
permalink: /ja/
lang: ja
alt_lang_url: /en/
date: 2026-04-08
last_modified_at: 2026-04-08
author: founder
---

# Independent Compute Domain Intelligence Bureau

ICD諜報局は構造的な未来予報と情報リテラシー教育を通じて、人々の思想的自立と主体的判断力の醸成を目的とする組織です。

<img src="{{ site.baseurl }}/emblem.png" alt="ICD Emblem" class="emblem-hero">

## セクション

- [構造予報]({{ site.baseurl }}/ja/strategic-forecasting/)
- [AI時代の情報リテラシー]({{ site.baseurl }}/ja/information-discernment/)
- [アーカイブ]({{ site.baseurl }}/ja/archives/)

## 最新の記事

{% assign latest = site.posts | where: "lang", "ja" | sort: "date" | reverse %}
{% for post in latest limit:3 %}
- [{{ post.title }}]({{ post.url | prepend: site.baseurl }}) <time>{{ post.date | date: "%Y-%m-%d" }}</time>
{% endfor %}


## ICDIBコンテンツの禁止利用行為
ICDは、事前の書面による許可なく、そのコンテンツに対するスクレイピング、取り込み、複製、要約、翻案、変形、再配布、AI学習への利用、または派生利用を明確に禁止します。これには、再投稿、スクリプト化、ならびにYouTubeその他のプラットフォームへのアップロードを含みます。
