---
layout: single
title: "Case Studies"
permalink: /case-studies/
---

Case studies in FinTech, PropTech, and Product Management. Each shows the insights, workflow optimizations, and product strategies that drove real business impact.

<ul class="case-study-grid">
  {% for post in site.posts %}
  <li class="case-study-card">
    <span class="category-pill">{{ post.categories | first }}</span>
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p>{{ post.excerpt | strip_html }}</p>
  </li>
  {% endfor %}
</ul>

