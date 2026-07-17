# Session and Blocker Protocol

## 1. Session-start message

The user starts every focused session with:

```text
START DAY <program day>
Date: YYYY-MM-DD
Mode: Green | Yellow | Red
Sleep/function: <public-safe summary>
Available focused minutes: <number>
Current weekly order: <order name>
Current state: <one sentence>
```

Do not ask “What should I do?” The controlling order is the first incomplete item in `plans/CURRENT_WEEK.md`.

## 2. Required AI Session Order

The AI returns one order using this structure:

```text
SESSION ORDER

Objective:
Why this is next:
Timebox:
Required prerequisite depth:
User-owned action:
AI assistance allowed:
Files/components allowed:

Steps:
1.
2.
3.

Expected evidence:
Stop line:
Pass condition:
If completed early:
```

Rules:

- one selected route;
- no unrelated alternatives;
- no future-phase expansion;
- no unexplained command dump;
- consequential commands are explained before execution;
- after output, identify what it proves and does not prove.

## 3. Session-end message

The user closes every session with:

```text
SESSION END
Focused minutes:
Completed behavior:
Evidence/commit:
Tests or observed output:
What I can explain:
Corrections received:
Unresolved blocker:
Exact next action:
```

The AI judges:

- **Pass** — order completed with sufficient evidence;
- **Partial** — continue the same order;
- **Blocked** — invoke blocker protocol;
- **Invalid evidence** — rerun or repair;
- **Out of scope** — stop, revert, park, or discard.

## 4. Technical blocker protocol

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

Spend up to 15 minutes inspecting evidence personally.

### Step 2 — Bound

Identify the likely affected layer:

- environment;
- network;
- process/service;
- file/permission;
- parser;
- validation;
- persistence;
- detection;
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
5. revise the hypothesis from output.

### Step 4 — Repair

Repair the smallest supported cause.

### Step 5 — Validate

Re-run:

- the failing case;
- a relevant success case;
- the nearest integration path.

Record what the repair proves and what remains unverified.

## 5. Missing prerequisite protocol

Initial repair cap: **90 focused minutes**.

The AI must state:

- exact missing concept;
- why it blocks the current order;
- required depth now;
- deferred depth;
- one verification task.

After verification, return immediately to the blocked order.

A prerequisite gap does not authorize a general course or new roadmap.

## 6. Environment blocker protocol

If unresolved within one session:

1. preserve state and evidence;
2. state whether the environment is required for the current gate;
3. choose the smallest workaround when one exists;
4. defer only the environment-specific part when safe;
5. register an explicit follow-up gate;
6. do not restart the project.

## 7. Planning-diversion protocol

When the user starts broad planning outside a formal review point, the AI should respond:

```text
This decision is already controlled by the 90-day system. The current order is: <order>. The next action is: <action>.
```

A brief clarification is allowed only if the current files conflict or lack a technically necessary decision.

## 8. New idea protocol

Record:

```text
Deferred idea:
Possible trigger:
```

Maximum discussion: five minutes.

No design, research, repository, task list, or implementation is created.

## 9. Change-request protocol

A plan-change request must include:

```text
Affected gate:
Evidence:
Why current route is infeasible or materially inferior:
Smallest proposed change:
Schedule consequence:
What remains fixed:
```

Without this evidence, reject the change and resume execution.

## 10. AI implementation boundary

AI may:

- teach;
- propose bounded structure;
- provide or edit supporting code;
- pair program;
- review;
- debug from evidence;
- generate tests and fixtures for review;
- help document completed behavior.

For learning-critical components, the user must progressively:

- explain purpose and flow;
- predict behavior;
- direct or modify implementation;
- run tests;
- inspect failure;
- diagnose a changed case;
- state limitations.

AI-generated complexity alone never passes an ownership gate.