---
layout: default
title: Independent Compute Domain
description: Official site of the Independent Compute Domain
permalink: /en/
lang: en
alt_lang_url: /ja/
date: 2026-04-08
last_modified_at: 2026-04-08
author: founder
---

# Independent Compute Domain Intelligence Bureau

The ICD Intelligence Bureau is an organization dedicated to fostering intellectual independence and the capacity for autonomous judgment — through structural forecasting and information literacy education.

## Sections

- [Strategic Forecasting]({{ site.baseurl }}/en/strategic-forecasting/)
- [Information Discernment]({{ site.baseurl }}/en/information-discernment/)
- [Archives]({{ site.baseurl }}/en/archives/)

## Latest posts

{% assign latest = site.posts | where: "lang", "en" | sort: "date" | reverse %}
{% for post in latest limit:3 %}
- [{{ post.title }}]({{ post.url | prepend: site.baseurl }}) <time>{{ post.date | date: "%Y-%m-%d" }}</time>
{% endfor %}

## Prohibited Uses of ICD Content
ICD expressly prohibits any scraping, ingestion, reproduction, summarization, adaptation, transformation, redistribution, AI training, or derivative use of its content without prior written permission. This includes reposting, script generation, and uploads to platforms such as YouTube.
