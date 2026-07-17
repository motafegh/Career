# Exact 13-Week Delivery Plan

Each week contains six 4-hour production days, one delivery package, exact Must Deliver outputs, and one hard gate. Daily execution detail for the active week is expanded in `CURRENT_WEEK.md`.

## Summary

| Week | Dates | Required hours | Delivery package | Hard gate |
|---:|---|---:|---|---|
| 1 | Jul 20–26 | 24 | Namespace closure + Python intake v0 | Bounded SSH cases and evidence close; parser/CLI normalizes success and failure fixtures |
| 2 | Jul 27–Aug 2 | 24 | Robust parser, validation, quarantine | Valid/invalid/unknown records behave deterministically; ownership change passes |
| 3 | Aug 3–9 | 24 | SQLite persistence and SQL | CLI persists runs/events/quarantine; required queries and duplicate rules pass |
| 4 | Aug 10–16 | 24 | Raw-to-report vertical slice | One command parses, validates, persists, detects, and reports with integration tests |
| 5 | Aug 17–23 | 24 | Docker SSH adapter | Controlled normal/failure Docker cases feed existing pipeline and match truth |
| 6 | Aug 24–30 | 24 | Scenario matrix, replay, CI | Multiple runs/parameters reproduce; CI passes from clean checkout |
| 7 | Aug 31–Sep 6 | 24 | Reliability closure | Failure matrix is tested; two reduced-prompt diagnoses pass |
| 8 | Sep 7–13 | 24 | Run-level experimental dataset | Reproducible runs map to truth, features, provenance, and leakage groups |
| 9 | Sep 14–20 | 24 | Rule baseline and error analysis | Metrics, sensitivity, errors, and data sufficiency are defensible |
| 10 | Sep 21–27 | 24 | Honest simple-ML decision | Group-safe simple model compared with rule; bounded conclusion recorded |
| 11 | Sep 28–Oct 4 | 24 | Engineering hardening | Clean setup, type/lint/test checks, security boundaries, and reconstruction pass |
| 12 | Oct 5–11 | 24 | Portfolio and interview package | README, diagram, demo, evidence, limitations, disclosure, and ownership defense pass |
| 13 | Oct 12–17 | 24 | External and market calibration | Review/setup feedback, 5–10 applications, corrections, and Day 90 evaluation complete |

---

## Week 1 — Namespace Closure + Python Intake v0

### Must Deliver

- canonical normal-authentication contract;
- fixed-count unauthorized-key failure contract;
- truth record, timestamps, markers, abort conditions, cleanup;
- sanitized success and failure log fixtures;
- cross-source evidence map;
- one bounded fault report;
- importable Python package;
- typed authentication-event model;
- success/failure parser;
- JSON-emitting CLI;
- required tests.

### Daily assignments

- **Monday:** execute and preserve normal/failure cases; write truth/scenario contracts; complete server-log evidence map.
- **Tuesday:** run fault prediction/diagnosis/repair; complete reduced-prompt namespace ownership check; close namespace scope.
- **Wednesday:** create Python project/package/test structure; commit fixtures; define typed event model and field contract.
- **Thursday:** implement success and failure parsing plus unit tests.
- **Friday:** implement CLI and fixture-to-JSON integration tests; perform one parser-field modification.
- **Saturday:** run full Week 1 gate; repair failures; if passed early, begin Week 2 validation categories and quarantine skeleton.

---

## Week 2 — Robust Intake, Validation, and Quarantine

### Must Deliver

- accepted-record contract;
- stable validation error categories;
- quarantine record/model;
- parser handling success, unauthorized failure, malformed, unknown, and partial records;
- deterministic CLI exits and output locations;
- unit/integration test suite;
- changed-rule ownership check.

### Daily assignments

- **Monday:** freeze minimum accepted fields and validation invariants; implement validation result types.
- **Tuesday:** implement malformed/partial handling and quarantine output.
- **Wednesday:** implement unknown-record handling and parser diagnostics without false normalization.
- **Thursday:** define CLI exit codes, input/output behavior, and batch-file behavior.
- **Friday:** complete behavior matrix tests and changed-input diagnosis.
- **Saturday:** run clean fixture suite; Ali adds/modifies one field or rule and tests it; close gate.

---

