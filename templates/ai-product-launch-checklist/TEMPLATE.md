# AI Product Launch Readiness Checker

**DGAF Framework · T-EH-01 · v1.0.0**

> A structured pre-launch audit for AI-powered products. 47 checkpoints across 6 domains. Built on the DGAF Framework.

---

## What This Is

Most AI product launches fail silently — the product ships, gets some traffic, and converts nothing. The failure isn't the product. It's that the launch had no structured readiness check. This template gives you one.

**Who this is for:** Founders, solo builders, and small teams shipping AI-powered products who want a repeatable launch protocol — not a generic checklist, but one built for the specific failure modes of AI products.

---

## The 6 Launch Domains

| Domain | Checkpoints | Most Common Failure |
|---|---|---|
| Product Readiness | 8 | Shipping before the core loop works |
| Governance & Safety | 7 | No human-in-the-loop for edge cases |
| Distribution Readiness | 8 | Launch to an audience you don't have yet |
| Conversion Infrastructure | 6 | Traffic arrives but no clear next step |
| Metrics & Instrumentation | 9 | Can't tell if the launch worked |
| Recovery Posture | 9 | No rollback plan for the first 48 hours |

---

## Domain 1: Product Readiness

- [ ] Core user loop executes end-to-end without manual intervention
- [ ] AI outputs are validated before reaching the user (not raw model output)
- [ ] Edge case handling is defined — what happens when the AI fails or hallucinates
- [ ] Latency is acceptable for the primary use case (defined: ___ms target)
- [ ] Rate limits and API costs are modeled at 10x, 100x, 1000x expected volume
- [ ] Data privacy posture is documented — what user data touches the model, where it goes
- [ ] The product does one thing well — scope is bounded, not a feature dump
- [ ] You have used it yourself for 7+ days before launch

**Gate:** All 8 checked before proceeding. If any are unchecked, that's your launch blocker — not marketing.

---

## Domain 2: Governance & Safety

- [ ] Every AI agent or workflow has a declared role (Orchestrator / Verifier / Executor / Monitor)
- [ ] Outputs are auditable — you can trace any output back to its inputs and model version
- [ ] Human review path exists for flagged or high-stakes outputs
- [ ] Model versioning is locked — you know exactly which model version shipped
- [ ] Prompt injection surface is assessed and documented
- [ ] Failure modes are documented with mitigations (not just "it's a beta")
- [ ] You can kill or roll back the AI component in under 10 minutes

**See also:** [Entrepreneur's AI Governance Starter Pack](https://github.com/ndrorchestration/entrepreneur-hub) — full governance kit for AI founders.

---

## Domain 3: Distribution Readiness

- [ ] You have an existing audience that matches your product's target user — or a specific plan to reach one
- [ ] Launch platform is chosen based on where your audience already is, not where you want them to be
- [ ] Your first 100 users are identified by name or channel — not "post on social and see"
- [ ] The product's CTA matches the audience's current state (not your ideal state)
- [ ] You have a content asset live before launch day that the target audience has already engaged with
- [ ] Launch timing avoids major competing events in your niche
- [ ] You have a second-day plan — what happens if day 1 is silent
- [ ] Referral or sharing mechanism is built in, not bolted on post-launch

**Non-obvious checkpoint:** Audience mismatch is the #1 distribution failure. If your existing audience is governance-curious and you're launching a product launch tool, you're pitching to the wrong room. Match product to audience, not audience to product.

---

## Domain 4: Conversion Infrastructure

- [ ] Every landing page has exactly one primary CTA
- [ ] The CTA is visible without scrolling on mobile
- [ ] The free tier clearly implies the paid tier exists (not hidden)
- [ ] Payment path is tested end-to-end before launch (not assumed to work)
- [ ] Inquiry path is tested — someone responding to your CTA gets a human reply within 24hr
- [ ] You know your conversion target: what does success look like in the first 7 days?

---

## Domain 5: Metrics & Instrumentation

- [ ] Traffic source tracking is live before launch (UTM or platform-native)
- [ ] Conversion event is defined and instrumented (not inferred from revenue)
- [ ] Funnel drop-off is measurable at each stage
- [ ] Baseline metrics are recorded pre-launch (traffic, conversion, revenue = $0 is a valid baseline)
- [ ] You have a "launch failed" definition — at what point do you pivot vs. persist?
- [ ] Week-1 review is scheduled before launch day
- [ ] Key metric is ONE number — not a dashboard of 12
- [ ] Referral source tracking connects distribution platform to conversion platform
- [ ] AI-specific metrics: model latency p50/p95, error rate, fallback activation rate

---

## Domain 6: Recovery Posture

- [ ] Rollback plan is documented and tested
- [ ] Communication template for outage/failure is drafted before it's needed
- [ ] Rate limiting is in place to prevent cost explosion from unexpected traffic
- [ ] Worst-case cost scenario is modeled (API costs at 10x traffic spike)
- [ ] Support path exists — user has a way to reach you if something breaks
- [ ] Known limitations are disclosed, not buried
- [ ] You have a 48-hour post-launch review scheduled
- [ ] Data loss scenario is assessed — what happens if your datastore fails on day 1?
- [ ] You can operate in degraded mode if the AI component fails entirely

---

## Launch Readiness Score

Count your checked items: ___/47

| Score | Status | Recommendation |
|---|---|---|
| 47/47 | Launch-ready | Ship |
| 40-46 | Nearly ready | Fix the gaps, then ship |
| 30-39 | Not ready | The unchecked items are your launch blockers |
| < 30 | Pre-launch | You're building, not launching — that's fine, keep building |

**The hard rule:** A score below 40 means the unchecked items will surface as problems in your first 48 hours. You can launch anyway — but you'll spend your launch energy fighting fires instead of reading signals.

---

## Enterprise Implementation

Need a second set of eyes on your specific launch readiness?

**Enterprise Starter — $199:** I review your repo/product setup, score you against all 47 checkpoints, and give you a specific remediation plan. Async, 24-48hr turnaround.

**→ Inquire:** [github.com/ndrorchestration/entrepreneur-hub](https://github.com/ndrorchestration/entrepreneur-hub)

---

> *Built with DGAF Framework — full AI governance toolkit for builders → [github.com/ndrorchestration/entrepreneur-hub](https://github.com/ndrorchestration/entrepreneur-hub)*
