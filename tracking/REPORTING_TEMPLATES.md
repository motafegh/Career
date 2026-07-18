# Deferred AegisLab Reporting Templates — Historical Only

> [!CAUTION]
> **These templates were written for the deferred AegisLab route and are non-controlling. Do not create current logs, reviews, application records, or evidence claims from the AegisLab-specific fields below.**
>
> UpgradePilot is the selected primary flagship under [`../UpgradePilot.md`](../UpgradePilot.md). UpgradePilot implementation has not started. The replacement evidence and progress tracker—and any UpgradePilot-specific reporting templates—have not yet been created.
>
> The next authorized action is to create the **UpgradePilot Learning and Execution Contract**. The original templates below are preserved unchanged as historical planning material.

---

# Reporting Templates

**Historical status:** Deferred by the formal UpgradePilot selection decision; not active reporting instructions.

Use public-safe language. Do not record medication, medical details, finances, credentials, or private personal information.

## 1. Daily execution log

Create at:

```text
tracking/daily/YYYY-MM-DD.md
```

```markdown
# Daily Execution — YYYY-MM-DD

- Program day:
- Week:
- Capacity mode: Green | Yellow | Red
- Required focused time: 4h | 2.5h | 0h
- Actual focused time:
- Current deliverable:

## Required outputs for today

- [ ]

## Work performed

-

## Evidence

- AegisLab commit/file/worklog:
- Commands/tests/queries:
- Observed output:
- Artifact paths:

## Understanding and ownership

- What Ali can explain:
- What Ali modified or directed:
- Prediction made before change:
- Where AI assistance was required:
- What remains unverified:

## Estimate quality

- Planned item materially underloaded: Yes | No
- Trivial work padded: Yes | No
- If completed early, next authorized deliverable entered: Yes | No | Not applicable

## Blocker or correction

- Expected:
- Actual:
- Strongest supported cause:
- Next diagnostic action:

## Exact next deliverable

-
```

A Red day may use only:

```markdown
# Daily Execution — YYYY-MM-DD

- Program day:
- Capacity mode: Red
- Technical work: paused
- State preserved at:
- Exact next deliverable when resumed:
```

## 2. Weekly review

Create at:

```text
tracking/weekly/week-NN.md
```

```markdown
# Week NN Review

- Dates:
- Standard required hours: 24
- Adjusted required hours:
- Actual hours:
- Green days:
- Yellow days:
- Red days:
- Gate: Pass | Partial | Blocked | Failed

## Evaluation judgment

One direct paragraph.

## Must Deliver status

| Deliverable | Status | Evidence | Limitation |
|---|---|---|---|

## Proof commands and results

-

## Ownership evidence

- Ali can explain:
- Ali intentionally modified:
- Ali tested:
- Ali diagnosed:
- AI assistance level:

## What was achieved

-

## What remains weaker or incomplete

-

## Main cause

- Plan issue:
- Execution issue:
- Technical blocker:
- Capacity context:

## Workload calibration

- Tasks materially underloaded:
- Tasks materially overloaded:
- Trivial tasks padded:
- Early completion advanced correctly:
- Delivery density judgment: Too low | Appropriate | Too high

## Scope and rule compliance

- New project started: Yes | No
- Sentinel time:
- Documentation percentage:
- Rabbit-hole event:
- Out-of-scope work:

## Carry decision

- Carry item:
- Optional scope removed:
- First next deliverable:

## Ledger update

- Weekly row updated: Yes | No
- Capability evidence updated: Yes | No
- Blocker registered: Yes | No
- Estimate defects registered: Yes | No
```

## 3. Day 14 workload review

Create at:

```text
tracking/reviews/day-14-workload.md
```

```markdown
# Day 14 Workload Review

## Delivery judgment

-

## Time evidence

- Standard hours:
- Adjusted hours:
- Actual hours:
- Production days completed:

## Delivery density

- Week 1 outputs:
- Week 2 outputs:
- Underloaded assignments:
- Overloaded assignments:
- Padded work detected:
- Idle time after early completion:

## Difficulty calibration

- Technically challenging enough:
- Too easy:
- Too difficult:
- Missing prerequisites:

## Decision

- Continue unchanged | compress further | rebalance | reduce unsafe load

## Bounded correction

- Evidence:
- Change:
- What remains fixed:
```

This review cannot change identity or primary project.

## 4. Day 30 and Day 60 review

Create at:

```text
tracking/reviews/day-30.md
tracking/reviews/day-60.md
```

```markdown
# Day XX Review

## Judgment

-

## Planned position

-

## Actual position

-

## Evidence and confidence

-

## Capability changes

| Capability | Previous evidence | Current evidence | Assistance | Limitation |
|---|---|---|---|---|

## Execution-system performance

- Focused hours achieved:
- Delivery gates passed:
- Planning-only weeks:
- New projects:
- Sentinel boundary compliance:
- Main recurring blocker:
- Delivery density:

## Plan quality

- Underloaded assumptions:
- Overloaded assumptions:
- Missing prerequisites:
- Scope problems:
- Sequence problems:

## Decision

- Continue unchanged | bounded correction required

## Approved bounded correction

- Evidence:
- Change:
- Schedule effect:
- What remains fixed:
```

## 5. Day 90 final evaluation

Create at:

```text
tracking/reviews/day-90.md
```

```markdown
# Day 90 Final Evaluation

## Final judgment

-

## Completed system

-

## Evidence

- Runnable behavior:
- Tests and CI:
- Parsing/validation/quarantine:
- Data and SQL:
- Docker:
- Rule baseline:
- ML decision:
- Portfolio:
- External feedback:
- Applications:

## Demonstrated ownership

- Can explain:
- Can modify:
- Can test:
- Can query:
- Can diagnose:
- Can reconstruct:
- Can transfer:

## Remaining AI dependence

-

## Execution-system evidence

- Total focused hours:
- Gates passed:
- Underloaded plan events:
- Overloaded plan events:
- Scope breaches:
- New projects:

## Strongest capability changes

-

## Unresolved weaknesses

-

## Market calibration findings

-

## Decision for next period

-

## Evidence-based next identity

-
```

## 6. Blocker report

Use only when the blocker survives ordinary diagnosis.

```markdown
# Blocker BR-XXX

- Date:
- Week/gate:
- Deliverable:
- Expected:
- Actual:
- Error/symptom:
- Last known working point:
- Evidence inspected:
- Affected layer:
- Hypotheses rejected:
- Strongest current hypothesis:
- Smallest next diagnostic action:
- Time already spent:
- Is the blocker gate-critical? Yes | No
- Parallel authorized deliverable available:
- Workaround/defer option:
```

## 7. Plan-change request

```markdown
# Change Request CR-XXX

- Date:
- Affected gate:
- Evidence of infeasibility, underloading, overloading, or material inferiority:
- Smallest proposed change:
- Schedule consequence:
- Optional scope removed:
- What remains fixed:
- Decision: Approved | Rejected | More evidence required
```

## 8. Application calibration log

Use during Week 13:

```markdown
# Application Calibration — <role/company>

- Role title:
- Location/work mode:
- Required core skills:
- Skills demonstrated by AegisLab:
- Skills partially demonstrated:
- Missing requirements:
- Application result/feedback:
- Evidence-based portfolio correction:
```

Do not turn application feedback into a new roadmap before the Day 90 review.