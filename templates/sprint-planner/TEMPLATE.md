# Solo AI Builder Sprint Planner

**DGAF Framework · T-EH-04 · v1.0.0**

> A 2-week sprint framework designed specifically for solo AI builders — accounting for the realities of building AI products alone: context switching, model reliability variability, and the temptation to keep architecting instead of shipping.

---

## Why Standard Agile Breaks for Solo AI Builders

Standard sprint frameworks assume a team. Solo AI building is a different constraint set:

- **You are the PM, engineer, and tester.** Context switching costs are 3-5x higher.
- **AI components are non-deterministic.** A task that took 2 hours last sprint may take 6 this sprint if the model behavior changed.
- **The architecture trap.** Solo builders with high technical depth default to architecture over shipping. Every sprint needs a forcing function to ship something.
- **No standup means no visibility.** You can drift for 3 days before noticing you're off-plan.

This framework addresses all four.

---

## The 2-Week Sprint Structure

### Sprint Planning (Day 1 — 60 min)

**Step 1: Set the sprint goal (10 min)**
One sentence. Ends with a user-observable outcome, not an engineering milestone.
- ❌ "Implement the COLLEEN monitoring agent"
- ✅ "COLLEEN runs a SWEEP and logs the results without manual intervention"

**Step 2: Identify the forcing function (5 min)**
What will you publish, ship, or show at the end of this sprint? If the answer is "nothing external," you're architecture sprinting. Name a specific artifact: a live template, a committed repo change, a published post.

**Step 3: Capacity audit (15 min)**
```
Available hours this sprint:          ___
Recurring obligations (subtract):    -___
AI/model reliability buffer (15%):   -___
Context-switching overhead (20%):    -___
Net available hours:                  ___
```

**Step 4: Task list (20 min)**
List every task for the sprint goal. Estimate each in hours. Verify total ≤ net available hours.

| Task | Hours | AI-dependent? | Owner |
|---|---|---|---|
| | | | |

**Rule:** If the task list exceeds net available hours, cut tasks — not hours. Overcommitment is a governance failure.

**Step 5: Define done (10 min)**
For each task, write one sentence defining what "done" looks like. Not "worked on" — done.

---

### Daily Check-in (Every Day — 10 min)

Three questions only:
1. What did I complete yesterday?
2. What am I doing today?
3. Is there a blocker I need to surface now (not later)?

Log answers in the sprint log. The act of writing forces visibility.

**Red flag:** If you skip the daily check-in for 2 consecutive days, you've lost visibility. Stop. Run an emergency mid-sprint review.

---

### Mid-Sprint Review (Day 7 — 30 min)

- [ ] Count completed tasks vs. planned tasks
- [ ] Identify any scope creep (tasks added after Day 1 planning)
- [ ] Re-verify sprint goal is still achievable
- [ ] If < 40% of tasks are complete: do a scope cut, not a heroics push
- [ ] Log mid-sprint status: on-track / at-risk / scope-cut-required

**The scope-cut rule:** Cutting scope is not failure. Shipping a smaller thing completely is better than shipping a larger thing partially. A half-built AI component is not a deliverable.

---

### Sprint Retrospective (Day 14 — 45 min)

**What shipped?**
- List every artifact published, committed, or delivered
- Mark each: ✅ complete / 🟡 partial / ❌ not done

**Estimation accuracy:**
```
Planned hours:     ___
Actual hours:      ___
Delta:             ___
Delta %:           ___%
```

**Velocity insight:** After 3 sprints, your average delta % is your personal velocity multiplier. Apply it to all future estimates.

**Three questions:**
1. What worked well that I should protect?
2. What slowed me down that I should eliminate?
3. What one change would make next sprint 20% better?

**Log entries for:**
- DECISION_LOG: any architectural decision made during the sprint
- AUDIT_TRAIL: any governance or publish events
- SWEEP_LOG: SWEEP if it was due this sprint

---

## Sprint Templates

### Sprint Goal Template
```
Sprint [N] — [Date Range]

Goal: [One sentence, user-observable outcome]
Forcing function: [Specific artifact to ship by Day 14]

Capacity:
  Available:           ___ hours
  Net (after buffers): ___ hours

Tasks:
  [Task 1] — ___ hours — done when: ___
  [Task 2] — ___ hours — done when: ___

Mid-sprint check scheduled: Day 7, [date]
Retro scheduled: Day 14, [date]
```

### Daily Log Template
```
[Date]
Completed: ___
Today: ___
Blocker: ___ (or: none)
```

---

## AI-Specific Sprint Rules

1. **Never assign AI-dependent tasks without a fallback.** If the model doesn't cooperate, what's the manual path?
2. **Lock model versions before a sprint starts.** A model update mid-sprint is an unplanned variable.
3. **AI evaluation is a task, not overhead.** If you're shipping an AI output, "evaluate output quality" is a named task with time allocated.
4. **Architecture discussions are capped at 20% of sprint time.** If you're spending more than that, you're in an architecture sprint. Name it explicitly or cut it.
5. **Ship something every sprint.** Even if it's documentation. The forcing function is non-negotiable.

---

## Enterprise Implementation

**Enterprise Starter — $199:** I'll review your last 2 sprints against this framework, identify your specific failure pattern (architecture trap / scope creep / estimation failure / visibility loss), and give you a sprint structure tuned to your actual working style.

**→ Inquire:** [github.com/ndrorchestration/entrepreneur-hub](https://github.com/ndrorchestration/entrepreneur-hub)

---

> *Built with DGAF Framework — full AI governance toolkit for builders → [github.com/ndrorchestration/entrepreneur-hub](https://github.com/ndrorchestration/entrepreneur-hub)*
