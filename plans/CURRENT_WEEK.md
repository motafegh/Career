# Deferred AegisLab Current-Week Plan — Historical Only

> [!CAUTION]
> **This file is deferred, superseded for active execution, and non-controlling. Do not execute any instruction, command, deliverable, gate, branch action, or next action below.**
>
> UpgradePilot is the formally selected primary 90-day flagship. [`../UpgradePilot.md`](../UpgradePilot.md) is the governing project charter. Broad project comparison is closed. UpgradePilot implementation has not started, and no replacement UpgradePilot weekly plan exists yet.
>
> The next authorized action is to create the **UpgradePilot capability and prerequisite specification**. The original AegisLab contents below are preserved unchanged as historical planning evidence.

---

# Current Week — Preparation + Week 1 Delivery Sprint

**Historical status:** Deferred by the formal UpgradePilot selection decision; not an active week.  
**Preparation:** 2026-07-18 to 2026-07-19  
**Execution week:** 2026-07-20 to 2026-07-26  
**Required production time:** 24 focused hours  
**Historical primary repository:** `motafegh/AegisLab`

## Weekly delivery package

> **Close the namespace SSH learning slice and deliver Python Intake v0: two sanitized SSH authentication fixtures, a typed normalized event, a parser for success/failure records, and a CLI that emits normalized JSON with passing tests.**

This week is intentionally demanding. Namespace-only work must not consume the whole week.

## Must Deliver

### A. Namespace Closure Pack

Create or update these AegisLab artifacts using equivalent existing locations only when the repository already has a stronger canonical path:

```text
docs/scenarios/ssh-auth-v0.md
docs/evidence/week-01/namespace-ssh-evidence-map.md
docs/evidence/week-01/fault-report.md
docs/evidence/week-01/ownership-check.md
docs/evidence/week-01/truth/normal.json
docs/evidence/week-01/truth/repeated-failure.json
tests/fixtures/sshd/success.log
tests/fixtures/sshd/unauthorized_key.log
```

Required scenario contract:

- **Normal case:** one successful public-key authentication by the authorized client identity.
- **Repeated-failure case:** exactly **5** authentication attempts using the valid but unauthorized client key, from the controlled client to the controlled target, within a **60-second** scenario window.
- Both cases require explicit start/end markers, actor, target, expected outcome, expected count, truth source, abort conditions, cleanup, and known limitations.
- Truth must be maintained separately from parser or detector output.

Required evidence map:

```text
claim
→ truth evidence
→ client evidence
→ server-log evidence
→ process evidence
→ socket evidence
→ packet evidence
→ confidence
→ limitation
```

Required bounded fault:

- the intended authorized client key is used;
- the lab `sshd` is deliberately pointed at an incorrect or unavailable authorization-file path;
- Ali predicts the layer and expected evidence before execution;
- the resulting failure is diagnosed from client/server/process/socket evidence;
- the configuration is repaired;
- the authorized success case is revalidated.

Do not change the ordinary host SSH service. Do not commit keys or secrets.

### B. Python Intake v0

Required project paths:

```text
pyproject.toml
src/aegislab/__init__.py
src/aegislab/event.py
src/aegislab/sshd_parser.py
src/aegislab/cli.py
tests/unit/test_event.py
tests/unit/test_sshd_parser.py
tests/integration/test_cli_parse.py
```

Equivalent paths are allowed only when AegisLab already has an accepted Python package structure. Do not create competing package layouts.

Required normalized event fields:

```text
schema_version
observed_at
environment
source
service
event_type
outcome
auth_method
principal
remote_address
remote_port
process_id
raw_record
parse_warnings
```

Week 1 permitted values:

- `service = "sshd"`
- `event_type = "authentication"`
- `outcome = "success" | "failure"`
- `auth_method`, `principal`, address, port, and PID may be optional only when the raw record genuinely lacks them; missing values must not be invented.
- `raw_record` preserves the sanitized original line.
- `parse_warnings` records nonfatal uncertainty.

Required CLI behavior:

```bash
python -m aegislab.cli parse tests/fixtures/sshd/success.log
python -m aegislab.cli parse tests/fixtures/sshd/unauthorized_key.log
```

Each command must emit normalized JSON Lines to standard output. Recognized authentication records must not be replaced by prose. Diagnostic text goes to standard error.

### C. Required test behavior

At minimum, tests must prove:

1. valid event construction;
2. invalid `outcome` is rejected;
3. success record maps timestamp, principal, authentication method, remote address, remote port, and PID where present;
4. unauthorized-key failure maps outcome, principal, remote address, remote port, and PID where present;
5. raw record is preserved;
6. missing optional data is not fabricated;
7. unrelated non-authentication log lines are not falsely normalized as authentication events;
8. success CLI command emits valid JSON;
9. failure CLI command emits valid JSON;
10. CLI output agrees with direct parser output.

The exact number of tests may exceed ten. Ten passing tests alone do not pass the gate unless the required behavior is covered.

## Week 1 hard gate

The week passes only when all are true:

- normal and five-attempt repeated-failure scenario contracts are versioned;
- truth records are independent from observed parser/detector output;
- one complete successful lifecycle and the bounded failure case are defensibly mapped across available evidence sources;
- the authorization-path fault is predicted, reproduced, diagnosed, repaired, and revalidated;
- namespace-only work is explicitly closed at the current depth;
- sanitized success and unauthorized-key fixtures are committed;
- the Python package imports cleanly;
- both CLI commands emit valid normalized JSON;
- all required tests pass;
- Ali explains each event field and parser flow with reduced prompting;
- Ali intentionally modifies one parser mapping or accepted record variant and adds/updates its test;
- no private key, credential, sensitive personal data, or unsafe host configuration enters the repository.

## Explicitly out of scope

- Docker and VM work;
- SQLite persistence;
- detector implementation;
- RAG, agents, Kafka, Kubernetes, cloud deployment, or web APIs;
- deeper SSH cryptography;
- broad AegisLab architecture changes;
- new teaching/governance frameworks;
- Sentinel work;
- career replanning.

---

# Preparation — Saturday, 2026-07-18

**Maximum:** 45 minutes total. Finish faster when possible.

## P1 — Control acknowledgment — maximum 10 minutes

Read only:

1. Career `README.md`
2. `governance/EXECUTION_CONTRACT.md`
3. this file

Record four lines in the daily log:

```text
Identity:
Weekly minimum:
Week 1 delivery package:
Sentinel status:
```

## P2 — Workspace confirmation — maximum 15 minutes

Record:

- current AegisLab branch;
- current commit SHA;
- current worktree path;
- current `PROJECT_STATE.md` path;
- current SSH reconstruction runbook path;
- current namespace SSH worklog path.

No technical execution.

## P3 — Monday entry point — maximum 15 minutes

Record:

- command used to inspect namespaces;
- command used to inspect the lab `sshd` process/listener;
- path or command for foreground server logs;
- exact command/runbook section used to rebuild missing temporary state;
- exact first Monday action.

## P4 — Commit preparation note — maximum 5 minutes

Commit only the public-safe preparation log if changed.

**Saturday stop line:** no namespace rebuild, no Python setup, no plan editing.

---

# Sunday, 2026-07-19

**Maximum:** 15 minutes.

- Confirm Monday's first action.
- Prepare the Session Start message.
- Confirm the two expected scenario case IDs.
- No technical implementation.

---

# Monday, 2026-07-20 — Execute and Define the Canonical Cases

**Required:** 4 focused hours  
**Daily deliverables:** scenario contract, two truth records, sanitized success/failure fixtures, initial evidence map

## Delivery order

1. **Inspect and restore only missing runtime state.** Maximum investigation budget: 20 minutes before invoking the blocker protocol.
2. Execute the normal case with explicit start/end timestamps and preserve:
   - client command/output;
   - foreground `sshd` log segment;
   - endpoints;
   - relevant process/socket state;
   - cleanup result.
