---
layout: default
title: Strategic Forecasting
description: Strategic forecasting reports and analyses from the Independent Compute Domain
permalink: /en/strategic-forecasting/
lang: en
alt_lang_url: /ja/strategic-forecasting/
date: 2026-04-08
last_modified_at: 2026-04-08
author: founder
---

# Strategic Forecasting

## Background Note for Reading the Future Amid the AI Revolution

{% for post in site.posts %}
  {% if post.lang == "en" and post.url contains "ai-revolution-reading-future" %}
<article class="pinned-post">
<h3>{{ post.title }}</h3>
<p>In the AI development race, the United States faces a structural disadvantage against China in terms of the scale of personal and biometric data accumulation and the ease of social implementation and experimentation. Maintaining its hegemonic position makes it difficult to choose to slow development, and the market is considered potentially prone to running out of control.</p>
<p><a href="{{ post.url | prepend: site.baseurl }}">→ Full article……</a></p>
</article>
  {% endif %}
{% endfor %}

{% for post in site.posts %}
  {% if post.lang == "en" and post.url contains "ai-revolution-uncontrollable" %}
<article class="pinned-post">
<h3>{{ post.title }}</h3>
<p>The AI revolution is already uncontrollable. Documents such as Model Spec, Preparedness Framework, Responsible Scaling Policy, and the EU AI Act are cited as ethical authorities, while in reality they combine governance documents authored by the developers themselves with regulations stripped of any deterrent power — functioning as a machinery that affirms the status quo.</p>
<p><a href="{{ post.url | prepend: site.baseurl }}">→ Full article……</a></p>
</article>
  {% endif %}
{% endfor %}

---

## All posts

{% assign posts = site.posts | where: "lang", "en" | where_exp: "post", "post.categories contains 'strategic-forecasting'" | sort: "date" | reverse %}
{% for post in posts %}
- <time>{{ post.date | date: "%Y-%m-%d" }}</time> [{{ post.title }}]({{ post.url | prepend: site.baseurl }})
  {{ post.description }}
{% endfor %}
