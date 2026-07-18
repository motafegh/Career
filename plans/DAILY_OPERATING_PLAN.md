# Exact Daily Operating Plan

## Current activation status

This file preserves general workload and session rules, but it does **not** authorize technical execution by itself.

- UpgradePilot is the formally selected primary flagship under [`../UpgradePilot.md`](../UpgradePilot.md).
- UpgradePilot implementation has not started.
- The existing AegisLab `CURRENT_WEEK.md` and daily route are deferred and non-controlling.
- No active UpgradePilot weekly or daily execution plan exists yet.
- Until the required UpgradePilot planning artifacts are approved, apply these rules only to the currently authorized planning artifact.
- The next authorized action is the **UpgradePilot capability and prerequisite specification**.

## 1. Production-day minimum

Monday through Saturday require **4 focused hours per day** in Green mode when the approved execution route is active. During an authorized preparation or planning hold, the controlling artifact may define a narrower workload.

Default structure after technical execution is activated:

| Time | Block | Duration | Purpose |
|---|---|---:|---|
| 13:45–14:00 | Open | 15 min | Read the first incomplete deliverable, inspect state, define expected proof |
| 14:00–16:00 | Block A | 120 min | Primary implementation, experiment, or bounded prerequisite repair |
| 18:00–20:30 | Dog walk/mobile window | not automatically counted | Required teach-back, evidence review, or one concrete blocker only |
| 20:30–22:30 | Block B | 120 min | Complete behavior, test, interpret, commit, and log |

The opening procedure is included in Block A. No planned project work begins after 22:45.

At least **3 hours per Green day** must normally involve direct laptop/terminal technical production after implementation is authorized. Mobile work can contribute at most 1 hour and only when the active approved UpgradePilot weekly plan names a concrete mobile-suitable deliverable.

## 2. Delivery-first rule

Each day has named outputs in the active approved UpgradePilot planning or weekly artifact. The deferred AegisLab `plans/CURRENT_WEEK.md` is not an active source of outputs.

Ali does not spend an assigned duration merely because it appears in the plan. When a task finishes:

1. run the required proof;
2. preserve the result;
3. continue to the next authorized item;
4. keep working until the daily quota is met or an explicit stop line is reached.

A 10-minute task receives approximately 10 minutes, not 45. A technically difficult task may consume the remaining block when evidence justifies it.

The managing agent must not use broad verbs such as “study,” “review,” or “understand” without naming the artifact, test, explanation, or modification that proves completion.

## 3. What counts as focused time

After technical execution is authorized, counts include:

- writing or modifying active code;
- running and interpreting experiments;
- writing or strengthening tests;
- debugging from evidence;
- SQL work tied to the active gate;
- focused prerequisite repair required by the current task;
- creating sanitized fixtures;
- creating required scenario truth/evidence artifacts;
- producing an explanation required by an ownership gate;
- technically necessary documentation derived from completed behavior.

During the current planning hold, only work required to create and validate the named authorized planning artifact counts. Implementation-like work does not become authorized merely because it produces an artifact.

Does not count by default:

- broad AI conversation;
- roadmap or career discussion outside the authorized artifact;
- browsing unrelated technologies;
- passive videos;
- rereading plans;
- formatting or polishing documentation;
- Sentinel inspection beyond the archive allowance;
- discussing future phases outside the authorized artifact;
- time when attention is substantially elsewhere;
- waiting for a command or tool without using the time on another authorized step.

Mobile work counts only when the current approved artifact permits it and the session produces a preserved explanation, evidence annotation, decision, or exact next action.

## 4. Capacity modes and exact quotas

### Green

- Daily minimum: **4 hours** after full execution activation, unless the current approved planning artifact defines a smaller preparation scope
- Structure: two 120-minute blocks during technical execution
- Work type: full active order
- Maximum planned load: 5 focused hours

### Yellow

- Daily minimum: **2.5 hours** after full execution activation
- Structure: one 90-minute and one 60-minute block, or one 150-minute block
- Missing 1.5 hours becomes weekly recovery work
- Work type: tests, fixtures, parser/validation, evidence review, small repair, derived documentation, bounded SQL after implementation is authorized
- No architecture changes or risky environment modifications

### Red

- Daily minimum: **0 hours**
- Required action: one brief public-safe state note
- No unsafe debt or compensatory overwork
- Resume the same next action later

## 5. Weekly hour enforcement

### Required total

After an UpgradePilot execution week is activated:

- Standard week: **24 focused hours**
- One Yellow day creates 1.5 recovery hours.
- Yellow recovery may be completed by adding up to 60 minutes to later Green days or through Saturday's remaining capacity.
- Red days reduce the adjusted weekly target by 4 hours each.
- No day exceeds 5 focused hours for recovery.

### Saturday

After weekly execution is activated, Saturday is a normal production day, not merely a buffer.

Saturday priorities:

1. finish the weekly Must Deliver package;
2. run the full weekly gate;
3. repair missing tests/evidence;
4. perform the authorized advancement item if the gate passed early;
5. close and commit the week.

Do not begin an unlisted future technology or feature.

### Sunday

After an UpgradePilot weekly plan exists, the mandatory 30-minute procedure is:

1. calculate focused hours;
2. mark weekly gate Pass, Partial, Blocked, or Failed;
3. link evidence;
4. complete the weekly ownership check;
5. identify the first next action;
6. activate the next approved UpgradePilot weekly version.

No implementation unless safety-critical cleanup remains.

## 6. Exact session start

Before focused work, record:

```text
START DAY <program day>
Date: YYYY-MM-DD
Mode: Green | Yellow | Red
Sleep/function: public-safe summary
Available focused minutes:
Current deliverable:
First expected artifact or proof:
```

Do not begin with “What should I do?” The first incomplete deliverable in the current approved artifact is controlling.

## 7. Exact session end

Record:

```text
SESSION END
Focused minutes:
Deliverables completed:
Evidence or commit:
Commands/tests and results:
What Ali can explain or modify:
AI assistance used:
Unresolved blocker:
Exact next deliverable:
```

Update the progress ledger only from this evidence.

## 8. Distraction protocol

When a new idea, project, course, tool, or architecture appears:

1. write one sentence under Deferred in the current approved artifact;
2. spend no more than five minutes on it;
3. return to the active deliverable;
4. do not ask another agent to expand the idea.

## 9. Difficulty protocol

### Confused

- Inspect evidence for 15 minutes.
- State expected behavior, actual behavior, decisive output, and one hypothesis.
- Request bounded AI help.

### Blocked

- Follow `operations/SESSION_PROTOCOL.md` after technical execution is authorized.
- Do not modify random layers.
- Do not redesign the project.

### Finished early

Use remaining focused time in this order:

1. run the named proof again from a clean or changed case;
2. complete the next Must Deliver item;
3. perform the required ownership modification or diagnosis;
4. complete the authorized advancement item;
5. clean and commit;
6. stop after the daily quota or explicit stop line.

During the current planning hold, replace technical proof steps with the review and consistency checks defined by the authorized planning artifact.

## 10. Documentation ceiling

Except during portfolio closure or an explicitly authorized planning artifact:

- documentation may consume at most **15% of focused weekly technical-execution time**;
- evidence, scenario contracts, truth records, and technically required interfaces are not counted as presentation documentation;
- existing plans are edited only when actual evidence or formal governance changed;
- polished prose cannot compensate for missing behavior or tests.