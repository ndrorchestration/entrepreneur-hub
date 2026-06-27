# TODO — Entrepreneur Hub

**Last updated:** 2026-06-27 (SWEEP-EH-004)  
**Owner:** Human operator + Amethyst  
**Status key:** 🔴 BLOCKING · 🟡 HIGH · 🟢 DONE · ⬜ QUEUED

---

## 🔴 BLOCKING — Do These Now

### 1. Create Needle Project "Entrepreneur Hub"
**Time:** ~5 min  
**Who:** Human operator (Needle account access required)  
**Unblocks:** T-EH-05 publish, Phase 1 gate, LinkedIn launch post, all revenue paths  
**Instruction:** Log in to Needle → New Project → Name: "Entrepreneur Hub" → Save  
**After:** Pass the project URL back to Amethyst to update NEEDLE_TEMPLATE_INDEX

---

### 2. Publish T-EH-05 on Needle
**Time:** ~15 min  
**Who:** Human operator  
**Blocked by:** Item 1 above  
**Instruction:**
- Open `templates/governance-starter-pack/TEMPLATE.md`
- Copy full content
- Create new template in Needle project "Entrepreneur Hub"
- Paste content, set title: "Entrepreneur's AI Governance Starter Pack"
- Set tags: governance, AI, entrepreneur, DGAF, audit, startup
- Publish
- Copy the live URL → pass to Amethyst  
**After:** Amethyst updates NEEDLE_TEMPLATE_INDEX + triggers LinkedIn post prep

---

### 3. Create Gumroad Enterprise Starter Page
**Time:** ~20 min  
**Who:** Human operator  
**Product name:** "AI Governance Enterprise Starter"  
**Price:** $199  
**Description:** See `docs/GUMROAD_PRODUCT_SPEC.md`  
**After:** Update README inquiry CTA link from GitHub Issues to Gumroad URL. Pass URL to Amethyst.

---

## 🟡 HIGH — Do These After Blockers Clear

### 4. Add Needle CTA to All 12 Active Governance Workflows
**Time:** ~24 min (~2 min each)  
**Who:** Human operator (Needle account access required)  
**CTA block to paste at TOP of each workflow description:**
```
---
🏗️ Built with DGAF Framework — 33+ governance patterns for agentic AI systems.
→ Full ecosystem: github.com/ndrorchestration/entrepreneur-hub
→ Enterprise Starter ($199): governance spec + 1hr async consult
   → github.com/ndrorchestration/entrepreneur-hub/issues/new
→ LinkedIn: linkedin.com/in/andrewhensel
---
```
**Workflows requiring CTA (12 total):**
1. Governed Agentic Parliament
2. [Governed] Kernel Evaluation Workflow
3. [Governed] KB Answer + Quality Check
4. [Governed] LLM Output Evaluator & Hallucination Checker
5. [Governed] Knowledge Base Q&A
6. [Governed] Dynamic Governance Agentic Formation (DGAF)
7. AOGA Dashboard Workflow
8. Curvature-Aware Governance Router
9. [Governed] Semantic Contamination Checker
10. [Governed] Constitutional AI Policy Validator
11. [Governed] Agent Performance Audit
12. Task Completion Query

**Impact:** 11K+ monthly views → zero conversion path today. This is the single highest-leverage ~24 min action available.

---

### 5. Publish LinkedIn Launch Post
**Time:** ~5 min  
**Who:** Human operator  
**Blocked by:** T-EH-05 live on Needle (need URL)  
**File:** `docs/LAUNCH_POST_LINKEDIN.md` — post is fully drafted. Replace `[Link to Needle template]` with live URL then publish.  
**Target:** +500 views, ≥1 GitHub star, ≥1 Enterprise Starter inquiry

---

### 6. Review IP Risk — GOV-005
**Time:** ~15 min  
**Who:** Human operator  
**Flagged by:** SWEEP-EH-004 (2026-06-27)  
**Key decisions needed:**
- Move `docs/GUMROAD_PRODUCT_SPEC.md` to private repo or strip pricing detail?
- Is Apache 2.0 the right license if DGAF patterns are intended as proprietary?
- Make `governance/` a private submodule?

---

## ⬜ QUEUED — Phase 1 Completion

- [ ] Update NEEDLE_TEMPLATE_INDEX with live URLs once T-EH-01–05 approved by Needle
- [ ] Replace GitHub Issues CTA with Gumroad URL once Gumroad page is live
- [ ] Verify GitHub Actions sweep-reminder.yml fires on first Wednesday
- [ ] Check GitHub Traffic → Referrers at Day 7 post-launch
- [ ] Update 12 CTA blocks once Gumroad URL is live (replace issues/new with Gumroad link)
- [ ] Run AOGA Dashboard Workflow verified run (clear ⚠️ flag in NEEDLE_WORKFLOW_REGISTRY)

---

## 🟢 DONE

- [x] Phase 0 closed (2026-06-25)
- [x] README rewritten as storefront (2026-06-25)
- [x] T-EH-05 full content build — 6 files (2026-06-26)
- [x] T-EH-01 content build (2026-06-26)
- [x] T-EH-02 content build (2026-06-26)
- [x] T-EH-03 content build (2026-06-26)
- [x] T-EH-04 content build (2026-06-26)
- [x] GitHub Actions SWEEP forcing function added (2026-06-25)
- [x] LinkedIn launch post drafted (2026-06-26)
- [x] Gumroad product spec written (2026-06-25)
- [x] AUDIT_TRAIL schema v1.1 with funnel_source (2026-06-26)
- [x] SWEEP-EH-002 completed (2026-06-25)
- [x] SWEEP-EH-003 completed (2026-06-26)
- [x] T-EH-01 submitted to Needle Partner Hub — Pending review (2026-06-27)
- [x] T-EH-02 submitted to Needle Partner Hub — Pending review (2026-06-27)
- [x] T-EH-03 submitted to Needle Partner Hub — Pending review (2026-06-27, syntax fix applied)
- [x] T-EH-04 submitted to Needle Partner Hub — Pending review (2026-06-27)
- [x] GOV-004 logged in AUDIT_TRAIL.md (2026-06-27)
- [x] GOV-005 logged in AUDIT_TRAIL.md — IP risk flag (2026-06-27)
- [x] SWEEP-EH-004 completed + logged in SWEEP_LOG.md (2026-06-27)
- [x] NEEDLE_WORKFLOW_REGISTRY.md created — all 12 workflows catalogued (2026-06-27)
- [x] 5 IP risk exposure areas identified and documented in GOV-005 (2026-06-27)
