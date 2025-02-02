---
layout: single
title: "A little bit about me..."
permalink: /
header:
  overlay_image: /assets/images/header-bg.jpg  # Add an image here
  overlay_filter: rgba(0, 0, 0, 0.5)  # Dark overlay for readability
  #caption: "Transforming Real Estate and FinTech Through Innovation"
---

I’m a **Product Leader** with a strong track record of leading **0-to-1 product launches**, scaling **digital experiences**, and driving **customer engagement** across **FinTech, PropTech, and Retail** industries. My unique background blends **technical expertise, real estate experience, and product strategy** to deliver high-impact solutions that transform how businesses operate.


### **🔹 My Superpowers**
- **📈 Data-Driven Growth**: Leveraged **A/B testing, cohort analysis, and LTV/CAC modeling** to optimize onboarding and increase retention.
- **⚙️ Workflow Automation**: Designed **self-service tools** that reduced operational friction by **20%** and cut underwriting time by **4 hours per loan**.
- **🤝 Cross-Functional Leadership**: Proven ability to collaborate across **engineering, UX, compliance, and business teams** to execute **high-ROI product roadmaps**.

### **🏆 Notable Highlights**
- **Product @ Hometap (B2C)**  
  → **Optimized user onboarding**, increasing **retention by 7%**, and delivered **self-guided workflows** that reduced user friction by **20%**.  

- **Product @ Beeline (B2B/B2C)**  
  → First US-based Product hire. Launched **Mortgage POS System (0-1)**, improving efficiency by **15%**, and built **TILES (mortgage eClosing SaaS platform)**, driving **$1.5B in projected transactions**.  

- **Slalom Consulting**  
  →  Delivered a **trade compliance reporting** solution aligned with European Securities and Markets Authority (ESMA) requirements, led emergency development of a **patient self-service portal** to handle COVID-19-related queries, successfully managing 1,200 daily inquiries during the pandemic.

  ### **📢 Let’s Connect**
I’m passionate about **using data, technology, and automation** to solve **complex business problems**. Let’s chat about how we can **redefine financial services** together!  
📧 [jonathan@jvasquez.net](mailto:jonathan@jvasquez.net) | [LinkedIn](https://www.linkedin.com/in/jonathanjvasquez)

---
## **📂 Case Studies**

<table>
  <thead>
    <tr>
      <th>Case Study</th>
      <th>Key Takeaways</th>
    </tr>
  </thead>
  <tbody>
    {% for post in site.posts limit:5 %}
    <tr>
      <td><a href="{{ post.url | relative_url }}">{{ post.title }}</a></td>
      <td>{{ post.excerpt | strip_html }}</td>
    </tr>
    {% endfor %}
  </tbody>
</table>

