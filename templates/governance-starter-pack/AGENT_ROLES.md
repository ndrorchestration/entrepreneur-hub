# AGENT ROLE TAXONOMY

**Framework:** DGAF v1.0  
**Template:** T-EH-05 Governance Starter Pack  
**Rule:** Every AI agent or automated workflow must be assigned exactly one role before it runs.

---

## The Four Roles

### Orchestrator
**Responsibility:** Coordinates agent calls, owns phase state, routes tasks to the right executor.  
**Authority:** Can invoke any other agent. Decides sequencing and retry logic.  
**Accountability:** If the wrong agent was called, the Orchestrator is responsible.  
**Anti-pattern:** Orchestrator that also executes — this collapses the oversight layer.

**Your Orchestrator:** [Name it. What does it do in your system?]

---

### Verifier
**Responsibility:** Audits outputs before they leave the system boundary. Checks for schema compliance, factual consistency, and governance violations.  
**Authority:** Can block any output. Veto is final.  
**Accountability:** If bad output ships, the Verifier failed.  
**Anti-pattern:** Verifier that self-approves (no independence from the Executor it's checking).

**Your Verifier:** [Name it. What does it check?]

---

### Executor
**Responsibility:** Performs bounded, well-defined tasks — file write, API call, content generation, data transform.  
**Authority:** Operates only within its designated scope. Cannot expand its own scope.  
**Accountability:** If the task was done wrong, the Executor is responsible. If the task was the wrong task, the Orchestrator is responsible.  
**Anti-pattern:** Executor with unbounded scope ("do whatever is needed").

**Your Executors:**  
1. [Executor name] — Scope: [what it does and doesn't do]  
2. [Executor name] — Scope: [what it does and doesn't do]  

---

### Monitor
**Responsibility:** Watches for drift, SLA violations, unresolved stubs, and SWEEP failures. The system's health signal.  
**Authority:** Can escalate to Orchestrator or flag for human review. Cannot modify outputs directly.  
**Accountability:** If a known issue goes undetected for >1 SWEEP cycle, the Monitor failed.  
**Anti-pattern:** Monitor that only logs without escalating (silent failure mode).

**Your Monitor:** [Name it. What does it watch? What triggers escalation?]

---

## Hybrid Role Declaration

If an agent legitimately serves two roles (e.g., a combined Orchestrator/Verifier for a small system), declare it explicitly:

```yaml
agent_id: [name]
roles: [orchestrator, verifier]
role_boundary: |
  Acts as Orchestrator for task routing.
  Acts as Verifier for output validation ONLY after task completion — 
  never verifies its own orchestration decisions.
risk_accepted: reduced_independence
mitigant: human_review_on_all_outputs
```

Hybrid roles require the `mitigant` field. If you can't name a mitigant, split the roles.

---

## Role Assignment Register

| Agent / Workflow | Role | Scope | Owner |
|---|---|---|---|
| [Name] | Orchestrator | [Scope] | [You] |
| [Name] | Verifier | [Scope] | [You] |
| [Name] | Executor | [Scope] | [You] |
| [Name] | Monitor | [Scope] | [You] |

*Add rows as you add agents. Every row must be filled completely before the agent is activated.*
