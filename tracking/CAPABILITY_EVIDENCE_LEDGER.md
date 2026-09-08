# Capability Evidence Ledger

**Owner:** Ali Rajabi  
**Status:** Approved and controlling cross-project capability record  
**Last reviewed:** 2026-09-08 — early Day-60 A7 capability reassessment  
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
Depth: D2 — Guided application; strong current retention within UpgradePilot evidence contexts
Best evidence: UpgradePilot manual investigation, AegisLab evidence-boundary work, and 2026-08-18 delayed recall repeatedly distinguishing evidence for one proposition from stronger unsupported conclusions; Ali explicitly retained that unavailable/unresolved does not mean false, broken, unsafe, or dangerous
Assistance: Substantial AI teaching and correction; the 2026-08-18 assessment used delayed own-words recall before correction
Last demonstrated: 2026-08-18
Confidence: Medium-high within current UpgradePilot-style evidence reasoning; transfer outside related technical investigations remains untested
Transfer limit: Does not establish independent decision writing or implementation of the evidence machinery in unfamiliar domains
Next reassessment: Changed technical evidence set where Ali independently classifies what is established, unresolved, refuted, and still unproven before AI correction
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

### 8.6 AI-assisted project direction and technical critique

```text
Responsibility: Direct AI-assisted project work by challenging scope, architecture pressure, evidence strength, unnecessary complexity, and unsupported conclusions
Depth: D2 with provisional D3 signals for selected direction/critique responsibilities; not D3 technical implementation ownership
Best evidence: Repeated Career/UpgradePilot boundary and scope challenges; during the 2026-08 review period Ali challenged case-shaped implementation that appeared too narrow/hardcoded and pushed the project toward explicit architecture/horizon reasoning; during recent source learning he challenged whether revision/blob/byte provenance fields actually earned their complexity and required the AI to trace where they were used and what failure each protection addressed
Assistance: AI provides substantial architecture/source analysis and alternatives; Ali supplies the challenge, concern, acceptance/rejection pressure, and questions that materially redirect investigation
Last demonstrated: 2026-08-18
Confidence: Medium-high that this is a real recurring strength; lower for unfamiliar professional-team design contexts
Transfer limit: Critique/direction does not establish ability to implement the resulting architecture, own its tests, diagnose unfamiliar failures, or operate as an independent software architect
Next reassessment: One bounded technical responsibility where Ali states the design concern, predicts the failure/trade-off, influences the implementation, then verifies the source/tests/result rather than stopping at the design discussion
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
Responsibility: Reconstruct and explain the major evidence/trust responsibilities in the current public-PR investigation architecture
Depth: D2 — Guided conceptual understanding; strongest in evidence/claim boundaries; exact responsibility sequencing uneven; implementation ownership unestablished
Best evidence: 2026-08-18 delayed no-repository recall correctly reconstructed the product's non-safety/non-autonomy doctrine, PR identity/base-head orientation, crossed-release rationale, upstream authority principle, bounded LLM trust boundary, deterministic post-LLM validation, and multiple "what this does not prove" distinctions. Recall was weaker on the exact post-DependencyVersionChange branch split, conditional Target activation, exact positive CI proposition, and some dependency-analysis ambiguity handling
Assistance: Architecture and learning were substantially AI-assisted; the formal assessment intentionally required Ali to answer before corrections and preserved the inaccuracies rather than scoring immediate repetition
Last demonstrated: 2026-08-18
Confidence: Medium-high for the evidence-first mental model; Medium/low for exact orchestration sequencing and positive proposition ownership
Transfer limit: Does not prove blank-page implementation, source-level orchestration ownership, meaningful test design, current modification capability, broad debugging, or transfer to an unfamiliar application
Next reassessment: After the current real-case learning route reaches source/tests, require reduced-prompt end-to-end reconstruction plus one meaningful source/test change and failure diagnosis
```

### 8.9 PyPI release-identity implementation ownership

```text
Responsibility: Implement, validate, test, and diagnose exact PyPI package/version identity acquisition
Depth: D0 for Ali ownership; D1 conceptual exposure may exist
Best evidence: Active AI-assisted project implementation and later integrated project validation; no separate Ali ownership demonstration sufficient to raise the implementation depth was inspected in this Career review
Assistance: Substantive implementation and test generation were AI-produced or AI-assisted
Last demonstrated: No sufficient Ali implementation-ownership demonstration as of 2026-08-18
Confidence: High that project progress alone does not establish ownership
Transfer limit: No independent implementation, testing, debugging, or general PyPI/API ownership claim
Next reassessment: Project-local evidence where Ali explains trust/failure states, materially modifies behavior or a meaningful test, and diagnoses a representative changed/failing case with reduced assistance
```

### 8.10 Local HTTP/proxy failure recognition and diagnostic redirection

