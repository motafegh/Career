# Deferred AegisLab 90-Day Master Plan — Historical Only

> [!CAUTION]
> **This plan is deferred, superseded for active execution, and non-controlling. Do not execute its phases, gates, deliverables, or next actions.**
>
> UpgradePilot is the formally selected primary 90-day flagship. [`../UpgradePilot.md`](../UpgradePilot.md) is the governing project charter. Broad project comparison is closed. UpgradePilot implementation has not started, and the replacement UpgradePilot master roadmap has not yet been created.
>
> The next authorized action is to create the **UpgradePilot Learning and Execution Contract**. The original AegisLab plan below is preserved as historical planning evidence and does not transfer architecture, sequencing, modules, or tasks into UpgradePilot.

---

# 90-Day Master Plan

**Historical status:** Deferred by the formal UpgradePilot selection decision; not an active roadmap.  
**Day 1:** 2026-07-20  
**Day 90:** 2026-10-17  
**Standard workload:** 24 focused hours per week  
**Planned technical capacity:** approximately 312 focused hours before health-adjusted exceptions

## Program outcome

By Day 90, AegisLab must contain one honest, reproducible, tested security-evidence vertical slice demonstrating:

- Python application/package structure;
- SSH evidence parsing and normalization;
- explicit validation and quarantine;
- SQLite persistence and useful SQL;
- deterministic run and evidence identity;
- rule-based detection and report generation;
- namespace and Docker scenario adapters;
- automated tests and CI;
- evidence-based failure diagnosis;
- a leakage-aware rule baseline and honest simple-ML decision;
- an accurate portfolio presentation Ali can explain, modify, test, query, and diagnose.

## Phase 0 — Preparation

**Dates:** 2026-07-18 to 2026-07-19  
**Maximum:** 45 focused minutes Saturday plus 15 minutes Sunday

Required:

- read the controlling route once;
- confirm AegisLab workspace, branch, current state, worklog, and runbook;
- confirm Sentinel is inactive;
- record Monday's first technical action.

Gate P0:

- the first production session can begin without additional planning;
- no technical implementation or system redesign occurred.

## Phase 1 — Namespace closure and Python intake foundation

**Week:** 1  
**Dates:** 2026-07-20 to 2026-07-26  
**Budget:** 24 focused hours

Required namespace outputs:

- bounded normal-authentication case;
- bounded unauthorized-key failure case;
- explicit truth, timestamps, markers, abort conditions, and cleanup;
- complete server-log/client/process/socket/packet evidence map;
- one deliberately broken layer, evidence-based diagnosis, repair, and revalidation;
- reduced-prompt ownership explanation;
- two sanitized representative SSH log fixtures.

Required Python outputs:

- `pyproject.toml` or equivalent project configuration;
- importable `src/aegislab` package;
- typed normalized authentication-event model;
- parser supporting one success and one failed-authentication record family;
- CLI command that reads a fixture and emits normalized JSON;
- tests for the required success/failure mappings.

Gate P1:

- namespace work is explicitly closed at the declared depth;
- the two scenario fixtures are reproducible and sanitized;
- the parser/CLI emits valid normalized events from both fixture types;
- tests pass;
- Ali can explain every initial event field and modify one parser mapping.

Hard stop:

No further namespace-only expansion after Gate P1. Remaining environment depth is deferred until Docker transfer.

## Phase 2 — Validation, quarantine, persistence, and first complete vertical slice

**Weeks:** 2–4  
**Dates:** 2026-07-27 to 2026-08-16  
**Budget:** 72 focused hours

### Week 2 — Robust intake

Required:

- explicit accepted/rejected record contract;
- validation errors with stable categories;
- quarantine representation and output;
- parser coverage for required success, unauthorized-key failure, malformed, unknown, and partial records;
- CLI exit behavior and error messages;
- unit and integration tests;
- ownership modification and changed-case diagnosis.

Gate:

- valid records normalize predictably;
- invalid/unknown records cannot silently become trusted events;
- CLI output and exit behavior are deterministic;
- Ali can add or change one field/rule and its tests.

### Week 3 — SQLite and SQL

Required:

- SQLite schema and migration/initialization path;
- normalized events, quarantined records, runs, and source metadata;
- deterministic run identity;
- insertion and duplicate behavior;
- useful `SELECT`, `WHERE`, `GROUP BY`, `ORDER BY`, and required `JOIN` queries;
- persistence tests and explainable schema choices.

Gate:

- CLI ingests fixtures into SQLite;
- required queries return verified results;
- duplicate/replay behavior is explicit;
- Ali can write and explain the required SQL without copying an opaque answer.

### Week 4 — Detection and report vertical slice

Required:

- time-window repeated-failure detector;
- detector configuration;
- finding representation;
- concise evidence-backed report;
- raw-to-report command;
- replay behavior;
- integration tests for normal, threshold-crossing, below-threshold, malformed, and duplicate cases;
- one deliberate broken-input or detector failure diagnosis.

Gate P2:

One clean command performs:

```text
raw SSH evidence
→ parse
→ validate/quarantine
→ persist
→ detect
→ report
```

