# Capability Evidence Ledger

**Owner:** Ali Rajabi  
**Status:** Approved and controlling cross-project capability record  
**Last reviewed:** 2026-08-05 — retrospective Day-14 capability calibration  
**Responsibility:** Capability depth, evidence, assistance, recency, confidence, transfer limits, claim boundaries, and reassessment across all projects and work

## 1. Boundary

This ledger records Career-level capability conclusions.

It does not:

- control project sessions or implementation;
- update after every project event;
- replace project tests, working evidence, or technical state;
- convert repository progress into Ali capability automatically;
- mark broad technologies complete.

A record changes only during a Career review or explicit capability assessment.

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

## 5. Evidence expectations

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

## 6. Record formats

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

## 8. Current capability records

### 8.1 Public dependency-update evidence reasoning

```text
Responsibility: Interpret one public Dependabot pull-request evidence set and produce or challenge a bounded weak maintainer recommendation
Depth: D2 — Guided application
Best evidence: Completed manual UpgradePilot case, proportional-check selection, and changed/missing-evidence variant; canonical history preserved in UpgradePilot
Assistance: Substantial AI retrieval, explanation, structure, and wording; Ali participated in interpretation and decision challenge
Last demonstrated: 2026-07-19
Confidence: Medium for the single guided case
Transfer limit: One Python lockfile-oriented case; no independent repeated maintainer-review or general dependency-management claim
Next reassessment: A materially different real case with less prompting and an independently structured evidence/uncertainty explanation
```

### 8.2 Observation, inference, uncertainty, and claim boundaries

```text
Responsibility: Distinguish observed evidence, interpretation, missing evidence, uncertainty, and unsupported conclusions in a bounded technical investigation
Depth: D2 — Guided application
Best evidence: UpgradePilot manual investigation plus AegisLab evidence-boundary and failure-reasoning work
Assistance: Substantial AI prompting and correction
Last demonstrated: 2026-07-21
Confidence: Medium within guided repository/security evidence contexts
Transfer limit: Unfamiliar domains and low-prompt decision writing remain unassessed
Next reassessment: Independent classification of a changed technical evidence set and explanation of what success does not prove
```

### 8.3 Contract and method reasoning

```text
Responsibility: Distinguish raw input, boundary validation, trusted nested data, persistence/report roles, and participate in a bounded representation-method decision
Depth: D2 guided conceptual participation; implementation ownership unestablished
Best evidence: UpgradePilot contract-gap challenge, specification review, and method-decision participation
Assistance: Substantial AI analysis and drafting; Ali-directed challenge and approval
Last demonstrated: 2026-07-21
Confidence: Medium for conceptual distinctions; Low for independent implementation transfer
Transfer limit: Does not establish Pydantic, general data-contract, packaging, testing, or application-architecture ownership
Next reassessment: Explain current active contracts, make a changed-case modification, add or repair a test, and diagnose one failure with reduced prompting
```

### 8.4 Linux and controlled failure reasoning

```text
Responsibility: Operate a bounded Linux/network laboratory, inspect process/network evidence, and localize a controlled SSH-related failure
Depth: D2 — Guided application
Best evidence: AegisLab guided namespace/SSH lifecycle and failure investigation
Assistance: Substantial AI instruction and interpretation support
Last demonstrated: 2026-07-18 or earlier preserved AegisLab evidence
Confidence: Medium for the bounded guided case; freshness decreasing
Transfer limit: No independent Linux administration, networking, or security-engineering ownership claim
Next reassessment: A new bounded diagnostic case where Ali selects inspection steps and explains layer responsibility with less prompting
```

### 8.5 Git and repository operation

```text
Responsibility: Use repositories and basic Git/GitHub operations to preserve and inspect project work
Depth: D2 — Guided application, mixed sub-responsibilities
Best evidence: Repeated repository use, commits, a revert, basic workflow exposure, and project participation
Assistance: Mixed; many repository decisions and operations guided by AI
Last demonstrated: 2026-07-27
Confidence: Medium for ordinary guided use
Transfer limit: Independent branching strategy, pull-request review, conflict resolution, history repair, and team workflow remain weak or unassessed
Next reassessment: Independently perform and explain a bounded branch/commit/review workflow and diagnose one common Git problem
```

### 8.6 AI-assisted project direction