```text
Responsibility: Recognize a relevant transport/environment cause family during a local HTTP inference failure and redirect the investigation accordingly
Depth: D2 — Guided application with one meaningful independent diagnostic intervention; D3 not established
Best evidence: During the UpgradePilot local-inference proxy-contamination incident, Ali observed that the local model service was not receiving the expected request, recognized a familiar VPN/proxy/no-proxy failure pattern, stopped the AI's current debugging direction, and redirected investigation toward proxy inheritance; project evidence subsequently confirmed ambient proxy contamination as the relevant cause family
Assistance: Ali supplied the key diagnostic redirect from retained prior context; AI/project tooling performed substantial investigation, implementation, and verification of the final fix
Last demonstrated: 2026-08-04 to 2026-08-05 review period
Confidence: Medium for this familiar bounded failure pattern
Transfer limit: Does not establish general HTTP, proxy, networking, `requests`, environment-configuration, or unfamiliar runtime-debugging ownership; exact fix details were not fully retained during Career recall
Next reassessment: A changed or unfamiliar transport/runtime failure where Ali selects evidence and diagnosis steps with limited assistance and can explain the repaired mechanism after delay
```

### 8.11 Recent real-case dependency, lockfile, and CI concepts

```text
Responsibility: Explain selected real software objects and evidence distinctions used by the current UpgradePilot dependency-environment/CI work
Depth: D2 — Guided conceptual application at the demonstrated scope
Best evidence: On 2026-08-18, without opening notes, Ali explained Soup Sieve as a transitive documentation/tooling dependency through Beautiful Soup, described uv as a Python package/project manager and uv.lock as a universal lock whose package presence does not prove a selected CI environment contains/consumes that package, reconstructed CI workflow→job→step structure, and correctly distinguished static YAML declaration from actual successful runtime evidence
Assistance: Subjects were taught through the UpgradePilot real-case learning route; assessment answers were delayed own-words recall and received later precision corrections on Soup Sieve/Beautiful Soup wording, uv.lock semantics, and `run:` versus `uses:`
Last demonstrated: 2026-08-18
Confidence: Medium for the demonstrated concepts
Transfer limit: Does not establish independent uv-lock parsing, GitHub Actions implementation, dependency-graph analysis, environment-membership coding, or CI-consumption ownership
Next reassessment: Continue the real S001 route into actual source/functions/tests and require a changed-case prediction or focused modification
```

### 8.12 Historical Day-30 combined source/test/modification/debugging checkpoint

```text
Responsibility: Read and explain central current Python source, understand representative project tests, materially modify source/test behavior, and diagnose a current real failure
Depth: D0 — Not established at the 2026-08-18 Day-30 review
Best evidence: During direct assessment Ali stated that he could not name a current Python function/module he had personally read deeply enough to explain, had not inspected a representative current test, had not participated in a meaningful code/test modification with pre-change understanding, and had no new post-proxy debugging case where he formed/localized a failure hypothesis
Assistance: Not applicable as a positive ownership claim; current repository implementation/testing is substantially AI-assisted/AI-generated
Last demonstrated: Explicitly assessed 2026-08-18
Confidence: High for the Day-30 checkpoint
Transfer limit: Historical combined checkpoint only; later A7 assessment splits this bundle because some sub-responsibilities improved while modification/diagnosis did not
Next reassessment: Superseded for current interpretation by 8.13 and 8.14 below
```

### 8.13 Current UpgradePilot source-flow and representative-test reasoning

```text
Responsibility: Read and explain one bounded current UpgradePilot source-flow responsibility and reason correctly about representative tests and their proof limits
Depth: D2 — Guided application at the selected artifact-serviceability / target-composition scope
Best evidence: September-7 project evidence records Ali selecting a failure-containment behavior before mutation and completing a post-implementation ownership check on the actual investigation flow, including branch independence, candidate-versus-applicability distinction, test-double semantics, and what static target evidence does not prove. The fresh pre-A7 inspection also confirms the related target artifact-environment source and focused-test changes reached main after the earlier MEMORY snapshot.
Assistance: Substantial AI-generated implementation, tests, explanation, and review; Ali's evidence is in pre-change reasoning, bounded source/test interpretation, proof-limit explanation, and technical challenge rather than independent authorship
Last demonstrated: 2026-09-07
Confidence: Medium for the bounded current responsibility
Transfer limit: Does not establish broad Python/application ownership, independent test design, independent implementation of the current flow, or transfer to unfamiliar modules
Claim permitted: Ali can describe selected current source/test responsibilities at guided depth and explain important proof/uncertainty boundaries
Claim prohibited: Independent ownership of UpgradePilot implementation or its test architecture
Next reassessment: A changed current responsibility with less prompting plus an ownership-bearing modification and/or current failure diagnosis
```

### 8.14 Ownership-bearing source/test modification and current causal diagnosis

```text
Responsibility: Materially modify a current source/test responsibility with pre-change understanding and diagnose a real current failure through useful causal evidence with reduced assistance
Depth: D0 — Not yet established at the A7 Career threshold
Best evidence: Current project/source/test progress and Ali design challenges are real, but inspected evidence still does not establish a sufficiently ownership-bearing modification plus a current unfamiliar causal diagnosis attributable to Ali. Deferred executable proof also cannot be counted as a successful diagnostic/verification result.
Assistance: Current implementation/test work remains substantially AI-assisted/AI-generated
Last demonstrated: Insufficient positive evidence as of 2026-09-08
Confidence: High that this stronger ownership proposition remains unestablished
Transfer limit: Do not infer from commits under Ali's GitHub identity, green/AI-generated tests, source reading, or design approval
Next reassessment: One legitimate current modification and one real failure/diagnosis with reduced assistance, whether in the same responsibility or separate bounded cases
```

