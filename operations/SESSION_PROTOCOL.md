# Session and Blocker Protocol

## Current activation status

This protocol does not authorize UpgradePilot technical implementation by itself.

- [`../UpgradePilot.md`](../UpgradePilot.md) is the governing project charter.
- [`../strategy/UPGRADEPILOT_CAPABILITY_AND_PREREQUISITE_SPECIFICATION.md`](../strategy/UPGRADEPILOT_CAPABILITY_AND_PREREQUISITE_SPECIFICATION.md) is the approved capability-control artifact.
- [`../governance/UPGRADEPILOT_LEARNING_AND_EXECUTION_CONTRACT.md`](../governance/UPGRADEPILOT_LEARNING_AND_EXECUTION_CONTRACT.md) is the approved operating contract.
- [`../plans/UPGRADEPILOT_90_DAY_MASTER_ROADMAP.md`](../plans/UPGRADEPILOT_90_DAY_MASTER_ROADMAP.md) is the approved master route.
- UpgradePilot implementation has not started.
- The existing AegisLab current-week and daily routes are deferred and non-controlling.
- No technical Session Order, implementation command, architecture task, corpus acquisition, model experiment, cloud deployment, or advanced-systems package may begin until the staged milestone plan, evidence/progress tracker, and first-session plan authorize it.
- The next authorized action is the **UpgradePilot Staged Milestone Plan**.

During the remaining planning hold, use this protocol only when useful for a bounded planning deliverable; do not issue technical execution orders.

## 1. Session-start message

After an active UpgradePilot planning or execution artifact defines a focused session, Ali starts with:

```text
START DAY <program day>
Date: YYYY-MM-DD
Mode: Green | Yellow | Red
Sleep/function: <public-safe summary>
Available focused minutes: <number>
Current deliverable: <artifact/behavior name>
Current state: <one sentence>
First expected proof: <file/test/command/output>
```

Do not ask “What should I do?” The first incomplete deliverable in the current approved artifact is controlling. Deferred AegisLab files are never controlling.

## 2. Required AI Session Order

After technical execution is explicitly authorized, the AI returns one order:

```text
SESSION ORDER

Deliverable:
Exact output path or behavior:
Why it is next:
Maximum time budget:
Required prerequisite depth:
Ali-owned action:
AI assistance allowed:
Files/components allowed:

Execution sequence:
1.
2.
3.

Proof commands/tests:
Expected evidence:
Stop line:
Pass condition:
Next authorized deliverable if completed early:
```

Rules:

- one selected route;
- exact output before commands;
- no unrelated alternatives;
- no future-phase expansion;
- no unexplained command dump;
- consequential commands are explained before execution;
- Ali predicts representative behavior;
- actual output is interpreted before continuation;
- identify what evidence proves and does not prove;
- time budgets are maxima, not targets to fill;
- continue only to the named next authorized deliverable;
- do not assign full sessions to administrative work that should take minutes;
- do not repeat demonstrated work merely to consume scheduled time;
- do not issue implementation commands during the planning hold.

## 3. Session-end message

Ali closes every authorized focused session with:

```text
SESSION END
Focused minutes:
Deliverables completed:
Evidence/commit:
Commands/tests and results:
What Ali can explain or modify:
Corrections received:
AI assistance used:
Capability evidence:
Unresolved blocker:
Exact next deliverable:
```

The AI judges:

- **Pass** — deliverable completed with sufficient evidence;
- **Partial** — continue the same deliverable;
- **Blocked** — invoke the blocker protocol;
- **Invalid evidence** — rerun or repair;
- **Out of scope** — stop, revert, park, or discard;
- **Underloaded** — materially smaller than planned; advance and record for calibration.

## 4. Technical blocker protocol

This section applies only after technical execution is authorized.

### Step 1 — Observe

Before changing code or configuration, record:

```text
Expected:
Actual:
Error/symptom:
Last known working point:
Evidence inspected:
Strongest current hypothesis:
```

Spend up to 15 minutes inspecting evidence personally where safe and practical.

### Step 2 — Bound

Identify the likely affected layer:

- environment;
- network;
- process/service;
- file/permission;
- acquisition;
- parser;
- validation;
- persistence;
- analysis/recommendation;
- model/evaluation;
- test;
- packaging/CI.

Do not change multiple layers simultaneously.

### Step 3 — Guided diagnosis

AI help is initially capped at 45 minutes.

The AI should:

1. challenge the current hypothesis;
2. request only decisive evidence;
3. select the smallest safe diagnostic action;
4. explain expected output categories;
5. revise the hypothesis from actual output.

### Step 4 — Repair

Repair the smallest supported cause.

### Step 5 — Validate

Re-run:

- the failing case;
- a relevant success case;
- the nearest integration path.

Record what the repair proves and what remains unverified.

## 5. Missing prerequisite protocol

Initial repair cap after technical execution begins: **90 focused minutes**.

The AI must state:

- exact missing concept;
- why it blocks the current deliverable;
- required depth now;
- deferred depth;
- bounded teaching action;
- one verification task;
- exact return point.

After verification, return immediately to the blocked deliverable.

A prerequisite gap does not authorize a general course or new roadmap. A materially larger gap triggers formal sequence or scope review.

## 6. External evidence blocker

When public evidence is missing, inaccessible, stale, conflicting, invalid, or expired:

1. preserve the evidence state;
2. do not fabricate certainty;
3. try only lawful and proportionate alternatives;
4. narrow the claim, request a targeted check, defer, or abstain;
5. record the effect on the report or evaluation.

## 7. Environment blocker protocol

After implementation is authorized, when an environment blocker remains unresolved within one session:

1. preserve state and evidence;
2. state whether the environment is required for the current gate;
3. choose the smallest workaround when one exists;
4. defer only the environment-specific part when safe;
5. register an explicit follow-up gate;
6. continue another authorized deliverable when dependency order permits;
7. do not restart the project.

## 8. Planning-diversion protocol

When broad planning begins outside the authorized artifact, respond:

```text
This decision is already controlled by the 90-day system.
Current deliverable: <deliverable>
Next action: <action>
```

The current controlling deliverable is the **UpgradePilot Staged Milestone Plan**. Architecture design, first-session commands, implementation, and advanced-system execution are out of scope until their later authorization.

A brief clarification is allowed only when current files conflict, are materially underloaded, or lack a necessary decision.

## 9. New idea protocol

Record:

```text
Deferred idea:
Possible trigger:
```

Maximum discussion: five minutes.

No design, research, repository, task list, or implementation is created outside the authorized artifact.