The result is deterministic for known fixtures, failure behavior is explicit, and Ali can change the threshold and explain the resulting behavior.

## Phase 3 — Docker transfer, repeatability, and reliability

**Weeks:** 5–7  
**Dates:** 2026-08-17 to 2026-09-06  
**Budget:** 72 focused hours

### Week 5 — Docker scenario adapter

Required:

- controlled client and SSH target;
- network exposure boundary;
- normal and repeated-failure cases;
- independent truth record;
- evidence collection;
- cleanup and reset;
- evidence fed through the existing Python path.

Gate:

- Docker preserves scenario meaning;
- the same pipeline processes Docker evidence;
- normal/failure results match truth.

### Week 6 — Scenario matrix and CI

Required:

- repeated run identities;
- varied failure counts and time spacing;
- namespace/Docker comparison;
- replay command;
- clean checkout test path;
- GitHub Actions CI for unit/integration tests;
- artifact/evidence inventory.

Gate:

- multiple bounded scenarios run reproducibly;
- CI passes from the repository state;
- environment differences are explicit.

### Week 7 — Reliability closure

Required:

- clean-state setup test;
- malformed/missing/partial/duplicate evidence tests;
- processing failure and recovery;
- environment failure and recovery;
- SQLite corruption or unavailable-database behavior bounded safely;
- parser version/schema mismatch behavior;
- limitations register.

Gate P3:

- known failure paths do not silently produce trusted findings;
- clean instructions reconstruct the bounded system;
- Ali diagnoses at least two changed failures with reduced prompting.

## Phase 4 — Data experiment, rule baseline, and honest ML decision

**Weeks:** 8–10  
**Dates:** 2026-09-07 to 2026-09-27  
**Budget:** 72 focused hours

### Week 8 — Experimental run dataset

Required:

- explicit experimental question;
- scenario/run unit of analysis;
- controlled run generator or matrix;
- run-level labels/truth;
- feature table derived only from available evidence;
- provenance and split groups;
- data-quality checks.

Gate:

- dataset rows map to reproducible runs;
- truth is not inferred solely from detector output;
- leakage groups are explicit.

### Week 9 — Rule evaluation and error analysis

Required:

- frozen rule baseline;
- precision, recall, false-positive, false-negative, and abstention/invalid counts where relevant;
- threshold sensitivity;
- scenario-group error analysis;
- sufficiency judgment;
- additional controlled runs only for registered evidence gaps.

Gate:

- rule behavior is quantitatively and qualitatively understood;
- a justified ML question exists or ML is rejected.

### Week 10 — Simple ML decision

Permitted models:

- logistic regression;
- shallow decision tree;
- small random forest only when justified.

Required:

- group-safe training/evaluation split;
- reproducible pipeline;
- comparison with the rule baseline;
- error analysis;
- limitations and claim boundary;
- clear decision: useful, not useful, insufficient data, or educational only.

Gate P4:

- conclusion is evidence-backed;
- rule remains the baseline;
- no advanced model or architecture search is added;
- Ali can explain features, split, metric, and one model error.

## Phase 5 — Engineering hardening and portfolio closure

**Weeks:** 11–12  
**Dates:** 2026-09-28 to 2026-10-11  
**Budget:** 48 focused hours

### Week 11 — Engineering hardening

Required:

- code organization review;
- type/lint/test checks;
- configuration and error-message cleanup;
- deterministic setup and demo data;
- security boundary review;
- threat/failure assumptions;
- one independent reconstruction attempt by Ali;
- ownership gaps list.

Gate:

- the system is stable enough to present honestly;
- critical setup or correctness defects are closed or explicitly bounded.

### Week 12 — Portfolio package

Required:

- accurate README;
- architecture/data-flow diagram;
- tested setup instructions;
- demo script and short recording where feasible;
- sample fixtures, evidence, finding, and report;
- tests and CI evidence;
- rule/ML comparison;
- limitations;
- AI-assistance disclosure;
- concise personal technical explanation and likely interview questions.

Gate P5:

- another engineer can understand and attempt setup;
- claims match reproducible evidence;
- Ali can explain, modify, test, query, and diagnose central components.

## Phase 6 — External calibration and final review

**Week:** 13  
**Dates:** 2026-10-12 to 2026-10-17  
**Budget:** 24 focused hours

Required:

- at least one external repository review request;
- one clean setup attempt by another person when feasible;
- comparison against selected real job descriptions;
- 5–10 calibration applications;
- repository/README corrections from valid feedback;
- ownership assessment;
- Day 90 evaluation;
- next-period decision.

Gate P6:

- external feedback exists;
- market assumptions are tested;
- the next plan is based on evidence rather than internal speculation.

## Program success

The program succeeds when:

1. AegisLab is a finished bounded vertical slice rather than another expanding architecture;
2. Python, validation, SQLite, testing, debugging, Docker, and CI are demonstrated;
3. the rule and ML decisions are honest and evidence-qualified;
4. Ali can defend central design and failure behavior;
5. the public portfolio is accurate;
6. external calibration has begun;
7. no new primary project was started.