## 9. Capability-family baseline

| Family | Current Career interpretation | Main evidence source | Priority reassessment |
|---|---|---|---|
| Python application engineering | Bounded current source-flow understanding now D2 at selected scope; direct modification/transfer ownership not established | UpgradePilot | Ownership-bearing modification + changed case |
| Testing and debugging | Representative-test semantics now D2 at selected current scope; one older proxy diagnostic signal; current unfamiliar causal diagnosis remains unestablished | UpgradePilot, AegisLab | Real current failure diagnosis with reduced assistance |
| API/HTTP acquisition | Guided conceptual/current evidence; one narrow proxy/environment diagnostic signal; implementation ownership mixed | UpgradePilot | Live/controlled acquisition or transport change and failure handling with reduced help |
| Parsing, validation, provenance | Evidence/trust reasoning is a relative strength; implementation ownership unestablished | UpgradePilot | Explain and modify one trust-boundary path and its tests |
| Data modeling, persistence, SQL | D0 or highly provisional; repository use in JobHunter is not Ali evidence | Future bounded responsibility | Real schema, queries, changed case, and diagnosis |
| Packaging and configuration | Guided setup evidence; ownership unestablished | UpgradePilot | Clean setup, dependency/config change, and packaging failure diagnosis |
| Git/GitHub collaboration | Guided ordinary use; professional review/collaboration weak | Multiple repositories | Independent bounded branch/review/conflict case |
| Deterministic analysis/evaluation | Guided conceptual reasoning improving | UpgradePilot | Build/change one deterministic evaluator or baseline and analyze errors |
| ML experimentation | Historical broad exposure; current Sentinel R4 work is AI-full-implementation | Sentinel | Reassess only a bounded ML/evaluation responsibility when Career explicitly selects it |
| Grounded AI/LLM evaluation | Strong trust-boundary understanding; implementation/evaluation ownership unestablished | UpgradePilot, JobHunter portfolio evidence | Bounded semantic/evaluation responsibility with actual test/error analysis |
| Secure engineering | Guided concepts and selected trust boundaries | AegisLab, UpgradePilot | Implement and diagnose one secure input/config/permission responsibility |
| Docker/CI/operational reproducibility | Mixed exposure; ownership unestablished | Sentinel, UpgradePilot | Reproduce, modify, and diagnose a supported setup |
| Cloud/distributed/Kubernetes/MLOps/agents | Exposure varies; professional capability unestablished | Portfolio projects/future responsibilities | Evidence-led only when market/project need justifies it |
| Technical communication | Stronger delayed explanation and uncertainty disclosure; market-facing concision still needs E2/project-defense use | Career/UpgradePilot | Concise technical/nontechnical project defense for a real vacancy |
| AI-assisted technical critique / harness direction | Real recurring strength at D2 with provisional D3 signals in selected direction/challenge work | UpgradePilot/Career discussions | Carry one critique/harness decision through implementation/test/result verification and changed context |
| Professional collaboration | Transferable business experience; technical-team evidence unestablished | Family business, future work | Code review, issue communication, planning, and feedback in real collaboration |

## 10. Claims permitted after the 2026-09-08 A7 review

Career may say that Ali:

- has D2 guided capability in evidence/uncertainty/claim-boundary reasoning within current UpgradePilot-style contexts;
- has bounded D2 current source-flow and representative-test reasoning for a selected current UpgradePilot responsibility;
- can explain why static target/workflow evidence does not establish stronger runtime or wheel-compatibility conclusions;
- demonstrates a recurring strength in AI-assisted technical critique, anti-overengineering pressure, and harness/direction work, with provisional D3 signals for selected direction responsibilities;
- has one older bounded proxy/environment diagnostic-redirection case;
- is deliberately developing an anchored-hybrid Python/data/applied-AI profile while preserving explicit AI-assistance boundaries.

Career must state when relevant that:

- the stronger ownership proposition of meaningful current source/test modification plus current causal diagnosis remains unestablished;
- SQL/relational-data and professional Git/review evidence remain weak;
- JobHunter and current Sentinel implementation are AI-full-implementation portfolio/research assets, not automatic Ali capability evidence.

Career may not yet say that Ali:

- independently owns the UpgradePilot request-to-output implementation or test architecture;
- has broad D3 Python/application engineering capability;
- independently diagnoses the project's main unfamiliar failures;
- generally owns PyPI/API acquisition, HTTP/proxy debugging, packaging, SQL, data modeling, backend, security, CI, ML, cloud, or advanced systems;
- owns JobHunter FastAPI/SQLite/LLM implementation or current Sentinel R4 ML/data implementation merely because he directs the projects;
- is mid-level or senior.

Application readiness is governed by `CAREER_STATE.md` and the employability plan rather than inferred directly from one capability record.

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
