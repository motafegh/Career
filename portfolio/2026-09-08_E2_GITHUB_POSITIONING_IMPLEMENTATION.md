# E2 GitHub Positioning Implementation Package

**Date:** 2026-09-08  
**Status:** ACTIVE / PARTIALLY EXECUTABLE FROM CAREER  
**Owner:** Career portfolio and claim positioning  
**Decision source:** `../CAREER_STATE.md` and `../tracking/research/2026-09-07_A6_PORTFOLIO_AND_GITHUB_E2_POSITIONING_AUDIT.md`

## 1. Purpose

Close the minimum employer-facing GitHub positioning gap without redesigning every repository or inflating Ali's ownership claims.

E2-P0 closes when:

- the GitHub profile has a concise employer-facing README;
- UpgradePilot, JobHunter, and Sentinel have clear repository-card descriptions/topics;
- the general profile pins are curated around those three projects;
- each project first screen exposes the correct Ali-versus-AI contribution boundary;
- the public Career repository is kept out of the primary recruiter path and does not duplicate stale employability status.

This package is the Career-owned wording/claim source. Technical project repositories remain responsible for applying their own README changes under their local rules.

---

## 2. GitHub profile README — approved E2 copy

Target repository: `motafegh/motafegh`  
Target file: `README.md`

```markdown
# Ali Rajabi

**Junior Software Engineer | Python, Data & Applied AI**

I am transitioning from substantial business and operational responsibility into software engineering, with a current focus on Python, data/evidence systems, and applied AI.

I use modern AI coding agents heavily, but I do not treat generated code as automatic engineering ownership. My current learning and project work emphasizes understanding system behavior, challenging designs, verifying evidence, reasoning about tests and failures, making meaningful changes, and becoming progressively more capable of defending the work independently.

## Selected projects

### [UpgradePilot](https://github.com/motafegh/UpgradePilot)
Evidence-backed decision support for maintainers reviewing Python dependency-update pull requests. It combines public GitHub, PyPI, upstream, CI, and repository evidence while preserving explicit uncertainty and abstention. UpgradePilot is my primary capability-building project: I direct product/evidence decisions, challenge architecture and proof boundaries, verify selected behavior, and am progressively working through current source and tests. Development is substantially AI-assisted and I do not present the complete repository as independently authored by me.

### [JobHunter](https://github.com/motafegh/jobhunter)
A local-first career-intelligence system built around provenance-preserving job evidence, deterministic source truth, reviewed semantic analysis, and reusable market/work intelligence. I direct and evaluate the AI-assisted development, especially the product boundaries around evidence, semantic authority, review, and fail-closed promotion. I do not claim independent ownership of the full FastAPI/SQLite/LLM implementation.

### [Sentinel](https://github.com/motafegh/sentinel-)
A smart-contract security and ML/data research project. My original Sentinel work was a long-running AI-assisted learning project involving Python, data pipelines, model training, Linux, and repeated dataset/model-quality problems. The later R4 continuation is AI-led research under my direction and is presented separately from my personal implementation capability. Its strongest current story is evidence-driven data/evaluation repair and refusing stronger training claims when supervision is insufficient.

## Current engineering direction

My current depth model is intentionally anchored rather than technology-collecting:

- Python and software-engineering fundamentals;
- data, evidence, and relational foundations;
- applied AI / LLM / agent systems as a differentiating area;
- secure, trustworthy, and evaluative engineering across the stack;
- backend, cloud, CI, Linux, networking, and operations when real responsibilities require them.

I am currently most interested in mentored junior or early-career roles around Applied AI / AI Implementation, technical implementation and automation, Python applications, and backend/integration work.

## Background

Before this transition I spent roughly six to seven years in a family manufacturing business across management, sales, purchasing, coordination, and operational decision-making. That experience remains relevant to how I approach requirements, prioritization, stakeholder communication, and ownership of outcomes.
```

Do not add unverified degrees, certifications, location/work-authorization claims, LinkedIn, phone number, or other contact details merely to make the profile look complete.

---

## 3. Repository-card metadata

### UpgradePilot

**Description**

```text
Evidence-backed decision support for Python dependency-update pull requests, with explicit provenance, uncertainty and abstention.
```

**Topics**

```text
python
dependabot
dependency-management
github-actions
software-supply-chain
evidence
llm
ai-assisted-development
```

### JobHunter

**Description**

```text
Local-first career intelligence from provenance-preserving job evidence and reviewed AI analysis.
```

**Topics**

```text
python
fastapi
sqlite
career-intelligence
job-analysis
llm
local-first
provenance
```

### Sentinel

**Description**

```text
AI-assisted smart-contract security and ML/data research with evidence-driven data and evaluation controls.
```

**Topics**

```text
python
machine-learning
smart-contract-security
solidity
data-quality
model-evaluation
security-research
ai-assisted-development
```

Keep topics selective. Do not add every technology visible somewhere in repository history.

---

## 4. General GitHub pin order

