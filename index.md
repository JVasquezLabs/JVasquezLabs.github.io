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

In my current role, I lead a product portfolio spanning **borrower experience, loan operations, and sales technology** across purchase, refinance, and HELOC lending — including point-of-sale conversion, automated underwriting, credit workflows, capital markets, and **AI systems that take actions, not just produce outputs**.

My work sits at the intersection of competing constraints: **borrower experience, fulfillment efficiency, credit economics, compliance, investor eligibility, and engineering capacity**.

  </div>
</div>

### My Superpowers
<span class="highlight-pill">AI-Powered Product Development</span> <span class="highlight-pill">Product Org Leadership</span> <span class="highlight-pill">Growth &amp; Experimentation</span>

- **AI-Powered Product Development** — Shipped an agentic underwriting engine and an LLM-powered chat sales assistant, cutting underwriting review time by **50%** and driving a **~40%** conversion improvement across point-of-sale flows.
- **Product Org Leadership** — Own strategy and roadmap for a multi-pod product organization; hire, level, and coach the PM team while partnering with engineering leadership on execution.
- **Growth & Experimentation** — Run A/B and multivariate testing across the funnel; delivered **$6M** in incremental profit and a **9.7%** lift in lead conversion.

### Notable Highlights
- **AI-Powered Underwriting & Loan Automation** — Own product strategy and roadmap for a multi-pod team spanning the B2C lending funnel; manage and coach the PM team while partnering with engineering leadership on execution. Built an agentic loan application workflow, delivered **$6M** in incremental profit, and drove a **~40%** conversion improvement across point-of-sale flows.
- **Growth & Risk Qualification (B2C Lending)** — Increased pre-qualified lead conversion by **9.7%** (an estimated **$400K**/month revenue impact), built an FCRA-compliant risk-qualification flow that enabled **$436M** in securitizations, and increased retention by **7%**.
- **0-to-1 Product Launch (Mortgage Lending)** — First product hire on the team. Launched a 0-to-1 mortgage point-of-sale system and built a mortgage eClosing SaaS platform projected to process **$1.5B**.
- **Regulatory & Compliance Product Strategy** — Delivered a trade compliance reporting solution aligned with European Securities and Markets Authority (ESMA) requirements, and led emergency development of a patient self-service portal that handled 1,200 daily inquiries during the pandemic.

### Building in the Age of AI
AI has made "product manager" and "builder" less distinct roles. I prototype the systems I'm proposing, not just the specs for them, using the same tools I ship to customers.

<img src="https://ghchart.rshah.org/4f46e5/JVasquezLabs" alt="Jonathan Vasquez's GitHub contribution activity" class="github-chart" loading="lazy" onerror="this.style.display='none'; document.getElementById('github-chart-fallback').hidden=false;">
<p id="github-chart-fallback" class="github-projects__status" hidden>Couldn't load live contribution data — <a href="https://github.com/JVasquezLabs">view my GitHub</a> directly.</p>

**Recent Projects**

<div class="case-study-grid" id="github-projects">
  <p class="github-projects__status">Loading recent projects&hellip;</p>
</div>

<script>
(function () {
  var container = document.getElementById('github-projects');
  if (!container) return;

  fetch('https://api.github.com/users/JVasquezLabs/repos?sort=pushed&per_page=10')
    .then(function (res) {
      if (!res.ok) throw new Error('GitHub API error');
      return res.json();
    })
    .then(function (repos) {
      var featured = repos
        .filter(function (r) { return !r.fork && r.name.toLowerCase() !== 'jvasquezlabs.github.io'; })
        .slice(0, 3);

      if (!featured.length) {
        container.innerHTML = '<p class="github-projects__status">No public projects to show right now &mdash; <a href="https://github.com/JVasquezLabs">visit my GitHub</a>.</p>';
        return;
      }

      container.innerHTML = featured.map(function (r) {
        var name = r.name.replace(/[&<>]/g, function (c) { return { '&': '&amp;', '<': '&lt;', '>': '&gt;' }[c]; });
        var desc = (r.description || 'No description provided.').replace(/[&<>]/g, function (c) { return { '&': '&amp;', '<': '&lt;', '>': '&gt;' }[c]; });
        var updated = new Date(r.pushed_at).toLocaleDateString('en-US', { year: 'numeric', month: 'short' });
        var langPill = r.language ? '<span class="category-pill">' + r.language + '</span>' : '';
        return '<div class="case-study-card">' + langPill +
          '<h3><a href="' + r.html_url + '" target="_blank" rel="noopener noreferrer">' + name + '</a></h3>' +
          '<p>' + desc + '</p>' +
          '<p class="project-card__meta">Updated ' + updated + '</p>' +
          '</div>';
      }).join('');
    })
    .catch(function () {
      container.innerHTML = '<p class="github-projects__status">Couldn\'t load live project data &mdash; <a href="https://github.com/JVasquezLabs">view my GitHub</a> directly.</p>';
    });
})();
</script>

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

