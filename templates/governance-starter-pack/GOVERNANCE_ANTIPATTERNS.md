# GOVERNANCE ANTI-PATTERNS

**Framework:** DGAF v1.0  
**Template:** T-EH-05 Governance Starter Pack  
**Format:** Trigger → Mechanism → Mitigation (≥1 non-obvious per entry)

---

## Anti-Pattern 1: Phase Theater

**Definition:** Marking a phase as complete without verifying the gate conditions are actually met.

**Trigger:** The phase exists in a document. A checkbox is near it. Time pressure or optimism causes the checkbox to get checked. Downstream work proceeds on a false foundation.

**Mechanism:** Phase gates are only enforced if someone checks them against reality, not against the doc itself. A ROADMAP is not a verification system — it's a record. Without an external forcing function, the gate becomes a checkbox, not a gate.

**Non-obvious failure mode:** Phase theater compounds. Phase 1 "done" on a false Phase 0 means Phase 2 inherits two layers of unreality. By Phase 3, the ROADMAP and the actual system state are completely decoupled.

**Mitigation:**
- Gate conditions must be verifiable by a third party (agent or human) without reading your mental state
- Define gate conditions as observable artifacts, not feelings ("Needle project exists" not "Needle setup complete")
- COLLEEN SWEEP checks phase gate conditions against artifact state, not ROADMAP checkboxes

---

## Anti-Pattern 2: Orphaned Stubs

**Definition:** Scaffolded artifacts (files, sections, schema fields) that contain placeholder content and have no active path to completion.

**Trigger:** A folder or file is created to signal intent. The creator moves on. No deadline, no owner, no escalation path. The stub ages in place.

**Mechanism:** Stubs are invisible to most governance processes because they look like work-in-progress, not failures. They don't throw errors. They don't block deploys. They just quietly accumulate.

**Non-obvious failure mode:** Stubs become the ambient state of a system. New contributors (or agents) treat `(pending)` as a valid status and replicate the pattern. After 6 months, most of the system is stub.

**Mitigation:**
- Every stub must have a resolution date or explicit `deferred` status with a reason
- COLLEEN SWEEP flags stubs unchanged for 2+ cycles as `🔴 UNRESOLVED`
- Unresolved stubs at 3+ cycles trigger a forced decision: build, kill, or archive

---

## Anti-Pattern 3: SWEEP Decay

**Definition:** A governance audit cadence that is defined in documentation but has no external forcing function — so it silently stops running.

**Trigger:** Audit cadence is documented as "weekly." No calendar event, no automated issue, no external deadline. The first week it gets skipped, the next skip feels smaller. Within a month, the cadence is gone.

**Mechanism:** Human memory is not a reliable scheduler. Documentation that says "do this weekly" is not a schedule — it's a wish.

**Non-obvious failure mode:** The SWEEP log shows entries, but they're being written retroactively or skipped when problems are known (because a broken SWEEP is embarrassing to document). The log becomes theater too.

**Mitigation:**
- SWEEP cadence must have a mechanical trigger: GitHub Actions cron issue, calendar event, or external reminder
- The trigger creates a work item that must be closed — not just a notification that can be dismissed
- SWEEP log must include the triggering mechanism in each entry so retroactive writes are detectable

---

## Anti-Pattern 4: CTA-Less Distribution

**Definition:** High-traffic content with no clear conversion path to a paid tier or deeper engagement.

**Trigger:** Content is published to capture an audience. The content succeeds at this. Revenue doesn't follow. The creator concludes there's no demand.

**Mechanism:** Free content with no CTA trains the audience to expect free content. The conversion path must be explicit, frictionless, and present at the point of highest engagement (end of the template, not in a separate document).

**Non-obvious failure mode:** A CTA that exists but points to the wrong tier for the audience. Governance-interested readers hitting a "Product Launch Checklist" CTA will not convert — wrong offer, right audience. The CTA must match the audience's current state, not the creator's preferred product.

**Mitigation:**
- Every piece of free content ends with one CTA, matched to the audience's demonstrated interest
- CTA links are verified in every COLLEEN SWEEP
- Revenue = $0 after 2+ SWEEPs with traffic → mandatory investigation, not acceptance

---

## Anti-Pattern 5: Role Ambiguity

**Definition:** AI agents assigned tasks without a declared governance role — no clear ownership, no accountability chain, no scope boundary.

**Trigger:** A new agent or automated workflow is added quickly to solve an immediate problem. The role declaration step is skipped because it feels like overhead. The agent works fine — until it doesn't.

**Mechanism:** Without a role boundary, agents expand scope opportunistically. An agent tasked to "check links" starts modifying files. An agent tasked to "summarize" starts making decisions. Each expansion is individually reasonable; collectively they create a system where no one knows what anything is authorized to do.

**Non-obvious failure mode:** Role ambiguity creates liability gaps. When something goes wrong in an undeclared-role system, it's impossible to determine whether the failure was the agent acting outside scope, the orchestrator routing incorrectly, or the verifier not catching the output. Root cause analysis fails because the accountability structure never existed.

**Mitigation:**
- Every agent gets exactly one role from the taxonomy before it runs — no exceptions
- Hybrid roles require explicit declaration with a named mitigant
- Agent role register is a COLLEEN SWEEP artifact — empty rows = governance violation
