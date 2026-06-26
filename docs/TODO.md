# TODO — Entrepreneur Hub

**Last updated:** 2026-06-26 (SWEEP-EH-003)  
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
**Description:** See docs/GUMROAD_PRODUCT_SPEC.md  
**After:** Update README inquiry CTA link from GitHub Issues to Gumroad URL. Pass URL to Amethyst.

---

## 🟡 HIGH — Do These After Blockers Clear

### 4. Add Needle CTA to 6 Existing Governance Workflows
**Time:** ~30 min  
**Who:** Human operator  
**CTA text to add (bottom of each workflow):**  
```
> Built with DGAF Framework — full AI governance toolkit for entrepreneurs  
> → [Entrepreneur Hub on GitHub](https://github.com/ndrorchestration/entrepreneur-hub)
```
**Impact:** Activates existing 11K view audience. Single highest-leverage traffic action.

---

### 5. Publish LinkedIn Launch Post
**Time:** ~5 min  
**Who:** Human operator  
**Blocked by:** T-EH-05 live on Needle (need URL)  
**File:** docs/LAUNCH_POST_LINKEDIN.md — post is drafted, replace `[Link to Needle template]` with live URL  
**Target:** +500 views, ≥1 GitHub star, ≥1 Enterprise Starter inquiry

---

## ⬜ QUEUED — Phase 1 Completion

- [ ] Publish T-EH-01 through T-EH-04 on Needle (after T-EH-05 is live)
- [ ] Update NEEDLE_TEMPLATE_INDEX with all live URLs
- [ ] Verify GitHub Actions sweep-reminder.yml fires on first Wednesday
- [ ] Check GitHub Traffic → Referrers at Day 7 post-launch

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
