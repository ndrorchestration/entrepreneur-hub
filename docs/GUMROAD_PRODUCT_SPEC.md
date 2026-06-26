# Gumroad Product Spec — Enterprise Starter ($199)
<!-- COLLEEN: verify Gumroad URL is live before each SWEEP -->
<!-- Status: DRAFT — requires manual Gumroad page creation -->

## Product Details

| Field | Value |
|---|---|
| **Product name** | AI Governance Enterprise Starter |
| **Price** | $199 (one-time) |
| **Format** | Digital download + async consult |
| **Target buyer** | AI founders, CTOs, operators using AI tools in production |
| **Conversion source** | GitHub README -> "Enterprise Starter" CTA |

## Gumroad Page Copy

### Headline
`AI Governance Enterprise Starter — DGAF Framework`

### Subheadline
`Stop flying blind on AI decisions. Get a complete governance system + 1hr async consult.`

### What's Included
- **Governance Starter Pack** (T-EH-05) — full template bundle
  - Decision log schema (Markdown + JSON)
  - Agent role taxonomy (Orchestrator, Verifier, Executor, Monitor)
  - COLLEEN SWEEP checklist (weekly audit cadence)
  - AUDIT_TRAIL schema v1.1 with funnel tracking
  - Phase-gate model (Phase 0-5)
  - 5 governance anti-patterns + mitigations
- **1hr Async Consult** — you send a Loom or voice memo of your architecture/problem, I send back a structured written diagnosis with recommendations within 5 business days
- **DGAF Framework reference doc** — the full system behind 12 published Needle workflows

### Who This Is For
- You're building an AI product and have no governance layer
- You have governance docs but they're aspirational, not operational
- You want a senior AI architect's eyes on your system without a $5K engagement

### Guarantee
30-day refund if the consult doesn't surface at least one non-obvious architectural risk.

### CTA Button Text
`Get Enterprise Starter — $199`

### Tags
`AI governance, DGAF, entrepreneur, startup, AI architecture, audit`

---

## Gumroad Setup Checklist
- [ ] Create product at gumroad.com/products/new
- [ ] Upload T-EH-05 bundle as the digital download
- [ ] Set price to $199
- [ ] Enable "Pay what you want" minimum at $199
- [ ] Add consult delivery instructions to confirmation email
- [ ] Copy Gumroad product URL
- [ ] Update README.md Enterprise Starter CTA with Gumroad URL
- [ ] Update NEEDLE_TEMPLATE_INDEX with Gumroad URL
- [ ] Log in AUDIT_TRAIL.md as GOV-EH-003
- [ ] Run COLLEEN SWEEP after go-live

## Revenue Attribution
```json
{
  "product_id": "enterprise-starter-199",
  "price": 199,
  "funnel_sources": ["github-readme", "needle-template-cta", "linkedin-post"],
  "colleen_audit_field": "funnel_source",
  "schema_version": "1.1"
}
```
