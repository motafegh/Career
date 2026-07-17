# Exact Daily Operating Plan

## 1. Production-day minimum

Monday through Friday require **3 focused hours per day** in Green mode.

Default structure:

| Time | Block | Duration | Purpose |
|---|---|---:|---|
| 13:45–14:00 | Open | 15 min | Read current order, inspect state, define expected evidence |
| 14:00–15:30 | Block A | 90 min | Primary implementation, experiment, or prerequisite repair |
| 18:00–20:30 | Dog walk/mobile window | not automatically counted | Review, teach-back, evidence reading, or one concrete blocker only |
| 20:45–22:15 | Block B | 90 min | Complete work, test, interpret, commit, and log |

The 15-minute opening is included within Block A preparation and does not add to the 3-hour quota.

No planned project work begins after 22:30. Preserve sleep and continuity rather than extending a weak session indefinitely.

## 2. What counts as focused time

Counts:

- writing or modifying active code;
- running and interpreting experiments;
- writing tests;
- debugging from evidence;
- SQL work tied to the active gate;
- focused prerequisite repair required by the current task;
- creating sanitized fixtures;
- producing an explanation required by the gate;
- technically necessary documentation derived from completed behavior.

Does not count by default:

- broad AI conversation;
- roadmap or career discussion;
- browsing unrelated technologies;
- passive videos;
- rereading plans;
- formatting documentation;
- Sentinel inspection beyond the archive allowance;
- discussing future phases;
- time when attention is substantially elsewhere.

Mobile work counts only when the current weekly plan permits it and the session produces a preserved note, explanation, decision, or next technical action.

## 3. Capacity modes and exact quotas

### Green

- Daily minimum: **3 hours**
- Structure: two 90-minute blocks
- Work type: full active order

### Yellow

- Daily minimum: **2 hours**
- Structure: two 60-minute blocks or one 120-minute block
- Missing 1 hour is assigned to Saturday
- Work type: tests, fixtures, review, small repair, derived documentation, bounded SQL
- No architecture changes or risky environment modifications

### Red

- Daily minimum: **0 hours**
- Required action: one brief public-safe state note
- No debt and no compensatory overwork
- Resume the same next action later

## 4. Weekly hour enforcement

### Required total

- Standard week: **15 focused hours**
- A single Yellow day changes weekday completion to 14 hours and creates 1 mandatory Saturday hour.
- Multiple Yellow days create matching Saturday debt up to the 3-hour Saturday cap.
- Red days reduce the expected total by 3 hours each and require evaluator review when repeated.

### Saturday

Saturday is mandatory when:

- hours are below the adjusted weekly requirement; or
- the weekly evidence gate is incomplete.

Maximum: **3 focused hours**.

Saturday priority:

1. gate blocker;
2. missing test/evidence;
3. hour debt;
4. weekly closure.

Do not start next week's work on Saturday.

### Sunday

Mandatory 20-minute procedure:

1. calculate focused hours;
2. mark weekly gate Pass, Partial, Blocked, or Failed;
3. link evidence;
4. identify the first next action;
5. activate the next `CURRENT_WEEK.md` version.

No implementation unless a safety-critical cleanup remains.

## 5. Exact session start

Before focused work, record:

```text
START DAY <program day>
Date: YYYY-MM-DD
Mode: Green | Yellow | Red
Sleep/function: public-safe summary
Available focused minutes:
Current weekly order:
First expected evidence:
```

Do not begin with a broad question such as “What should I do?” The first incomplete order is already controlling.

## 6. Exact session end

Record:

```text
SESSION END
Focused minutes:
Completed behavior:
Evidence or commit:
Tests/output:
What I can explain:
Unresolved blocker:
Exact next action:
```

Update the progress ledger only from this evidence.

## 7. Distraction protocol

When a new idea, project, course, tool, or architecture appears:

1. write one sentence under Deferred in the current weekly file;
2. spend no more than five minutes on it;
3. return to the active command;
4. do not ask another agent to expand the idea.

## 8. Difficulty protocol

### Confused

- Inspect evidence for 15 minutes.
- State symptom, expected behavior, actual behavior, and one hypothesis.
- Request bounded AI help.

### Blocked

- Follow `operations/SESSION_PROTOCOL.md`.
- Do not modify random layers.
- Do not redesign the project.

### Finished early

Use remaining focused time in this order:

1. run or strengthen required tests;
2. perform the required teach-back;
3. clean and commit the active work;
4. prepare the next listed action;
5. stop.

Do not pull work from a later week unless the current gate has passed and the weekly file explicitly authorizes it.

## 9. Documentation ceiling

Except during Week 12:

- documentation may consume at most **20% of focused weekly time**;
- existing plans are edited only when actual evidence changed;
- polished prose cannot compensate for missing behavior or tests.