## Week 3 — SQLite Persistence and SQL

### Must Deliver

- database initialization path;
- tables for runs, normalized events, quarantined records, and source metadata;
- deterministic run ID;
- insertion transaction behavior;
- explicit duplicate/replay behavior;
- required SQL query set;
- persistence/integration tests.

### Daily assignments

- **Monday:** design minimum schema from existing event contract; implement initialization.
- **Tuesday:** implement runs and source metadata insertion.
- **Wednesday:** implement normalized-event and quarantine insertion with transactions.
- **Thursday:** implement duplicate/replay rules and tests.
- **Friday:** write required `SELECT`, `WHERE`, `GROUP BY`, `ORDER BY`, and justified `JOIN` queries.
- **Saturday:** run CLI-to-database integration; Ali writes/explains required queries; close gate.

---

## Week 4 — Detection and Raw-to-Report Vertical Slice

### Must Deliver

- configurable time-window failed-authentication detector;
- finding model linked to evidence/run identity;
- concise report output;
- raw-to-report CLI command;
- replay behavior;
- integration tests for normal, below threshold, threshold crossing, malformed, and duplicate cases;
- one deliberate detector/input failure diagnosis.

### Daily assignments

- **Monday:** define detector contract and implement time-window grouping.
- **Tuesday:** implement finding model and evidence references.
- **Wednesday:** implement report rendering and CLI wiring.
- **Thursday:** implement replay and deterministic output tests.
- **Friday:** complete full behavior matrix and deliberate fault diagnosis.
- **Saturday:** execute clean raw-to-report gate; Ali changes threshold and predicts/verifies outcome.

---

## Week 5 — Docker SSH Scenario Adapter

### Must Deliver

- bounded Docker client and target;
- explicit network/exposure boundary;
- lab identities/configuration isolated from host state;
- normal/failure scenario commands;
- truth and run markers;
- evidence collection and cleanup;
- pipeline ingestion of Docker evidence.

### Daily assignments

- **Monday:** define adapter contract and Docker topology without changing scenario semantics.
- **Tuesday:** implement target, client, identities, and network boundary.
- **Wednesday:** run normal case; preserve truth and evidence; process through pipeline.
- **Thursday:** run repeated failure; preserve truth and evidence; process through pipeline.
- **Friday:** implement reset/cleanup and compare namespace/Docker evidence.
- **Saturday:** clean reconstruction and full adapter gate.

---

## Week 6 — Scenario Matrix, Replay, and CI

### Must Deliver

- run matrix with varied failure counts and spacing;
- deterministic run identity and manifest;
- replay command;
- namespace/Docker comparison artifact;
- clean checkout test command;
- GitHub Actions CI;
- evidence/artifact inventory.

### Daily assignments

- **Monday:** implement run manifest and repeat command.
- **Tuesday:** run count variants and verify detector boundary.
- **Wednesday:** run timing variants and verify time-window behavior.
- **Thursday:** implement replay and output-hash/determinism checks where justified.
- **Friday:** configure CI and fix clean-checkout failures.
- **Saturday:** execute scenario matrix and CI gate; record environment differences.

---

## Week 7 — Reliability Closure

### Must Deliver

- clean-state setup result;
- malformed, missing, partial, unknown, duplicate, and replay tests;
- parser/schema-version mismatch behavior;
- unavailable/corrupt database behavior;
- processing failure and recovery;
- Docker/environment failure and recovery;
- limitations register;
- two reduced-prompt diagnoses.

### Daily assignments

- **Monday:** clean-state setup and missing-dependency failure.
- **Tuesday:** evidence-quality failure matrix.
- **Wednesday:** persistence/database failure matrix.
- **Thursday:** environment/service/network failure matrix.
- **Friday:** repair/recovery validation and limitations.
- **Saturday:** two changed-case diagnosis checks and full reliability gate.

---

## Week 8 — Experimental Run Dataset

### Must Deliver

- explicit experimental question;
- run/scenario unit of analysis;
- controlled run-generation matrix;
- independent truth labels;
- run-level feature table;
- provenance and dataset manifest;
- leakage groups and intended role split;
- data-quality tests.

### Daily assignments

