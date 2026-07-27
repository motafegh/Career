# Capability Evidence Ledger

**Owner:** Ali Rajabi  
**Status:** Approved and controlling cross-project capability record  
**Last reviewed:** 2026-07-27  
**Responsibility:** Capability depth, evidence, assistance, recency, confidence, transfer limits, claim boundaries, and reassessment across all projects and work

## 1. Boundary

This ledger records Career-level capability conclusions.

It does not:

- control project sessions or implementation;
- update after every project event;
- replace project tests, working evidence, or technical state;
- convert repository progress into Ali capability automatically;
- mark broad technologies complete.

A capability record is added or changed only during a Career review or explicit capability assessment.

## 2. Assessment principles

1. Assess a specific responsibility, not a broad topic.
2. Record what Ali personally demonstrated.
3. Separate exposure, guided application, independent bounded application, technical ownership, and advanced independent capability.
4. Record AI and human assistance honestly.
5. Record date, recency, confidence, and transfer limit.
6. Require changed-case, failure, delayed, and reduced-prompt evidence when the claimed depth needs them.
7. Do not average mixed responsibilities into an optimistic broad score.
8. Project progress and product maturity are separate from capability.
9. A failed task may reveal diagnostic capability or a precise gap.
10. Stale or context-specific evidence cannot support an unrestricted current claim.

## 3. Depth model

| Depth | Controlled meaning |
|---|---|
| **D0 — Unassessed** | Reliable ability has not been established. Exposure, discussion, or AI-generated work is insufficient. |
| **D1 — Introduced** | Ali recognizes the responsibility, practical purpose, main boundary, and relationship to a real system after teaching. |
| **D2 — Guided application** | Ali performs a bounded real or representative task with substantial explanation, examples, prompts, or correction and interprets the evidence correctly. |
| **D3 — Independent bounded application** | Ali performs a representative bounded responsibility with limited assistance, selects meaningful actions, handles a changed case, and diagnoses a common relevant failure. |
| **D4 — Technical ownership** | Ali can design or challenge, implement or materially modify, test, diagnose unfamiliar failures, explain trade-offs and system effects, and reproduce the responsibility with low assistance across relevant contexts. |
| **D5 — Advanced independent capability** | Ali repeatedly designs, operates, diagnoses, and evolves the responsibility across materially different contexts and substantial trade-offs with low assistance. |

D5 is not required for the current career cycle. A narrow D2 or D3 may be the correct result for many responsibilities.

## 4. Assistance labels

- **AI-generated** — AI produced the substantive artifact, implementation, analysis, or decision structure.
- **AI-assisted** — Ali performed meaningful work with substantial AI explanation, generation, correction, or repair.
- **Ali-directed** — Ali materially shaped the problem, constraints, approach, or decision.
- **Ali-verified** — Ali directly inspected checks or evidence, interpreted important output, and stated proof and limits correctly.
- **Ali-owned** — evidence supports explanation, modification, testing, diagnosis, and reduced-prompt reproduction at the stated scope.

Several labels may apply to different parts of one responsibility. Participation labels do not replace D-level evidence.

## 5. Evidence expectations by depth

### D1

Normally require:

- own-words practical meaning;
- relationship to a real project or professional responsibility;
- one important boundary, limitation, or failure distinction.

### D2

Normally require:

- guided real or representative application;
- correct interpretation of actual output or evidence;
- explicit assistance;
- one bounded check, modification, query, test, or decision where applicable;
- a narrow transfer limit.

### D3

Normally require:

- representative bounded case;
- changed case or variant;
- meaningful action, test, or query selected with limited prompting;
- relevant failure diagnosis or repair;
- ownership-bearing modification;
- delayed reconstruction or recall where useful;
- explicit transfer limit.

One immediate guided success cannot establish D3.

### D4

Normally require:

- repeated evidence across materially different cases or sessions;
- design or challenge participation;
- implementation and test ownership;
- unfamiliar failure diagnosis;
- system-wide trade-off explanation;
- low-assistance reproduction;
- explicit limitations.

### D5

Require sustained independent performance across varied contexts, unfamiliar failures, consequential trade-offs, and operational effects.

## 6. Record format

### Lean record — default

```text
Responsibility:
Depth:
Best evidence:
Assistance:
Last demonstrated:
Confidence:
Transfer limit:
Next reassessment:
```

### Extended record — use only when justified