```text
Responsibility: Direct AI-assisted project and repository work by challenging scope, purpose, governance, and unsupported conclusions
Depth: D2 to provisional D3 for selected direction/challenge responsibilities
Best evidence: Repeated challenges that corrected Career/UpgradePilot boundaries, project purpose, source-learning design, excessive ceremony, and AI ownership assumptions
Assistance: AI-assisted analysis; Ali supplies the material challenge, intent, and approval
Last demonstrated: 2026-08-05
Confidence: Medium
Transfer limit: Direction and critique do not establish implementation, testing, technical design ownership, or professional-team transfer
Next reassessment: Independently frame a technical/product responsibility, compare alternatives, reject unsupported scope, and validate the resulting implementation/evidence
```

### 8.7 UpgradePilot installation, test, and live-run operation

```text
Responsibility: Set up and run the current UpgradePilot package, execute its deterministic suite, run one safe public case, and interpret the bounded result
Depth: D2 — Guided application
Best evidence: Recorded WSL2 Python 3.12 editable installation, deterministic test runs, and safe public evidence runs preserved in UpgradePilot
Assistance: Project commands, expected behavior, source, and many tests were substantially AI-provided; Ali executed and inspected selected results
Last demonstrated: 2026-08-05 or latest reviewed project-local operation
Confidence: Medium for guided setup/operation; lower for independent repair and transfer
Transfer limit: Successful commands alone do not establish test design, packaging ownership, independent setup repair, code ownership, or transfer to another application
Next reassessment: Reproduce a current supported path with less prompting, explain the request-to-output path, diagnose one setup/test failure, and justify the result boundaries
```

### 8.8 Current UpgradePilot investigation-architecture understanding

```text
Responsibility: Reconstruct and explain the major responsibilities and evidence branches in the current public-PR investigation architecture
Depth: D2 — Guided conceptual understanding; implementation ownership unestablished
Best evidence: On 2026-08-05, without consulting the repository or another AI, Ali reconstructed the evidence-first product mission and substantial parts of the PR/repository identity, changed-file/dependency, CI, PyPI/upstream, release-interval, and changelog path; he also correctly identified recent areas he had not yet learned rather than filling gaps by guessing
Assistance: The architecture and earlier learning were substantially AI-assisted; the 2026-08-05 assessment answer was delayed/reduced-context recall, followed by Career corrections on incomplete or incorrect details
Last demonstrated: 2026-08-05
Confidence: Medium for the high-level evidence architecture; Low for recent semantic/orchestration details and source-level transfer
Transfer limit: Does not prove blank-page implementation, current application-orchestration ownership, meaningful test design, source-level modification, broad debugging, or transfer to an unfamiliar project
Next reassessment: After project-local learning at an appropriate UpgradePilot boundary, reassess coherent reduced-prompt reconstruction together with meaningful modification/test/diagnosis evidence from the project repository
```

### 8.9 PyPI release-identity implementation ownership

```text
Responsibility: Implement, validate, test, and diagnose exact PyPI package/version identity acquisition
Depth: D0 for Ali ownership; D1 conceptual exposure may exist
Best evidence: Active AI-assisted project implementation and later integrated project validation; no separate Ali ownership demonstration sufficient to raise the implementation depth was inspected in this Career review
Assistance: Substantive implementation and test generation were AI-produced or AI-assisted
Last demonstrated: No sufficient Ali implementation-ownership demonstration as of 2026-08-05
Confidence: High that project progress alone does not establish ownership
Transfer limit: No independent implementation, testing, debugging, or general PyPI/API ownership claim
Next reassessment: Project-local evidence where Ali explains trust/failure states, materially modifies behavior or a meaningful test, and diagnoses a representative changed/failing case with reduced assistance
```

### 8.10 Local HTTP/proxy failure recognition and diagnostic redirection

```text
Responsibility: Recognize a relevant transport/environment cause family during a local HTTP inference failure and redirect the investigation accordingly
Depth: D2 — Guided application with one meaningful independent diagnostic intervention; D3 not established
Best evidence: During the recent UpgradePilot local-inference proxy-contamination incident, Ali observed that the local model service was not receiving the expected request, recognized a familiar VPN/proxy/no-proxy failure pattern, stopped the AI's current debugging direction, and redirected investigation toward proxy inheritance; project evidence subsequently confirmed ambient proxy contamination as the relevant cause family
Assistance: Ali supplied the key diagnostic redirect from retained prior context; AI/project tooling performed substantial investigation, implementation, and verification of the final fix
Last demonstrated: 2026-08-04 to 2026-08-05 review period
Confidence: Medium for this familiar bounded failure pattern
Transfer limit: Does not establish general HTTP, proxy, networking, `requests`, environment-configuration, or unfamiliar runtime-debugging ownership; exact fix details were not fully retained during Career recall
Next reassessment: A changed or unfamiliar transport/runtime failure where Ali selects evidence and diagnosis steps with limited assistance and can explain the repaired mechanism after delay
```