- **Monday:** define question, unit, outcomes, and non-goals.
- **Tuesday:** design and execute first controlled run matrix.
- **Wednesday:** derive run-level features and bind to provenance.
- **Thursday:** define groups/splits and test leakage constraints.
- **Friday:** data-quality and support analysis; register evidence gaps.
- **Saturday:** fill only gate-critical run gaps; freeze dataset version.

---

## Week 9 — Rule Baseline and Error Analysis

### Must Deliver

- frozen rule configuration;
- evaluation code and population manifest;
- precision, recall, false-positive, false-negative, and invalid/abstention counts where relevant;
- threshold sensitivity;
- per-scenario error analysis;
- data-sufficiency decision;
- justified ML question or explicit ML rejection.

### Daily assignments

- **Monday:** freeze evaluation population and rule.
- **Tuesday:** implement and validate metrics.
- **Wednesday:** run threshold sensitivity.
- **Thursday:** inspect false positives/negatives by scenario group.
- **Friday:** evaluate support, leakage, and limitations.
- **Saturday:** close registered evidence gaps only; issue ML/no-ML decision gate.

---

## Week 10 — Honest Simple-ML Decision

### Must Deliver

- group-safe split;
- reproducible preprocessing/training pipeline;
- one smallest justified model;
- comparison with frozen rule;
- error analysis;
- limitations and public claim boundary;
- Ali explanation of features, split, metrics, and one error.

### Daily assignments

- **Monday:** choose smallest justified model and freeze inputs.
- **Tuesday:** implement reproducible training and baseline checks.
- **Wednesday:** evaluate held-out groups and verify no leakage.
- **Thursday:** compare errors and operational behavior with rule.
- **Friday:** perform sensitivity/limitations and draft decision.
- **Saturday:** ownership check and final ML decision; stop model work.

---

## Week 11 — Engineering Hardening

### Must Deliver

- code/module boundary review;
- type, lint, unit, integration, and CI checks;
- deterministic configuration/setup;
- error-message and failure-behavior cleanup;
- security/exposure assumptions;
- dependency and secrets review;
- Ali clean reconstruction attempt;
- ownership-gap register.

### Daily assignments

- **Monday:** structure/type/lint audit and repairs.
- **Tuesday:** configuration, paths, setup, and deterministic fixture cleanup.
- **Wednesday:** error messages, exit behavior, and test gaps.
- **Thursday:** security boundary, secrets, permissions, exposure, and threat assumptions.
- **Friday:** Ali reconstructs system from requirements/instructions with reduced help.
- **Saturday:** repair only presentation-blocking defects; freeze technical scope.

---

## Week 12 — Portfolio and Interview Package

### Must Deliver

- accurate README;
- architecture/data-flow diagram;
- tested setup and demo instructions;
- sample raw evidence, normalized event, quarantine, database query, finding, and report;
- test/CI evidence;
- rule/ML comparison;
- limitations;
- AI-assistance disclosure;
- short demo recording where feasible;
- concise technical defense and question set.

### Daily assignments

- **Monday:** README identity, problem, scope, and honest status.
- **Tuesday:** architecture/data/evidence diagrams.
- **Wednesday:** clean setup/demo script and verification.
- **Thursday:** sample evidence/results, limitations, and AI disclosure.
- **Friday:** record demo and conduct technical defense.
- **Saturday:** external-review preflight; freeze portfolio package.

---

## Week 13 — External and Market Calibration

### Must Deliver

- at least one external review request;
- clean setup attempt by another person where feasible;
- 5–10 selected job descriptions and requirement matrix;
- 5–10 calibration applications;
- valid feedback corrections;
- Day 90 ownership and execution evaluation;
- evidence-based next-period decision.

### Daily assignments

- **Monday:** send review/setup requests and select role set.
- **Tuesday:** compare portfolio evidence to role requirements and repair obvious presentation gaps.
- **Wednesday:** submit first application batch.
- **Thursday:** submit remaining calibration applications and practice project explanation.
- **Friday:** integrate valid external feedback and complete evidence inventory.
- **Saturday:** Day 90 evaluation and next-period decision.

## Carry rule

When a week fails:

1. use remaining Saturday capacity;
2. cut optional presentation and scenario variety;
3. carry only the blocking gate item;
4. preserve later deadlines where technically possible;
5. block ML when the core pipeline or reliable data is incomplete;
6. never create a replacement roadmap.