3. Execute exactly five unauthorized-key attempts within the bounded window and preserve the corresponding evidence.
4. Sanitize and commit one representative success log fixture and one unauthorized-key failure fixture.
5. Write `ssh-auth-v0.md` with actors, target, identities, semantics, counts, timing, markers, truth source, abort conditions, cleanup, and limitations.
6. Write separate `normal.json` and `repeated-failure.json` truth records.
7. Start the cross-source evidence map with the decisive authentication and disconnect claims.
8. Run a secrets/private-key check on staged files before commit.

## Monday proof

- normal case has exactly one intended success;
- repeated-failure truth records exactly five intended unauthorized-key attempts;
- truth files do not copy conclusions from parser/detector output;
- fixtures contain no private keys or sensitive paths beyond safe lab context;
- scenario contract is sufficient to rerun both cases.

## Monday stop line

Do not begin Python code until the scenario contract, truth records, fixtures, and initial evidence map are committed.

---

# Tuesday, 2026-07-21 — Diagnose the Fault and Close Namespace Scope

**Required:** 4 focused hours  
**Daily deliverables:** completed evidence map, fault report, ownership check, namespace closure commit

## Delivery order

1. Complete the normal/failure evidence map across truth, client, server log, process, socket, and packet evidence.
2. Before changing configuration, write the fault prediction:
   - changed layer;
   - expected client symptom;
   - expected server-log evidence;
   - what TCP/socket evidence should still prove;
   - repair condition.
3. Point the lab server at an incorrect/unavailable authorization-file path using the lab-specific configuration only.
4. Validate configuration syntax where applicable, run the intended authorized-key attempt, and preserve evidence.
5. Diagnose the failure layer without changing unrelated network or identity state.
6. Repair the authorization path and revalidate a successful authorized login.
7. Write `fault-report.md` with prediction, evidence, rejected hypotheses, cause, repair, and validation.
8. Complete a reduced-prompt explanation covering:
   - actor/target and four-tuple;
   - host identity versus client authentication identity;
   - `known_hosts` versus `authorized_keys`;
   - listener and per-connection processes;
   - what client/log/process/socket/packet evidence proves;
   - encrypted visibility boundary;
   - fault-layer diagnosis.
9. Record corrections and assistance in `ownership-check.md`.
10. Update AegisLab project/learning state only from demonstrated evidence and declare namespace-only work closed.

## Tuesday proof

- fault reproduced with the intended authorized key;
- evidence shows why the problem was authorization configuration rather than DNS, routing, TCP reachability, or server identity;
- repaired case succeeds;
- Ali's explanation requires materially less step-by-step prompting than reconstruction work;
- remaining SSH depth is explicitly deferred.

## Tuesday stop line

After namespace closure is committed, no more namespace-only experimentation this week.

---

# Wednesday, 2026-07-22 — Build Python Package and Event Contract

**Required:** 4 focused hours  
**Daily deliverables:** importable package, project config, typed event model, parser/CLI skeleton, first tests

## Delivery order

1. Inspect the repository for an existing accepted Python package/test structure. Reuse it when present.
2. Create or update `pyproject.toml` with only dependencies/tools required now.
3. Create the importable `aegislab` package and test directories.
4. Implement the typed normalized authentication event with the exact Week 1 fields.
5. Add minimum construction/validation behavior for allowed outcome and service/event constants.
6. Create parser and CLI function boundaries without implementing unrelated formats.
7. Add tests for valid construction and invalid outcome.
8. Run package import and test commands from the repository root.
9. Write a brief field contract in code docstrings or an existing technical specification; do not create a large architecture document.

## Wednesday proof

```bash
python -c "import aegislab"
pytest -q
```

Both commands succeed from the declared development environment.

Ali must explain:

- why the model exists;
- difference between raw record and normalized fields;
- which fields are required versus optional;
- why absent data must not be invented.

## Wednesday stop line

Do not add database, detector, API, or generic framework abstractions.

---

# Thursday, 2026-07-23 — Implement SSH Authentication Parsing

**Required:** 4 focused hours  
**Daily deliverables:** working success/failure parser and required unit tests

## Delivery order

