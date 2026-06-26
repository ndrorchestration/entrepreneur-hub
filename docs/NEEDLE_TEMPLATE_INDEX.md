# Needle Template Index — Entrepreneur Hub

**Maintained by:** COLLEEN-L5  
**Last SWEEP:** June 26, 2026 (SWEEP-EH-003)  
**Registry policy:** All entries require `template_id`, `risk_tier`, `needle_link`, `github_spec_path`, `release_date`, `policy_id`.

> ✅ **SWEEP-EH-003 (June 26, 2026):** All 5 T-EH templates are now content-built and committed to `main`.  
> Status upgraded from scaffolded stubs to `pending-publish`.  
> T-EH-05 is publish-ready — blocked only on Needle project creation (manual action, ~5 min).  
> Once Needle URL is received, update T-EH-05 row and trigger LinkedIn launch post.  
> **Next required SWEEP:** July 3, 2026.

---

## Active Templates

| ID | Name | Risk Tier | Needle Link | Spec Path | Build Status | Policy | COLLEEN Status |
|---|---|---|---|---|---|---|---|
| T-EH-05 | **Entrepreneur's AI Governance Starter Pack** | Medium | *(pending Needle project creation)* | templates/governance-starter-pack/ | ✅ content-built | P-34, P-01 | 🟡 PENDING-PUBLISH — blocked on Needle project |
| T-EH-01 | AI Product Launch Readiness Checker | Medium | *(pending publish)* | templates/ai-product-launch-checklist/ | ✅ content-built | P-34, P-10 | 🟡 PENDING-PUBLISH |
| T-EH-02 | AI Template Marketplace Optimizer | Low | *(pending publish)* | templates/marketplace-optimizer/ | ✅ content-built | P-34 | 🟡 PENDING-PUBLISH |
| T-EH-03 | Monetization Diagnostic for AI Tools | Low | *(pending publish)* | templates/monetization-diagnostic/ | ✅ content-built | P-34 | 🟡 PENDING-PUBLISH |
| T-EH-04 | Solo AI Builder Sprint Planner | Low | *(pending publish)* | templates/sprint-planner/ | ✅ content-built | P-34, P-33 | 🟡 PENDING-PUBLISH |

---

## Publish Protocol — When Needle URL Is Received

For each template published, immediately:
```
1. Update Needle Link column with live URL
2. Update Build Status → live
3. Update COLLEEN Status → ✅ LIVE
4. Append to AUDIT_TRAIL.md:
   id: PUB-00N
   event_type: publish
   template_id: T-EH-0X
   needle_url: [url]
   date: [date]
5. Log in SWEEP_LOG.md
6. If T-EH-05: trigger LinkedIn launch post (docs/LAUNCH_POST_LINKEDIN.md)
```

---

## COLLEEN Audit Protocol

When a template goes live, log immediately:
```
template_id:
release_date:
needle_link: [full URL]
github_spec_path:
risk_tier:
policy_id:
colleen_flag: resolved
```
→ Append to [AUDIT_TRAIL.md](../governance/AUDIT_TRAIL.md) and update row above.
