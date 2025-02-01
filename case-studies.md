---
layout: single
title: "Case Studies"
permalink: /case-studies/
---

<style>
@import url('{{ "/css/custom.css" | relative_url }}');
</style>

# 📂 Case Studies

Explore real-world examples of **product management success**, including workflow automation, fintech innovation, and customer experience improvements.

{% for post in site.posts %}
<div class="case-study">
  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
  <p>{{ post.excerpt }}</p>
  <a href="{{ post.url | relative_url }}" class="read-more">Read More →</a>
</div>
<hr>
{% endfor %}