Recommended broad-profile order:

```text
1. UpgradePilot
2. jobhunter
3. sentinel-
```

Do not feature `Career` as a primary portfolio project. Older learning/tutorial/experimental repositories should not precede these three on the general profile.

Role-specific CV/application material may reorder projects without changing the general profile pins.

---

## 5. UpgradePilot README handoff

The project README already has a technically useful quickstart and strong claim discipline. Do not rewrite it broadly.

Project-local README work should insert an employer-facing layer immediately after the opening product definition and before the detailed quickstart. That layer should answer:

1. What works today?
2. Why is this distinct from generic dependency automation or generic AI code review?
3. What is the shortest inspectable flow?
4. What is Ali's actual contribution and what is AI-assisted?
5. What is not yet proven/complete?

Approved claim boundary:

```text
Ali directs and learns through the AI-assisted development of UpgradePilot, including product/evidence decisions, repeated challenge of scope and proof boundaries, selected pre-change design decisions, and bounded current source/test reasoning. The repository's substantive implementation and tests are heavily AI-assisted; the complete Python/test architecture is not presented as independently authored or independently owned by Ali.
```

Do not claim the final maintainer recommendation is implemented until project truth says so. Do not claim production readiness, safe upgrades, complete compatibility proof, or independent full-repository authorship.

---

## 6. JobHunter README handoff

Keep the existing product-first README. Add a concise development/contribution section near the top, after the opening product description and before deep feature detail.

Approved wording:

```markdown
## Development and contribution model

JobHunter is also an AI-assisted engineering project. Ali directs the product, evidence/authority boundaries, semantic-review rules, and acceptance/rejection decisions, and evaluates the resulting behavior and research. Substantial architecture, source, tests, debugging, and continuation have been produced with AI assistance. The repository's product capability is therefore kept separate from claims about Ali's independent FastAPI, SQLite/SQL, LLM-orchestration, or full-source implementation ownership.
```

Do not weaken the product story merely because development is AI-assisted.

---

## 7. Sentinel README handoff

Sentinel's first screen should become a research story before exposing the full stack.

Required first-screen order:

```text
plain-language problem
→ strongest current research/evaluation constraint
→ original Ali-involved era vs later AI-led R4 continuation
→ current Phase-8 boundary
→ then deep architecture
```

Approved contribution wording:

```markdown
## Project eras and contribution boundary

Sentinel has two important development eras. The original project was Ali's long-running AI-assisted learning/building work across Python, data preparation, repeated ML training, Linux, graph/agent experiments, and dataset-quality diagnosis. The later R4 continuation is substantially AI-led research under Ali's direction and should not be interpreted as independent ownership of the current ML/data, LangGraph, zkML, blockchain, or full-system implementation.

The strongest current R4 result is methodological rather than a new model-quality claim: the project repaired data/evaluation assumptions, found representation and supervision problems, and continues to withhold full retraining/promotion while the evidence needed for trustworthy evaluation remains incomplete.
```

The current README's older G7/"Phase 8 next" wording should be reconciled against the current `docs/handbook/16_current_status.md` before project-local publication, because current project evidence now places Phase 8 in progress with later accepted representation work.

---

## 8. Career repository public role

`motafegh/Career` is an operating system and audit trail, not a technical portfolio project.

Public README rules:

- explain what the repository is and its repository-boundary purpose;
- point to `CAREER_STATE.md` for live state instead of duplicating application/readiness status;
- do not advertise detailed blockers or stale review dates in the README;
- do not pin/feature this repository for employers by default.

---

## 9. Manual GitHub UI actions required

The current connected GitHub interface available to this Career session can edit repository files but does not expose repository creation, profile pinning, repository descriptions, or topic mutations.

Ali therefore needs to perform these UI-only actions after the repository-side copy is ready:

1. Create public repository `motafegh/motafegh` with `README.md` using section 2.
2. Set the descriptions/topics from section 3 on the three repositories.
3. Verify/pin the repositories in the section-4 order.

These manual actions are required before E2-P0 can be called fully closed.

---

## 10. E2 closure checklist

| Item | State |
|---|---|
| Career-owned approved profile copy | DONE |
| Career-owned repository metadata copy | DONE |
| Career-owned pin recommendation | DONE |
| Career README stale recruiter-facing status removed | PENDING until committed |
| UpgradePilot employer-facing first layer | PROJECT-LOCAL PENDING |
| JobHunter contribution boundary | PROJECT-LOCAL PENDING |
| Sentinel simplified/two-era first screen | PROJECT-LOCAL PENDING |
| `motafegh/motafegh` repository + profile README | MANUAL GITHUB UI PENDING |
| descriptions/topics | MANUAL GITHUB UI PENDING |
| pins verified/curated | MANUAL GITHUB UI PENDING |
| short final claim/materials check | PENDING AFTER ABOVE |

Do not activate the pre-authorized narrow application band until the minimum E2 first-screen/profile corrections are actually in place and Career runs the short activation check.
