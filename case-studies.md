---
layout: page
title: "Case Studies"
permalink: /case-studies/
---

# 📂 Case Studies

Real-world examples of **product management success**, including workflow automation, fintech innovation, and customer experience improvements.

{% for post in site.posts %}
- **[{{ post.title }}]({{ post.url }})** - {{ post.excerpt }}
{% endfor %}