Use for central capabilities, D3+ claims, disputed assessment, mixed ownership, portfolio claims, or significant role-readiness decisions.

Additional fields may include:

```text
Context:
Ownership dimensions:
Changed-case evidence:
Failure evidence:
Delayed evidence:
Breadth:
Freshness:
Claim permitted:
Claim prohibited:
Reassessment trigger:
```

## 7. Performative-check prohibition

The following alone cannot establish D3, D4, D5, or ownership:

- repeating an explanation immediately after AI;
- typing an AI-provided change;
- approving an AI-selected design;
- running a command successfully;
- passing AI-generated tests;
- reading code and agreeing with it;
- producing one guided artifact;
- recognizing terminology;
- repository sophistication;
- project completion.

## 8. Current retained capability records

These are conservative Career conclusions migrated from prior reviews. They do not reflect every later UpgradePilot event until the first refounded Career review is completed.

### 8.1 Public dependency-update evidence reasoning

```text
Responsibility: Interpret one public Dependabot pull-request evidence set and produce or challenge a bounded weak maintainer recommendation
Depth: D2 — Guided application
Best evidence: Completed manual UpgradePilot case and changed/missing-evidence variant; canonical history preserved in UpgradePilot
Assistance: Substantial AI retrieval, explanation, structure, and wording; Ali participated in evidence interpretation and decision challenge
Last demonstrated: 2026-07-19
Confidence: Medium for the single guided case
Transfer limit: One Python lockfile-oriented case; does not establish independent repeated maintainer review or general dependency-management competence
Next reassessment: A materially different real case with less prompting and an independently structured evidence/uncertainty explanation
```

### 8.2 Observation, inference, uncertainty, and claim boundaries

```text
Responsibility: Distinguish observed evidence, interpretation, missing evidence, uncertainty, and unsupported conclusions in a bounded technical investigation
Depth: D2 — Guided application
Best evidence: UpgradePilot manual investigation plus prior AegisLab evidence-boundary and failure-reasoning work
Assistance: Substantial AI prompting and correction
Last demonstrated: 2026-07-21
Confidence: Medium within guided repository/security evidence contexts
Transfer limit: Transfer to unfamiliar domains and low-prompt decision writing remains unassessed
Next reassessment: Independent classification of a changed technical evidence set and explanation of what success does not prove
```

### 8.3 Contract and method reasoning

```text
Responsibility: Distinguish raw input, boundary validation, trusted nested data, persistence/report roles, and participate in a bounded representation-method decision
Depth: D2 guided conceptual participation; implementation depth previously D1/unassessed
Best evidence: UpgradePilot contract-gap challenge, specification review, and method-decision participation
Assistance: Substantial AI analysis and drafting; Ali-directed challenge and approval
Last demonstrated: 2026-07-21
Confidence: Medium for the conceptual distinctions; Low for independent implementation transfer
Transfer limit: Does not establish Pydantic, general data-contract, packaging, testing, or application-architecture ownership
Next reassessment: Inspect current active implementation, explain the contract path, make a changed-case modification, add or repair a test, and diagnose one failure with reduced prompting
```

### 8.4 Linux and controlled failure reasoning

```text
Responsibility: Operate a bounded Linux/network laboratory, inspect process/network evidence, and localize a controlled SSH-related failure
Depth: D2 — Guided application
Best evidence: AegisLab guided namespace/SSH lifecycle and failure investigation
Assistance: Substantial AI instruction and interpretation support
Last demonstrated: 2026-07-18 or earlier preserved AegisLab evidence
Confidence: Medium for the bounded guided case; freshness decreasing
Transfer limit: Does not establish independent Linux administration, networking, or security-engineering ownership
Next reassessment: A new bounded diagnostic case requiring Ali to select inspection steps and explain layer responsibility with less prompting
```

### 8.5 Git and repository operation

```text
Responsibility: Use repositories and basic Git/GitHub operations to preserve and inspect project work
Depth: D2 — Guided application, mixed sub-responsibilities
Best evidence: Repeated repository use, commits, a revert, basic workflow exposure, and project participation
Assistance: Mixed; many repository decisions and operations guided by AI
Last demonstrated: 2026-07-27
Confidence: Medium for ordinary guided use
Transfer limit: Independent branching strategy, pull-request review, conflict resolution, history repair, and team workflow remain unassessed or weak
Next reassessment: Ali independently performs and explains a bounded branch/commit/review workflow and diagnoses one common Git problem
```

