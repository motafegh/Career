# E2 GitHub Positioning Implementation Package

**Date:** 2026-09-08  
**Status:** ACTIVE / REPOSITORY-SIDE COPY COMPLETE / GITHUB UI ACTIONS PENDING  
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

This package is the Career-owned wording/claim source. Technical project repositories remain responsible for their own technical truth and later README maintenance.

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

## 5. UpgradePilot README result

Completed on 2026-09-08 in `motafegh/UpgradePilot`.

The README now includes an employer/reviewer layer before the detailed quickstart covering:

- current product behavior;
- differentiation from generic dependency automation / generic AI code review;
- a short inspectable evidence flow;
- Ali's actual contribution and AI-assistance boundary;
- current product/proof limitations.

Commit:

```text
35b1fa56b08d10aa6211e2a1e06931f426ab0bdc
```

Approved claim boundary remains:

```text
Ali directs and learns through the AI-assisted development of UpgradePilot, including product/evidence decisions, repeated challenge of scope and proof boundaries, selected pre-change design decisions, and bounded current source/test reasoning. The repository's substantive implementation and tests are heavily AI-assisted; the complete Python/test architecture is not presented as independently authored or independently owned by Ali.
```

---

## 6. JobHunter README result

Completed on 2026-09-08 in `motafegh/jobhunter`.

The product-first README is preserved and now includes a concise development/contribution boundary near the top.

Commit:

```text
68bbad7c501a673950e73d59aa16439c63dc81e7
```

Published wording:

```markdown
## Development and contribution model

JobHunter is also an AI-assisted engineering project. Ali directs the product, evidence/authority boundaries, semantic-review rules, and acceptance/rejection decisions, and evaluates the resulting behavior and research. Substantial architecture, source, tests, debugging, and continuation have been produced with AI assistance. The repository's product capability is therefore kept separate from claims about Ali's independent FastAPI, SQLite/SQL, LLM-orchestration, or full-source implementation ownership.
```

---

## 7. Sentinel README result

Completed on 2026-09-08 in `motafegh/sentinel-` after reconciling the public first screen against the canonical current-status owner.

The README now opens with:

```text
plain-language research problem
→ strongest current evidence/evaluation constraint
→ original Ali-involved era vs later AI-led R4 continuation
→ current Phase-8 boundary
→ then deep architecture
```

It also replaces the stale `Phase 8 next` framing with the current `Phase 8 IN_PROGRESS / G8 open` state and current R4 constraints.

Commit:

```text
b0c0e031b35785977a8be2c59cee3dff9f195d22
```

---

## 8. Career repository public role

Completed on 2026-09-08.

The Career README now:

- describes Career as an operating system rather than a technical portfolio project;
- delegates fast-changing truth to `CAREER_STATE.md`;
- removes stale duplicated employability/application text;
- keeps the three-project employer path explicit.

Commit:

```text
e6278978b80c3dbd6ced6e2badac9ae27d481829
```

---

## 9. Manual GitHub UI actions required

The connected GitHub interface available to this Career session can edit repository files but does not expose repository creation, profile pinning, repository descriptions, or topic mutations.

Ali therefore needs to perform only these remaining UI actions:

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
| Career README stale recruiter-facing status removed | DONE |
| UpgradePilot employer-facing first layer | DONE |
| JobHunter contribution boundary | DONE |
| Sentinel simplified/two-era first screen | DONE |
| `motafegh/motafegh` repository + profile README | MANUAL GITHUB UI PENDING |
| descriptions/topics | MANUAL GITHUB UI PENDING |
| pins verified/curated | MANUAL GITHUB UI PENDING |
| short final claim/materials check | PENDING AFTER ABOVE |

Do not activate the pre-authorized narrow application band until the remaining GitHub UI actions are in place and Career runs the short activation check.
