---
name: career-claim-audit
description: >
  Audit whether Career-facing claims about Ali, his projects, skills, ownership, experience, metrics, readiness, or production status are actually supported. Use when the requested result is what a CV/resume, GitHub, portfolio, LinkedIn, application, interview, or project description may truthfully say; especially for wording such as built, owned, production-ready, expert, demonstrated, improved by X%, or similar. Decompose compound sentences into atomic claims, trace each to canonical evidence and AI-assistance boundaries, and return the strongest defensible wording. If the primary request is the underlying D-level/capability itself, use capability-assessment. If the primary request is a formal final Career decision such as application readiness, strategy, project allocation, or live positioning, use career-review as primary and use this as supporting claim analysis. Do not use for market calibration or ordinary copyediting with no factual-claim question.
compatibility: Designed for the motafegh/Career repository and agents that can inspect Career claim owners plus underlying project evidence when a material claim depends on it.
---

# Career Claim Audit

## Purpose

Audit the factual and evidentiary strength of Career-facing claims before they are published, submitted, or used in interviews.

This skill owns the **claim-audit procedure**. It does not redefine Ali's capability, project truth, market evidence, or Career state. Those remain with their canonical owners.

The objective is the strongest defensible claim, not maximum caution and not maximum promotion.

## Load only the truth owners needed for the claim

1. Follow [`../../../AGENTS.md`](../../../AGENTS.md) and the Career authority order.
2. Use [`../../../profile/CAREER_PROFILE.md`](../../../profile/CAREER_PROFILE.md) for public-safe personal and professional facts.
3. Use [`../../../tracking/CAPABILITY_EVIDENCE_LEDGER.md`](../../../tracking/CAPABILITY_EVIDENCE_LEDGER.md) when a claim implies demonstrated capability, ownership, or skill depth.
4. Use [`../../../portfolio/PROJECT_PORTFOLIO.md`](../../../portfolio/PROJECT_PORTFOLIO.md) and the relevant project-specific Career record when the claim concerns project role, Ali-versus-AI contribution, or portfolio positioning.
5. Use [`../../../market/ALI_RAJABI_MASTER_CV.md`](../../../market/ALI_RAJABI_MASTER_CV.md) when auditing or changing the canonical CV wording.
6. Read [`../../../CAREER_STATE.md`](../../../CAREER_STATE.md) only when the claim depends on current working identity, employability/application phase, or another live Career conclusion.
7. Inspect underlying project source/tests/evidence only when a material project-behavior or contribution claim cannot be validated safely from Career's current canonical records.

Do not load every owner for every sentence. Route each atomic claim to the smallest relevant source.

## Claim-audit workflow

### 1. Identify the surface and audience

Determine where the claim will appear:

- master or tailored CV;
- GitHub/profile/project description;
- portfolio page;
- LinkedIn or public post;
- application answer;
- interview explanation;
- internal Career record.

Apply the repository's public/private boundary. A truthful fact may still be inappropriate for the public Career repository.

### 2. Decompose compound wording into atomic claims

Do not audit a promotional sentence as one indivisible statement.

Example:

> I built a production-ready FastAPI/SQLite AI platform used for career intelligence.

Contains separate propositions such as:

- the product exists;
- it uses FastAPI;
- it uses SQLite;
- it has AI functionality;
- Ali personally built/implemented it;
- it is production-ready;
- it is used for the stated purpose.

Each proposition may have a different verdict.

### 3. Classify each claim

Useful claim classes include:

- **Personal fact** — employment, role history, dates, education, language, location, etc.
- **Project/product fact** — what a repository or system demonstrably does or uses.
- **Ali contribution** — what Ali directed, implemented, modified, tested, diagnosed, verified, researched, or decided.
- **Capability/skill** — what Ali can personally defend or perform.
- **Status/readiness** — production-ready, deployed, validated, application-ready, complete, operational, etc.
- **Metric/outcome** — counts, percentages, performance, revenue, scale, speed, quality, users, time saved, etc.
- **Experience/seniority** — junior, senior, professional, years of technical experience, team experience, ownership level.

Do not let evidence for one class silently support another.

### 4. Locate the canonical evidence

For each atomic claim, identify:

- the Career truth owner;
- the underlying evidence when needed;
- date/freshness;
- assistance or authorship boundary;
- known uncertainty or transfer limit.

If a capability proposition is not already settled, do not infer it from the project stack. Use the canonical Career capability evidence and, when necessary, require a proper capability reassessment rather than solving it through wording.

