---
layout: single
title: "Case Studies | Jonathan Vasquez"
permalink: /case-studies/
---

## **📂 Case Studies**
🔍 Below is a collection of **detailed case studies** showcasing my expertise in **FinTech, PropTech, and Product Management**.

Each case study includes **key insights, workflow optimizations, and product strategies** that drove real business impact.

---

{% for post in site.posts %}
### **[{{ post.title }}]({{ post.url | relative_url }})**
📝 **Summary:** {{ post.excerpt | strip_html }}  
🔗 [Read Full Case Study →]({{ post.url | relative_url }})

---
{% endfor %}