## 9. Capability-family baseline

| Family | Current Career interpretation | Main evidence source | Priority reassessment |
|---|---|---|---|
| Python application engineering | Mixed exposure; broad independent depth unestablished | UpgradePilot, Sentinel | Current source explanation, central modification, test, and failure diagnosis |
| Testing and debugging | Guided and mixed; one bounded diagnostic-redirection signal; broad ownership unestablished | UpgradePilot, AegisLab | Ali-selected changed/failing case, meaningful test responsibility, and diagnosis |
| API/HTTP acquisition | Guided current evidence; one narrow proxy/environment diagnostic signal; implementation ownership mixed | UpgradePilot | Live/controlled acquisition or transport change and failure handling with reduced help |
| Parsing, validation, provenance | Guided conceptual/current implementation exposure | UpgradePilot | Explain and modify one trust-boundary path and tests |
| Data modeling, persistence, SQL | D0 or highly provisional | Prior projects, future UpgradePilot | Real schema, queries, changed case, and diagnosis |
| Packaging and configuration | Guided setup evidence; ownership unestablished | UpgradePilot | Clean setup, dependency/config change, and packaging failure diagnosis |
| Git/GitHub collaboration | Guided use | Multiple repositories | Independent bounded branch/review/conflict case |
| Deterministic analysis/evaluation | Introduced/guided | UpgradePilot | Build or change a baseline and analyze errors |
| ML experimentation | Broad exposure, weak independent ownership | Sentinel | Reproducible baseline/model/evaluation with defensible truth and reduced help |
| Grounded AI/LLM evaluation | Current project exposure and introduced trust-boundary concepts; ownership unestablished | UpgradePilot, prior AI-assisted work | Bounded project-local semantic/evaluation responsibility with unsupported-claim analysis |
| Secure engineering | Guided concepts and selected trust boundaries | AegisLab, UpgradePilot | Implement and diagnose one secure input/config/permission responsibility |
| Docker/CI/operational reproducibility | Mixed exposure; ownership unestablished | Sentinel, UpgradePilot | Reproduce, modify, and diagnose a supported setup |
| Cloud/distributed/Kubernetes/MLOps/agents | Exposure varies; professional capability unestablished | Historical projects/future pilots | Evidence-led A1/A2 records only when admitted |
| Technical communication | Strong interest; improved project-architecture explanation; formal professional evidence incomplete | Project explanations, Career review | Concise audience-specific project explanation and review response |
| Professional collaboration | Transferable business experience; technical-team evidence unestablished | Family business, future work | Code review, issue communication, planning, and feedback in real collaboration |

## 10. Claims permitted after the 2026-08-05 review

Career may say that Ali:

- has narrow guided experience interpreting public dependency-update evidence and observation/inference boundaries;
- has run and interpreted bounded UpgradePilot test/live-evidence paths with substantial assistance;
- now has a materially stronger retained conceptual model of UpgradePilot's major evidence architecture, demonstrated through reduced-context reconstruction;
- demonstrated one bounded instance of using retained technical context to interrupt and redirect AI debugging toward the relevant runtime cause family;
- has strong AI-assisted project-direction and scope-challenge participation;
- is deliberately building evidence toward Python/data/AI engineering rather than claiming current mastery.

Career may not yet say that Ali:

- independently owns the UpgradePilot request-to-output implementation or current semantic/orchestration implementation;
- independently designs the project's meaningful tests or diagnoses its main unfamiliar failures;
- generally owns PyPI/API acquisition, HTTP/proxy debugging, packaging, SQL, data modeling, backend, security, CI, ML, or advanced systems;
- has broad D3 Python/application engineering capability from the current evidence;
- is broadly job-ready for every target role;
- is mid-level or senior.

## 11. Review workflow

When a capability review is requested:

1. define the role, claim, or decision;
2. select specific responsibilities;
3. inspect relevant current evidence;
4. verify actual behavior rather than summaries;
5. identify Ali's personal action and assistance;
6. choose the appropriate depth;
7. record confidence and transfer limit;
8. state permitted and prohibited claims where material;
9. define the next reassessment;
10. update Career state, portfolio, or market records only when the conclusion changes them.

## 12. Maintenance

Change model sections only when assessment rules change. Update capability records only during an explicit Career review or capability assessment.
