---
layout: post
title: "Automating Loan Underwriting with an AI Agent at MegaLoans"
date: 2026-06-01
categories: [Fintech, Product Management]
excerpt: "How an AI underwriting agent automated income, employment, and residency verification, cutting review time by 50%, scaling capacity to 1,000 loans a month, and driving a ~40% lift in conversion."
toc: true
toc_sticky: true
---

<div class="stat-row">
  <div class="stat-tile"><span class="stat-tile__number">50%</span><span class="stat-tile__label">Faster underwriting review</span></div>
  <div class="stat-tile"><span class="stat-tile__number">1,000/mo</span><span class="stat-tile__label">Loan processing capacity</span></div>
  <div class="stat-tile"><span class="stat-tile__number">~40%</span><span class="stat-tile__label">Conversion lift</span></div>
  <div class="stat-tile"><span class="stat-tile__number">$6M</span><span class="stat-tile__label">Incremental profit</span></div>
</div>

## Background
After modernizing the appraisal workflow and redesigning the agent portal, MegaLoans turned its automation focus to the loan application itself: the manual verification work sitting between a borrower applying and a processor issuing a pre-approval.

---

## Problem Statement
### Key Challenge: Manual Document Collection and Verification
- Borrowers manually uploaded pay stubs and bank statements to prove income and assets.
- Processors manually requested missing documents and manually created conditions — the outstanding items required before a loan could move forward.
- This created delays in origination and initial quoting, and when income wasn't verified correctly upfront, it surfaced as rework and inaccurate quotes later in the process.

---

## Approach
I owned strategy and requirements for an AI underwriting agent that automates income, employment, and residency verification, and built early prototypes to validate the approach. Engineering and data science built and trained the production system.

### How the Agent Works
- **Direct data verification** — Pulls income and employment data from payroll providers (Argyle), asset and bank data from Plaid, and identity/residency data from Persona, instead of relying on borrower-uploaded documents.
- **GSE guidelines as the baseline** — Evaluates each case against standard GSE guidelines, with custom exception-handling rules layered on top for cases those guidelines don't cleanly resolve.
- **Tiered handoff, not a binary pass/fail** — When the agent can fully clear income, employment, and residency, it issues an end-to-end automated pre-approval. When it can't, it doesn't just reject the case: some are flagged for a human to verify the agent's finding, others are routed to a human to complete the step manually.

### Guardrails
- **Exception-handling monitoring** to catch and route edge cases rather than let them fail silently.
- **Live feedback loop** — Users can flag how the agent performed on a given task in real time, which the team used to monitor accuracy and prioritize fixes, especially when document formats changed or new edge cases showed up.
- The system went through an AI security review before launch.

---

## Results & Impact
- **Reduced underwriting review time by 50%**, freeing up processor capacity.
- **Scaled processing capacity to 1,000 loans per month.**
- **Drove a ~40% improvement in conversion** across point-of-sale flows, largely from faster time-to-pre-approval.
- **Delivered $6M in incremental profit** through the combination of cost reduction and new revenue.

---

## Key Learnings
- **Automation isn't binary.** The highest-leverage design decision wasn't "automate or don't" — it was building three distinct paths (auto-approve, human-verify, human-complete) instead of forcing every edge case into a single fallback.
- **Live feedback is what makes an agent maintainable.** Without a way for users to flag bad outcomes in real time, drift in document formats or edge cases would have gone undetected until it showed up in downstream metrics.
- **Directing an AI build is a different skill than shipping a feature.** Owning strategy and requirements while engineering and data science built the model meant translating ambiguous edge cases into rules a model could act on — and knowing when to route to a human instead of forcing full automation.

---

## Conclusion
This initiative built on the appraisal workflow and agent portal work that came before it, extending MegaLoans' automation further upstream into the application and underwriting process itself. Together, the three initiatives reflect a multi-year push to remove manual bottlenecks across the borrower journey, while treating human review as a deliberate design choice rather than a fallback.
