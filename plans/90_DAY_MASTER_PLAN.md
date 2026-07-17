# 90-Day Master Plan

**Day 1:** 2026-07-20  
**Day 90:** 2026-10-17  
**Committed baseline:** 15 focused hours per week

## Program outcome

By Day 90, AegisLab must contain one honest, reproducible, tested vertical slice demonstrating Python/data engineering with secure-engineering practices and an evidence-qualified ML decision.

## Phase 0 — Preparation

**Dates:** 2026-07-18 to 2026-07-19  
**Maximum:** 2 focused hours

Required:

- read the Career control files once;
- confirm AegisLab is the sole active project;
- place Sentinel under the archive boundary;
- inspect the current AegisLab state;
- activate Week 1;
- do not redesign either project.

Gate P0:

- Career repository is readable and controlling;
- first session can begin without another planning discussion.

## Phase 1 — Close namespace SSH understanding

**Weeks:** 1–2  
**Dates:** 2026-07-20 to 2026-08-02  
**Budget:** 30 focused hours

Required:

- correlate successful and failed SSH attempts with foreground server logs;
- map client, process, socket, log, and packet evidence;
- define normal-authentication and repeated-failure cases;
- establish expected truth, fixed counts, timing, markers, abort conditions, and cleanup;
- run both bounded cases;
- break one layer, diagnose it, repair it, and revalidate;
- explain and reconstruct the mechanism with materially reduced prompting.

Gate P1:

- namespace scenario meaning is explicit;
- evidence sources and limitations are explainable;
- bounded cases are reproducible;
- one fault has been diagnosed;
- remaining noncritical SSH depth is deferred.

Hard stop:

No more namespace expansion after Gate P1.

## Phase 2 — Python evidence pipeline foundation

**Weeks:** 3–4  
**Dates:** 2026-08-03 to 2026-08-16  
**Budget:** 30 focused hours

Required:

- Python package/application structure;
- CLI skeleton;
- configuration boundary;
- raw SSH fixtures;
- normalized authentication-event model;
- parser;
- explicit validation;
- quarantine path;
- unit-test foundation;
- malformed and changed-input tests.

Gate P2:

- a raw fixture is parsed into a validated normalized event;
- invalid input is rejected or quarantined predictably;
- tests prove both success and failure behavior;
- the user can explain and modify one parsing rule.

## Phase 3 — Persistence and complete vertical slice

**Weeks:** 5–6  
**Dates:** 2026-08-17 to 2026-08-30  
**Budget:** 30 focused hours

Required:

- SQLite schema;
- foundational SQL;
- run identity and source/environment metadata;
- event insertion and useful queries;
- rule-based time-window detector;
- finding representation;
- concise report;
- unit and integration tests;
- replay command;
- deliberate broken-input diagnosis.

Gate P3:

A clean command performs:

```text
raw evidence
→ parse
→ validate/quarantine
→ persist
→ detect
→ report
```

The output is correct for known fixtures and failure behavior is explicit.

## Phase 4 — Docker transfer and repeatability

**Weeks:** 7–8  
**Dates:** 2026-08-31 to 2026-09-13  
**Budget:** 30 focused hours

Required:

- Docker client and target preserving the namespace scenario meaning;
- normal and repeated-failure cases;
- evidence preservation;
- setup and cleanup;
- independent truth record;
- multiple run identities;
- changed failure count and timing;
- replay support;
- namespace/Docker evidence comparison;
- CI for Python tests.

Gate P4:

- the scenario runs reproducibly in Docker;
- the same pipeline processes its evidence;
- comparisons describe environment differences without changing scenario semantics;
- CI passes.

## Phase 5 — Reliability closure

**Week:** 9  
**Dates:** 2026-09-14 to 2026-09-20  
**Budget:** 15 focused hours

Required:

- clean-state setup test;
- malformed evidence test;
- missing-record test;
- duplicate/replay test;
- one processing failure;
- one environment failure;
- evidence-based diagnosis and recovery;
- limitations record.

Gate P5:

- known failure paths are tested or explicitly bounded;
- setup is reproducible from clean instructions;
- failures do not silently produce trustworthy findings.

## Phase 6 — Rule baseline and ML-ready experiment

**Week:** 10  
**Dates:** 2026-09-21 to 2026-09-27  
**Budget:** 15 focused hours

Required:

- run-level dataset;
- explicit feature definitions;
- leakage groups;
- split by run/scenario group;
- rule baseline;
- precision, recall, false-positive analysis;
- data sufficiency assessment.

Gate P6:

- rule performance is measurable;
- evaluation populations are explicit;
- leakage risks are controlled or documented;
- a justified ML question exists—or ML is rejected.

## Phase 7 — Honest ML decision

**Week:** 11  
**Dates:** 2026-09-28 to 2026-10-04  
**Budget:** 15 focused hours

Permitted models:

- logistic regression;
- shallow decision tree;
- small random forest only when justified.

Required:

- reproducible training;
- comparison with rule baseline;
- limitations;
- no inflated language;
- clear decision: useful, not useful, insufficient data, or educational only.

Gate P7:

- the ML conclusion is evidence-backed;
- the rule remains the comparison baseline;
- no advanced model is added.

## Phase 8 — Portfolio closure

**Week:** 12  
**Dates:** 2026-10-05 to 2026-10-11  
**Budget:** 15 focused hours

Required:

- accurate README;
- architecture diagram;
- tested setup instructions;
- demo script;
- sample evidence and report;
- tests and CI evidence;
- limitations;
- AI-assistance disclosure;
- concise personal technical explanation.

Gate P8:

- another person can understand and attempt setup;
- claims match evidence;
- the user can explain, modify, test, and diagnose central components.

## Phase 9 — External calibration and final review

**Week:** 13  
**Dates:** 2026-10-12 to 2026-10-17  
**Budget:** 15 focused hours

Required:

- external repository review;
- clean setup attempt by another person when feasible;
- 5–10 calibration applications;
- comparison with actual role requirements;
- ownership assessment;
- Day 90 evaluation;
- next-period decision.

Gate P9:

- external feedback exists;
- market assumptions are tested;
- the next plan is based on evidence rather than internal speculation.

## Program success

The program succeeds when:

1. AegisLab is a finished bounded vertical slice rather than another expanding architecture;
2. Python, validation, SQLite, testing, debugging, Docker, and CI are demonstrated;
3. the ML decision is honest and baseline-driven;
4. the public portfolio is accurate;
5. external calibration has begun;
6. no new primary project was started.