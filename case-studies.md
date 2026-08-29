---
layout: single
title: "Case Studies"
permalink: /case-studies/
---

Below is a collection of detailed case studies showcasing my expertise in **FinTech, PropTech, and Product Management** — each with the key insights, workflow optimizations, and product strategies that drove real business impact.

<ul class="case-study-grid">
  {% for post in site.posts %}
  <li class="case-study-card">
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p>{{ post.excerpt | strip_html }}</p>
  </li>
  {% endfor %}
</ul>

