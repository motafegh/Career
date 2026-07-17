# Current Week — Preparation and Week 1

**Active dates:** 2026-07-18 to 2026-07-26  
**Execution week:** Week 1, 2026-07-20 to 2026-07-26  
**Weekly focused minimum:** 15 hours  
**Primary repository:** `motafegh/AegisLab`

## Controlling outcome

> Complete server-log lifecycle correlation for the current namespace SSH scenario and demonstrate a reduced-prompt cross-source explanation.

## Week 1 gate

The week passes only when all are true:

- one complete successful SSH connection lifecycle is identified in foreground `sshd` logs;
- important log lines are mapped to client output, process ancestry, sockets, namespace membership, and packet evidence where available;
- evidence-source limitations are explicit;
- uncertain timestamp or identity matches remain labeled uncertain;
- the learner explains the lifecycle with materially reduced prompting;
- AegisLab current state and learning state are updated only from demonstrated evidence.

## Explicitly out of scope

- Docker work;
- VM work;
- Python evidence pipeline implementation;
- deeper SSH cryptography;
- new AegisLab architecture or roadmap;
- new study-guide framework;
- Sentinel work;
- career planning discussion.

## Preparation — Saturday, 2026-07-18

**Maximum:** 2 focused hours

### Order P1 — Read the control system once — 30 minutes

Read:

1. Career `README.md`
2. `governance/EXECUTION_CONTRACT.md`
3. `strategy/STRATEGY_AND_SCOPE.md`
4. this file

Evidence:

- one short note stating the fixed identity, weekly minimum, primary project, and Week 1 outcome.

Stop line:

- do not edit the system unless a factual error prevents execution.

### Order P2 — Inspect and freeze current project positions — 45 minutes

- Confirm AegisLab `PROJECT_STATE.md` is current enough to resume.
- Confirm Sentinel is not open as an active workstream.
- Do not inspect Sentinel internals.

Evidence:

- current AegisLab commit or project-state reference;
- one sentence: “Sentinel is an autonomous research archive and is not active this week.”

### Order P3 — Prepare Week 1 workspace — 45 minutes

- Identify the current AegisLab branch/worktree.
- Confirm the latest relevant SSH worklog and reconstruction runbook.
- Identify where foreground `sshd` logs are expected to exist or how they will be regenerated.
- Record the exact first Monday command or inspection action.

Do not rebuild the lab today unless required only to verify the resume path.

## Preparation — Sunday, 2026-07-19

**Maximum:** 20 minutes

- Reopen this file.
- Confirm Monday's first action.
- Prepare the session-start message.
- No technical implementation.

---

## Monday, 2026-07-20 — Establish the evidence timeline

**Mode requirement:** Green 3h; Yellow 2h; Red 0h with state note

### Block A — 90 minutes

1. Inspect current WSL, namespaces, lab paths, and `sshd` state.
2. Rebuild only missing runtime layers using the existing runbook.
3. Start foreground lab `sshd` with preserved logging if needed.
4. Execute one bounded successful SSH connection.
5. Preserve client output and the complete matching server-log segment.

Expected evidence:

- runtime inspection;
- client endpoint and server endpoint;
- start/end timestamps;
- foreground server-log file or captured output;
- exact connection selected for Week 1 analysis.

### Block B — 90 minutes

1. Put the selected events into chronological order.
2. Mark connection establishment, host verification, authentication, session establishment, and disconnect where visible.
3. Separate observed facts from interpretations.
4. Commit or preserve sanitized evidence and a brief worklog update.

Stop line:

- do not begin broad correlation with packets/processes until the server-log timeline is complete.

Pass condition:

- one successful connection has a bounded, preserved, timestamped client/server-log timeline.

---

## Tuesday, 2026-07-21 — Interpret server logs

### Block A — 90 minutes

1. Read each important server-log line.
2. Identify emitting process/PID where available.
3. Explain practical meaning and lifecycle position.
4. Mark lines that do not prove the assumed interpretation.

### Block B — 90 minutes

1. Map server-log stages to client debug output.
2. Identify client-only, server-only, and shared claims.
3. Write a concise evidence table:

```text
claim | client evidence | server-log evidence | confidence | limitation
```

Pass condition:

- authentication and disconnect stages are mapped without treating either side as complete truth.

---

## Wednesday, 2026-07-22 — Correlate processes, sockets, and namespaces

### Block A — 90 minutes

1. Re-establish a bounded connection if live evidence is required.
2. capture listener, privileged child, authenticated child, and client process relationships;
3. capture both socket-table perspectives;
4. capture namespace PID membership.

### Block B — 90 minutes

1. Correlate PIDs, endpoints, and timestamps with Tuesday's log timeline.
2. State what process evidence proves.
3. State what socket evidence proves.
4. State what namespace membership proves.
5. Record unresolved ambiguity.

Pass condition:

- one cross-source process/socket/log map exists and endpoints/PIDs are not guessed.

---

## Thursday, 2026-07-23 — Add packet evidence and test understanding

### Block A — 90 minutes

1. Use preserved packet evidence if it matches the selected connection reliably.
2. Otherwise predict and capture one narrow new SSH connection.
3. Identify TCP establishment, SSH identification, encrypted traffic, and teardown.
4. Map only defensible packet events to the host/log timeline.

### Block B — 90 minutes

Complete a reduced-prompt explanation covering:

- client `ssh`;
- listener and per-connection `sshd` processes;
- client/server four-tuple;
- host key and client authentication key;
- `known_hosts` and `authorized_keys`;
- what client, log, process, socket, namespace, and packet evidence each prove;
- what remains invisible after encryption;
- what happens during teardown.

Pass condition:

- explanation is accurate at current depth and major corrections are recorded.

---

## Friday, 2026-07-24 — Close Week 1 gate

### Block A — 90 minutes

Produce one concise AegisLab cross-source evidence map for the selected connection.

Required structure:

1. scenario and endpoints;
2. chronological lifecycle;
3. evidence-source table;
4. decisive observations;
5. uncertainty and limitations;
6. current learner ownership level;
7. remaining work for the canonical normal/failure cases.

### Block B — 90 minutes

1. Run the final Week 1 evidence check.
2. Correct unsupported claims.
3. Update AegisLab `PROJECT_STATE.md` and current learning state only if evidence changed.
4. Commit the bounded Week 1 result.
5. Update Career `tracking/PROGRESS_LEDGER.md`.

Pass condition:

- every Week 1 gate item is satisfied.

---

## Saturday, 2026-07-25 — Buffer

Mandatory only when:

- focused hours are below the adjusted weekly requirement; or
- the Week 1 gate is incomplete.

Maximum: 3 focused hours.

Allowed:

- complete missing evidence;
- fix one factual mapping;
- finish reduced-prompt explanation;
- run the gate;
- update records.

Not allowed:

- begin Week 2 scenario design;
- polish beyond gate requirements.

## Sunday, 2026-07-26 — Weekly closure

**Time:** 20 minutes

1. Calculate focused time.
2. Mark Week 1 Pass, Partial, Blocked, or Failed.
3. Link AegisLab evidence/commit.
4. Record the single Week 2 entry action.
5. Replace this file with the activated Week 2 order only after closure.

## Deferred ideas

Record new ideas below as one sentence only. Do not develop them.

- None.

## Exact next action

Complete **Preparation Order P1**. If already completed, execute the first incomplete order in sequence.