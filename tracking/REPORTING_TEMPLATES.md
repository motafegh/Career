# Reporting Templates

Use public-safe language. Do not record medication, medical details, finances, credentials, or private personal information.

## 1. Daily execution log

Create daily logs when useful at:

```text
tracking/daily/YYYY-MM-DD.md
```

Template:

```markdown
# Daily Execution — YYYY-MM-DD

- Program day:
- Week:
- Capacity mode: Green | Yellow | Red
- Required focused time: 3h | 2h | 0h
- Actual focused time:
- Active order:

## Intended evidence

-

## Work performed

-

## Evidence

- AegisLab commit/file/worklog:
- Commands/tests/queries:
- Observed output:

## Understanding and ownership

- What I can explain:
- What I modified or directed:
- Where AI assistance was required:
- What remains unverified:

## Blocker or correction

- Expected:
- Actual:
- Strongest supported cause:
- Next diagnostic action:

## Exact next action

-
```

A Red day may use only:

```markdown
# Daily Execution — YYYY-MM-DD

- Program day:
- Capacity mode: Red
- Technical work: paused
- State preserved at:
- Exact next action when resumed:
```

## 2. Weekly review

Create at:

```text
tracking/weekly/week-NN.md
```

Template:

```markdown
# Week NN Review

- Dates:
- Required hours:
- Actual hours:
- Green days:
- Yellow days:
- Red days:
- Gate: Pass | Partial | Blocked | Failed

## Evaluation judgment

One direct paragraph.

## Evidence

- Commits:
- Tests:
- Working behavior:
- Explanation/ownership evidence:

## What was achieved

-

## What remains weaker or incomplete

-

## Main cause

- Plan issue:
- Execution issue:
- Technical blocker:
- Capacity context:

## Scope and rule compliance

- New project started: Yes | No
- Sentinel time:
- Documentation percentage:
- Rabbit-hole event:
- Out-of-scope work:

## Carry decision

- Carry item:
- Optional scope removed:
- First next action:

## Ledger update

- Weekly row updated: Yes | No
- Capability evidence updated: Yes | No
- Blocker registered: Yes | No
```

## 3. Day 30 and Day 60 review

Create at:

```text
tracking/reviews/day-30.md
tracking/reviews/day-60.md
```

Template:

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
- Gates passed:
- Planning-only weeks:
- New projects:
- Sentinel boundary compliance:
- Main recurring blocker:

## Plan quality

- Unrealistic assumptions:
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

The review cannot replace the working identity or primary project unless evidence satisfies the execution contract's change criteria.

## 4. Day 90 final evaluation

Create at:

```text
tracking/reviews/day-90.md
```

Template:

```markdown
# Day 90 Final Evaluation

## Final judgment

-

## Completed system

-

## Evidence

- Runnable behavior:
- Tests and CI:
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
- Can transfer:

## Remaining AI dependence

-

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

## 5. Blocker report

Use only when the blocker survives ordinary diagnosis.

```markdown
# Blocker BR-XXX

- Date:
- Week/gate:
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
- Workaround/defer option:
```

## 6. Plan-change request

```markdown
# Change Request CR-XXX

- Date:
- Affected gate:
- Evidence of infeasibility or material inferiority:
- Smallest proposed change:
- Schedule consequence:
- Optional scope removed:
- What remains fixed:
- Decision: Approved | Rejected | More evidence required
```

## 7. Application calibration log

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