### 8.6 AI-assisted project direction

```text
Responsibility: Direct AI-assisted project and repository work by challenging scope, purpose, governance, and unsupported conclusions
Depth: D2 to provisional D3 for selected direction/challenge responsibilities
Best evidence: Repeated challenges that corrected Career/UpgradePilot boundaries, project purpose, source-learning design, excessive ceremony, and AI ownership assumptions
Assistance: AI-assisted analysis; Ali provides the material challenge, intent, and approval
Last demonstrated: 2026-07-27
Confidence: Medium
Transfer limit: Direction and critique do not establish implementation, testing, or technical design ownership; low-assistance transfer to a professional team is unassessed
Next reassessment: Ali independently frames a technical/product responsibility, compares alternatives, rejects unsupported scope, and validates the resulting implementation/evidence
```

## 9. Capability-family baseline

The table below prevents unassessed areas from being mistaken for completed capability. It is not a broad scorecard.

| Family | Current Career interpretation | Main evidence source | Priority reassessment |
|---|---|---|---|
| Python application engineering | Mixed exposure; broad independent depth unestablished | UpgradePilot, Sentinel | Active source explanation, modification, test, and failure diagnosis |
| Testing and debugging | Guided and mixed; ownership unestablished | UpgradePilot, AegisLab | Ali-selected changed/failing test and diagnosis |
| API/HTTP acquisition | Guided current evidence | UpgradePilot | Live/controlled acquisition change and failure handling with reduced help |
| Parsing, validation, provenance | Guided conceptual/current implementation exposure | UpgradePilot | Explain and modify one trust-boundary path and tests |
| Data modeling, persistence, SQL | D0 or highly provisional | Prior projects, future UpgradePilot | Real schema, queries, changed case, and diagnosis |
| Packaging and configuration | Introduced/guided; independent ownership unestablished | UpgradePilot | Editable install, dependency/config change, packaging failure diagnosis |
| Git/GitHub collaboration | Guided use | Multiple repositories | Independent bounded branch/review/conflict case |
| Deterministic analysis/evaluation | Introduced/guided | UpgradePilot | Build/change baseline and analyze errors |
| ML experimentation | Broad exposure, weak independent ownership | Sentinel | Reproducible baseline/model/evaluation with defensible truth and reduced help |
| Grounded AI/LLM evaluation | Exposure; capability unestablished | Prior AI-assisted work | Bounded comparison with unsupported-claim evaluation |
| Secure engineering | Guided concepts and selected boundaries | AegisLab, UpgradePilot | Implement and diagnose one secure input/config/permission responsibility |
| Docker/CI/operational reproducibility | Mixed exposure; ownership unestablished | Sentinel, UpgradePilot | Reproduce, modify, and diagnose a real supported setup |
| Cloud/distributed/Kubernetes/MLOps/agents | Exposure varies; professional capability unestablished | Historical projects/future pilots | Evidence-led A1/A2 records only when admitted |
| Technical communication | Strong interest; formal professional evidence incomplete | Project explanations | Concise audience-specific project explanation and review response |
| Professional collaboration | Transferable business experience; technical-team evidence unestablished | Family business, future work | Code review, issue communication, planning, and feedback in real collaboration |

## 10. Claim rules

- A broad family such as Python, ML, security, or data engineering cannot receive one undifferentiated depth.
- A narrow D3 does not imply broad job independence.
- High confidence does not raise the depth.
- Current project progress may justify reassessment but does not update a record automatically.
- A skill can transfer partially while requiring renewed assistance in an unfamiliar context.
- Stale evidence must be refreshed before strong current claims.
- Advanced A-level exposure records and D-level capability records must remain distinct.

## 11. Career review workflow

When a capability review is requested:

1. define the role, claim, or decision being evaluated;
2. select specific responsibilities;
3. inspect only relevant current project, work, or market evidence;
4. verify actual behavior rather than relying on summaries;
5. identify Ali's personal action and assistance;
6. choose the appropriate depth;
7. record confidence and transfer limit;
8. state the claim permitted and prohibited where material;
9. define the next reassessment;
10. update `CAREER_STATE.md`, portfolio, or market records only when the conclusion changes them.

## 12. Maintenance

Change the model sections only when assessment rules change. Update capability records only during an explicit Career review or capability assessment.
