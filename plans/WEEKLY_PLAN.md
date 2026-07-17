# Exact 13-Week Plan

Each week has one outcome and one gate. Daily details are activated in `CURRENT_WEEK.md`.

| Week | Dates | Exact outcome | Gate |
|---:|---|---|---|
| 1 | Jul 20–26 | Complete server-log lifecycle correlation | Client, logs, processes, sockets, and packets mapped; reduced-prompt explanation completed |
| 2 | Jul 27–Aug 2 | Close namespace SSH checkpoint | Bounded normal/failure cases, truth, markers, cleanup, fault diagnosis, reduced-guidance reconstruction |
| 3 | Aug 3–9 | Establish Python project foundation | Package, CLI skeleton, configuration, fixtures, event model, tests run |
| 4 | Aug 10–16 | Complete parsing and validation | Valid record parses; malformed record quarantines; changed-rule test passes |
| 5 | Aug 17–23 | Complete SQLite persistence | Schema, inserts, queries, run/source metadata, persistence tests pass |
| 6 | Aug 24–30 | Complete first vertical slice | Raw fixture to finding/report works through one command and integration test |
| 7 | Aug 31–Sep 6 | Build Docker scenario adapter | Controlled normal and failure cases produce preserved evidence and clean up |
| 8 | Sep 7–13 | Make runs repeatable and add CI | Multiple run IDs, changed parameters, replay, comparison, CI pass |
| 9 | Sep 14–20 | Close reliability gaps | Clean setup, malformed/missing/duplicate tests, processing/environment failure recovery |
| 10 | Sep 21–27 | Establish rule baseline and ML-ready data | Run-level dataset, leakage groups, explicit features, rule metrics, sufficiency decision |
| 11 | Sep 28–Oct 4 | Make honest ML decision | Simple reproducible model compared with rule; bounded conclusion recorded |
| 12 | Oct 5–11 | Close portfolio presentation | README, diagram, setup, demo, sample evidence, CI, limitations, AI disclosure |
| 13 | Oct 12–17 | Obtain external calibration | External review/setup attempt, 5–10 applications, role comparison, Day 90 evaluation |

## Week 1 — Server-log lifecycle correlation

### Monday

- Restore or inspect current namespace SSH runtime.
- Identify the exact successful connection to analyze.
- Preserve the complete foreground `sshd` log segment.
- Establish a timestamped event sequence.

### Tuesday

- Annotate server log lines.
- Map authentication stages and connection lifecycle.
- Identify what client output confirms or does not confirm.

### Wednesday

- Correlate log lines with process ancestry, socket endpoints, and namespace membership.
- Add packet evidence where timestamps permit.
- Record uncertainty rather than forcing false matches.

### Thursday

- Re-run one bounded connection when preserved evidence is insufficient.
- Predict expected log/process/socket/packet behavior first.
- Complete a reduced-prompt explanation.

### Friday

- Produce the concise cross-source evidence map in AegisLab.
- Run the Week 1 knowledge/evidence gate.
- Update AegisLab project and learning state only from demonstrated evidence.

### Saturday

Buffer only if the gate or 15-hour minimum is incomplete.

### Sunday

20-minute review and Week 2 activation.

## Week 2 — Namespace closure

- Monday: define exact normal-authentication contract and truth record.
- Tuesday: define fixed-count repeated unauthorized-key contract, bounds, and abort conditions.
- Wednesday: execute both cases and preserve comparable evidence.
- Thursday: introduce one bounded fault, diagnose from evidence, repair, and rerun.
- Friday: reconstruct and explain with materially reduced guidance; close or explicitly defer.

## Week 3 — Python foundation

- Monday: create package layout and test runner.
- Tuesday: define configuration and paths.
- Wednesday: preserve sanitized raw fixtures.
- Thursday: define typed normalized event model.
- Friday: implement CLI skeleton and first passing test.

## Week 4 — Parsing and validation

- Monday: implement minimum parser for one known record.
- Tuesday: support required successful-authentication fields.
- Wednesday: support required failed-authentication fields.
- Thursday: implement validation and quarantine.
- Friday: changed-input and malformed-input tests; user modifies one rule.

## Week 5 — SQLite

- Monday: learn and implement schema.
- Tuesday: insert validated events.
- Wednesday: add run/source/environment metadata.
- Thursday: implement required SELECT, WHERE, GROUP BY, ORDER BY queries.
- Friday: persistence and query tests; explain schema choices.

## Week 6 — Vertical slice

- Monday: implement time-window rule.
- Tuesday: define finding representation.
- Wednesday: generate concise report.
- Thursday: integrate CLI/replay path and failure handling.
- Friday: raw-to-report integration gate and deliberate broken input.

## Week 7 — Docker adapter

- Monday: define Docker adapter boundaries without changing scenario meaning.
- Tuesday: build controlled client and target.
- Wednesday: run normal authentication and preserve evidence.
- Thursday: run repeated failure and cleanup.
- Friday: feed evidence through the existing pipeline.

## Week 8 — Repeatability and CI

- Monday: add run identity and repeat command.
- Tuesday: vary failure count.
- Wednesday: vary timing and test rule behavior.
- Thursday: compare namespace and Docker evidence.
- Friday: configure CI and pass tests from clean checkout.

## Week 9 — Reliability

- Monday: clean-state setup test.
- Tuesday: malformed and missing evidence tests.
- Wednesday: duplicate and replay behavior.
- Thursday: processing failure and recovery.
- Friday: environment failure, limitations, and reliability gate.

## Week 10 — Rule baseline

- Monday: define experimental question and unit of analysis.
- Tuesday: create run-level feature table.
- Wednesday: define leakage groups and split.
- Thursday: measure rule baseline.
- Friday: analyze precision, recall, false positives, and data sufficiency.

## Week 11 — ML decision

- Monday: select the smallest justified model.
- Tuesday: implement reproducible training.
- Wednesday: evaluate on held-out run groups.
- Thursday: compare with rule and inspect errors.
- Friday: record bounded decision; stop ML work.

## Week 12 — Portfolio closure

- Monday: accurate README and project boundary.
- Tuesday: architecture/data-flow diagram.
- Wednesday: clean setup instructions and demonstration script.
- Thursday: sample evidence/report, limitations, AI disclosure.
- Friday: ownership review and final portfolio gate.

## Week 13 — External calibration

- Monday: request external repository review.
- Tuesday: run or request clean setup attempt.
- Wednesday: compare project against selected job descriptions.
- Thursday: submit calibration applications.
- Friday/Saturday: evaluate feedback and complete Day 90 review.

## Carry rule

When a week fails:

1. use Saturday buffer;
2. cut optional material;
3. carry only the blocking gate item;
4. preserve later deadlines where possible;
5. remove ML before allowing an incomplete core pipeline;
6. never create a replacement roadmap.