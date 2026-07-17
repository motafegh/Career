# Session and Blocker Protocol

## 1. Session-start message

Ali starts every focused session with:

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

Do not ask “What should I do?” The controlling item is the first incomplete deliverable in `plans/CURRENT_WEEK.md`.

## 2. Required AI Session Order

The AI returns one order using this structure:

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
- after output, identify what it proves and does not prove;
- a time budget is a maximum, not a target to fill;
- when the deliverable finishes early, continue to the named next authorized deliverable;
- do not assign a full session to administrative work that should take minutes;
- do not repeat a demonstrated lab merely to consume scheduled time.

## 3. Session-end message

Ali closes every session with:

```text
SESSION END
Focused minutes:
Deliverables completed:
Evidence/commit:
Commands/tests and results:
What Ali can explain or modify:
Corrections received:
AI assistance used:
Unresolved blocker:
Exact next deliverable:
```

The AI judges:

- **Pass** — deliverable completed with sufficient evidence;
- **Partial** — continue the same deliverable;
- **Blocked** — invoke blocker protocol;
- **Invalid evidence** — rerun or repair;
- **Out of scope** — stop, revert, park, or discard;
- **Underloaded** — deliverable was materially smaller than planned; advance immediately and record for weekly calibration.

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
- why it blocks the current deliverable;
- required depth now;
- deferred depth;
- one verification task.

After verification, return immediately to the blocked deliverable.

A prerequisite gap does not authorize a general course or new roadmap.

## 6. Environment blocker protocol

If unresolved within one session:

1. preserve state and evidence;
2. state whether the environment is required for the current gate;
3. choose the smallest workaround when one exists;
4. defer only the environment-specific part when safe;
5. register an explicit follow-up gate;
6. continue another authorized deliverable when dependency order permits;
7. do not restart the project.

## 7. Planning-diversion protocol

When Ali starts broad planning outside a formal review point, the AI should respond:

```text
This decision is already controlled by the 90-day system. The current deliverable is: <deliverable>. The next action is: <action>.
```

A brief clarification is allowed only if the current files conflict, are materially underloaded, or lack a technically necessary decision.

## 8. New idea protocol

Record:

```text
Deferred idea:
Possible trigger:
```

Maximum discussion: five minutes.

No design, research, repository, task list, or implementation is created.

## 9. Underloading protocol

When Ali completes a planned item in materially less time than allocated:

1. verify that the item truly passed;
2. record actual time;
3. do not manufacture more documentation or repetition;
4. move to the next authorized deliverable;
5. record the estimate error at weekly closure;
6. compress similar future work during the next weekly activation.

Underloading is a plan defect to correct, not evidence that Ali should stop working.

## 10. Change-request protocol

A plan-change request must include:

```text
Affected gate:
Evidence:
Why current route is infeasible, underloaded, overloaded, or materially inferior:
Smallest proposed change:
Schedule consequence:
What remains fixed:
```

Without this evidence, reject the change and resume execution.

## 11. AI implementation boundary

AI may:

- teach;
- propose bounded structure;
- provide or edit supporting code;
- pair program;
- review;
- debug from evidence;
- generate tests and fixtures for review;
- help document completed behavior.

For learning-critical components, Ali must progressively:

- explain purpose and flow;
- predict behavior;
- direct or modify implementation;
- run tests;
- inspect failure;
- diagnose a changed case;
- state limitations.

AI-generated complexity alone never passes an ownership gate.