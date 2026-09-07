---
layout: single
title: "Product Leadership in FinTech & AI"
permalink: /
header:
  overlay_image: /assets/images/header-bg.jpg  # Add an image here
  overlay_filter: "linear-gradient(135deg, rgba(15, 23, 42, 0.75), rgba(79, 70, 229, 0.45))"
  #caption: "Transforming Real Estate and FinTech Through Innovation"
---

<div class="profile-intro">
  <img src="/assets/images/profile.jpg" alt="Jonathan Vasquez" class="profile-photo">
  <div class="profile-intro__text" markdown="1">

I lead a product portfolio spanning borrower experience, loan operations, and sales technology across purchase, refinance, and HELOC lending. This includes point-of-sale conversion, automated underwriting, credit workflows, capital markets, and AI systems that take actions, not just produce outputs.

The work sits at the intersection of competing constraints: borrower experience, fulfillment efficiency, credit economics, compliance, investor eligibility, and engineering capacity.

  </div>
</div>

### My Superpowers
<span class="highlight-pill">AI-Powered Product Development</span> <span class="highlight-pill">Product Org Leadership</span> <span class="highlight-pill">Growth &amp; Experimentation</span>

- **AI-Powered Product Development**: Shipped an agentic underwriting engine and LLM-powered chat assistant that cut review time by 50% and improved conversion by ~40%.
- **Product Org Leadership**: Own strategy and roadmap for multi-pod organization. Hire, level, and coach PM team while partnering with engineering on execution.
- **Growth & Experimentation**: Run A/B and multivariate testing. Delivered $6M in incremental profit and 9.7% conversion lift.

### Notable Highlights
- **AI-Powered Underwriting & Loan Automation**: Built agentic loan application workflow for multi-pod team. Delivered $6M profit and ~40% conversion lift.
- **Growth & Risk Qualification**: Increased lead conversion 9.7% ($400K/month impact). Built FCRA-compliant risk-qualification flow that enabled $436M securitizations and 7% retention lift.
- **0-to-1 Mortgage Lending**: Launched mortgage point-of-sale system and eClosing platform projected to process $1.5B.
- **Regulatory & Compliance**: Delivered trade compliance reporting solution aligned with ESMA requirements. Built patient self-service portal handling 1,200 daily inquiries during pandemic.

### What I'm Building Now
Agentic underwriting system that reads documents, calculates income, and acts on its output—advancing files and requesting documents without human involvement. Multi-AUS routing strategy for mortgage lending that evaluates loans across multiple systems to optimize outcomes. Home equity product line is funded and expanding partnerships.

### What Matters Most
I build for real business outcomes in regulated industries where constraints are features, not friction. Product decisions live at the intersection of borrower experience, capital markets, compliance, and engineering capacity. I care more about moving metrics that matter than shipping features. Good product leadership means hiring people smarter than you and getting out of their way.
### Let's Connect
I care about building products that move real business metrics, not just ship features. If you're tackling hard problems in fintech, proptech, or AI-driven decisioning, let's talk.

📧 [jonathan@jvasquez.net](mailto:jonathan@jvasquez.net) &nbsp;|&nbsp; [LinkedIn](https://www.linkedin.com/in/jonathanjvasquez)

---
## Case Studies

<ul class="case-study-grid">
  {% for post in site.posts limit:5 %}
  <li class="case-study-card">
    <span class="category-pill">{{ post.categories | first }}</span>
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p>{{ post.excerpt | strip_html }}</p>
  </li>
  {% endfor %}
</ul>

