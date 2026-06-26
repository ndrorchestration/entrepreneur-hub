# COLLEEN SWEEP CHECKLIST

**Framework:** DGAF v1.0  
**Cadence:** Weekly  
**Owner:** [your Monitor agent or you]  
**Schema ref:** T-EH-05 / SWEEP_LOG

---

## What a SWEEP Is

A SWEEP is a structured weekly audit. It catches problems that accumulate slowly — dead links, unresolved stubs, schema drift, missed phase gates, and CTA gaps. It is not optional. A system that skips SWEEPs is a system that's drifting.

**Time required:** 15 minutes if nothing is broken. Longer if you find issues (that's the point).

---

## Pre-SWEEP

- [ ] Record today's date as SWEEP date
- [ ] Note last SWEEP date — gap should be 5-9 days
- [ ] Open SWEEP_LOG and create a new entry stub

---

## Section 1: Link Integrity

- [ ] Every URL in your README resolves (no 404)
- [ ] Every URL in your template index resolves
- [ ] Every CTA link in published content resolves
- [ ] Payment/inquiry link resolves and accepts input

**Flag:** Any broken link → `🔴 BROKEN` status in SWEEP_LOG, fix within 24hr

---

## Section 2: Stub Resolution

- [ ] List all `(pending)` / `(stub)` / `(TODO)` entries across all docs
- [ ] For each stub: has it moved since last SWEEP?
- [ ] Any stub unchanged for 2+ SWEEPs → escalate to `🔴 UNRESOLVED`

**Flag:** Unchanged stub at 2 SWEEPs = governance violation, requires explicit decision: build it, kill it, or defer with date

---

## Section 3: Schema Compliance

- [ ] AUDIT_TRAIL entries follow current schema version
- [ ] No required fields are empty (`null` must be intentional, not forgotten)
- [ ] `funnel_source` field populated on all revenue events
- [ ] Agent role register has no empty rows

---

## Section 4: Phase Gate Verification

- [ ] Current phase is correctly marked in ROADMAP
- [ ] Phase gate conditions are met (not just marked done)
- [ ] No phase marked `✅` with unmet gate conditions

---

## Section 5: Revenue Signal Check

- [ ] Check traffic analytics — any new referral sources?
- [ ] Any new GitHub Issues / inquiry messages since last SWEEP?
- [ ] CTA is present and correct in all published templates
- [ ] Upsell link resolves to correct destination

**If traffic > 0 and revenue = $0 for 2+ SWEEPs:** This is a packaging/CTA gap, not a demand gap. Log it and act.

---

## Section 6: Agent Health

- [ ] Every active agent has an assigned role in the register
- [ ] No agent running outside its declared scope
- [ ] Monitor agent last ran within the expected cadence
- [ ] Any agent errors logged since last SWEEP?

---

## Post-SWEEP

- [ ] Log all findings in SWEEP_LOG with status (`✅ ok` / `🟡 WARN` / `🔴 UNRESOLVED`)
- [ ] Close SWEEP entry with: date, duration, finding count, action count
- [ ] Schedule next SWEEP (7 days from today)
- [ ] If GitHub Actions SWEEP reminder exists: close the issue

---

## SWEEP Log Entry Template

```markdown
### SWEEP-[NNN]: [YYYY-MM-DD]
**Type:** weekly-colleen  
**Duration:** [X min]  
**Status:** clean | issues-found | issues-found → remediated  

**Findings:**
| # | Section | Finding | Status | Action |
|---|---|---|---|---|
| 1 | [Section] | [What was found] | 🟡 WARN | [What was done] |

**Summary:** [X findings, Y remediated, Z deferred]
```