If a project behavior is uncertain, inspect project evidence rather than converting portfolio prose into technical proof.

### 5. Separate subject from system

Be precise about **who or what** performed the action.

These are materially different:

- `The repository implements X.`
- `AI-assisted development produced X under Ali's direction.`
- `Ali verified X.`
- `Ali materially modified and tested X.`
- `Ali independently implemented X.`

Do not use first-person authorship when only the product fact is established.

AI assistance should be disclosed at the level needed to keep the claim accurate, but do not mechanically repeat a disclaimer in every sentence when the surrounding section already makes the boundary clear.

### 6. Audit technology claims carefully

Distinguish:

- technology present in a repository;
- exposure/familiarity;
- guided use;
- demonstrated capability;
- independent ownership.

A project importing FastAPI or using SQLite does not by itself justify listing FastAPI/API design or SQL as demonstrated personal capability.

### 7. Audit status and readiness language

Treat words such as these as evidence-bearing claims:

- production-ready;
- production-grade;
- deployed;
- battle-tested;
- reliable;
- secure;
- validated;
- complete;
- autonomous;
- job-ready;
- expert.

Require evidence appropriate to the claimed scope. `Production-oriented` and `production-ready` are not interchangeable.

### 8. Audit metrics and counts

A numeric claim must have a traceable basis and correct denominator/scope.

Do not invent or preserve unsupported metrics merely because they strengthen a CV bullet.

When only a narrower count is supported, keep the count narrow. When the number is approximate, label it honestly if approximation is defensible and useful.

### 9. Assign a verdict to each atomic claim

Use one of these practical outcomes:

- **Supported** — evidence directly supports the claim as written.
- **Supported with narrowing** — the underlying fact is real but wording overstates scope, authorship, depth, status, or certainty.
- **Unsupported** — current evidence contradicts or does not support the assertion strongly enough.
- **Unresolved/stale** — evidence may exist but is insufficient, outdated, or not yet verified for the proposed wording.
- **Private-not-public** — may be truthful but should not be placed in the public Career repository or public-facing artifact.

Do not turn `unresolved` into `false`.

### 10. Produce the strongest defensible wording

When rewriting is part of the request, preserve specificity and value while removing only the unsupported component.

Prefer:

> Directed and evaluated AI-assisted development of a local-first career-intelligence product using FastAPI and SQLite; implementation remains substantially AI-generated and is not claimed as independent source ownership.

Over a vague fallback such as:

> Worked on an AI project.

The goal is evidence-bounded strength, not self-erasure.

### 11. Check cross-document consistency when material

A claim can be individually plausible but inconsistent with another Career artifact.

When the same material claim appears across CV, portfolio, GitHub positioning, project records, or capability records, verify that differences reflect audience/format rather than contradictory ownership or capability assertions.

Do not create duplicate truth owners just to make wording consistent.

### 12. Persist only when requested or required

Do not edit the CV, portfolio, profile, state, or project records merely because this skill identified a claim issue.

Persist only when Ali explicitly asks to update the artifact or an active Career review/application workflow requires the change under repository governance. Update the canonical owner rather than scattering the same correction across unrelated files.

## Invalid shortcuts

Never use these shortcuts:

- repository uses technology = Ali owns technology;
- project sophistication = personal capability;
- market demand = demonstrated skill;
- AI-assisted project = no legitimate Ali contribution;
- product behavior = personal authorship;
- passing tests = production-ready;
- project is production-oriented = production-ready;
- one supported fact = whole compound sentence supported;
- approximate memory = verified metric;
- stronger wording = better wording.

## Output

Keep small audits concise. For material or multi-claim audits, use a structure such as:

| Atomic claim | Verdict | Evidence/owner | Problem if any | Strongest defensible form |
|---|---|---|---|---|

Then state, when relevant:

- overall claim risk;
- capability or project evidence that remains unresolved;
- privacy/public-safety issue;
- exact artifact that should change if persistence is authorized.

If the user asked for finished replacement wording, provide the final evidence-bounded wording after the audit.

## Final checks

Before finalizing, verify that:

- compound promotional language was decomposed when needed;
- each claim was routed to the right truth owner;
- product facts, Ali contribution, capability, status, and metrics were not conflated;
- AI assistance/authorship was represented accurately;
- unresolved evidence was not treated as false;
- the wording retained the strongest supportable value rather than becoming unnecessarily weak;
- public/private boundaries were respected;
- no Career artifact was changed merely because the skill ran.