1. Inspect the exact sanitized fixture line formats.
2. Write expected normalized outputs before implementing parsing.
3. Implement parsing for the required accepted-public-key success format.
4. Implement parsing for the required unauthorized/public-key failure format present in the fixture.
5. Preserve timestamp, PID, user/principal, address, port, authentication method, and raw line where available.
6. Return no authentication event for unrelated lines; do not guess.
7. Add tests for all parser requirements listed above.
8. Run tests after each behavior family.
9. Deliberately alter one fixture value and confirm the output changes as predicted.
10. Commit only after direct parser tests pass.

## Thursday proof

- parser output matches prewritten expected events;
- no values are fabricated;
- unrelated lines do not become auth events;
- raw source is preserved;
- direct parser tests pass.

## Thursday stop line

Do not generalize into a full syslog framework or support every OpenSSH message.

---

# Friday, 2026-07-24 — Build CLI and Integration Path

**Required:** 4 focused hours  
**Daily deliverables:** working CLI for both fixtures, JSON output contract, integration tests

## Delivery order

1. Implement the exact `parse` CLI subcommand.
2. Read a supplied file line by line.
3. Emit one JSON object per recognized authentication event to standard output.
4. Send diagnostics to standard error.
5. Define deterministic serialization for timestamps, warnings, and optional fields.
6. Add success-fixture and failure-fixture integration tests.
7. Verify CLI output deserializes and equals direct parser output.
8. Run both required commands manually.
9. Run full Week 1 test suite.
10. Record exact commands and outputs in the worklog without copying unnecessary raw logs.

## Friday proof

```bash
python -m aegislab.cli parse tests/fixtures/sshd/success.log
python -m aegislab.cli parse tests/fixtures/sshd/unauthorized_key.log
pytest -q
```

- both CLI commands exit successfully;
- standard output contains valid JSON Lines;
- output fields match direct parser behavior;
- all required tests pass.

## Friday stop line

Do not add batch directories, SQLite, detector logic, or presentation polish.

---

# Saturday, 2026-07-25 — Ownership Modification and Full Gate

**Required:** 4 focused hours  
**Daily deliverables:** Ali-owned parser change, full gate report, clean commit

## Delivery order

1. Start from a clean checkout/worktree state and rerun the declared commands.
2. Ali selects one authorized ownership change:
   - add support for one second real success/failure line variant already present in preserved evidence; or
   - intentionally change one existing field mapping/normalization rule with a justified contract update.
3. Before implementation, Ali predicts affected outputs and tests.
4. Ali directs or performs the change and adds/updates tests.
5. Introduce one bounded parser defect or changed fixture and diagnose the failed test from evidence.
6. Repair and rerun the complete suite.
7. Complete the event-field/parser-flow explanation without reading generated prose.
8. Run a staged-file secret/sensitive-data inspection.
9. Produce a concise Week 1 gate report linking every Must Deliver artifact and proof.
10. Update Career daily/weekly evidence and commit.

## Authorized advancement after full gate passes early

Only when every Week 1 gate item passes:

- create Week 2 validation error categories;
- define the quarantine model skeleton;
- add no more than the first malformed-record test.

Do not begin SQLite or Docker.

## Saturday hard gate

Mark Week 1 **Pass** only when every item in the Week 1 hard gate is evidenced. Hours without artifacts do not pass. Early completion of a subtask does not end the production day.

---

# Sunday, 2026-07-26 — Closure and Week 2 Activation

**Required:** 30 minutes, not technical hours

1. Calculate actual focused time and capacity adjustments.
2. Mark every Must Deliver item Pass/Fail with a link.
3. Record test command and result.
4. Record Ali's ownership modification and diagnosis result.
5. Mark the week Pass, Partial, Blocked, or Failed.
6. Carry only the exact blocking item when necessary.
7. Activate Week 2.

## Deferred ideas

New ideas receive one sentence only.

- None.

## Exact next action

On Saturday, July 18, complete **P1–P4 in no more than 45 minutes total**. The first technical action remains Monday's runtime inspection and canonical case execution.