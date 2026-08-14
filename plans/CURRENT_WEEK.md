# Current Near-Term Personal Execution Plan

**Owner:** Ali Rajabi  
**Status:** Active Career execution aid  
**Period:** 2026-08-15 through 2026-08-21  
**Career authority:** [`../CAREER_STATE.md`](../CAREER_STATE.md) and [`CURRENT_CAREER_CYCLE.md`](CURRENT_CAREER_CYCLE.md)  
**Technical capability checkpoint:** [`2026-08-18_TECHNICAL_CAPABILITY_CHECKPOINT.md`](2026-08-18_TECHNICAL_CAPABILITY_CHECKPOINT.md)  
**Technical truth owner:** `motafegh/UpgradePilot` `MEMORY.md`, current plans, source, tests, ADRs/specifications, learning evidence, and working memory

## 1. Purpose

Use the final days before the 2026-08-18 Day-30 Career review to convert UpgradePilot's rapid recent progress into **selected retained understanding, source/test familiarity, and bounded ownership evidence** without trying to memorize the entire recent repository history or slowing legitimate project execution.

After the August-18 review, use the review result as the decision gate for the remainder of this week. Do not pre-authorize a new Career learning direction before that assessment.

This file remains a **Career execution and evidence plan**, not an UpgradePilot implementation plan. Career defines the capability/evidence outcomes to pursue. UpgradePilot alone controls exact technical continuation, architecture decisions, implementation, tests, project-local learning, and source changes.

## 2. Recalibration from actual UpgradePilot progress

The previous plan expected the A→C product-decision model to return to bounded implementation. That correction has already happened substantially.

By 2026-08-15, UpgradePilot has materially progressed through:

- implementation of the first mechanism-specific impact-candidate and candidate-applicability foundation;
- deterministic proposition/path/candidate composition with explicit evidence and path-model coverage;
- the first real discriminating-investigation selection → acquisition → observation → reevaluation loop;
- a materially different second mechanism: artifact serviceability / wheel compatibility;
- verified artifact-serviceability behavior, including a 397-test full active regression at one recorded checkpoint;
- a first bounded Target artifact-environment evidence slice from exact GitHub Actions workflow source;
- promotion of accepted A→B→C semantics into a canonical Product Decision Model specification;
- an evidence-earned cross-responsibility architecture gate because CI and Target independently consume overlapping GitHub Actions workflow structure;
- Phase-C transfer/adversarial pressure supporting the leading architecture direction with constraints;
- current live continuation into **Phase D — architecture decision classification and durable-owner selection**, before any refactor or new parser dependency/source migration.

The current project architecture candidate is approximately:

```text
RepositoryTextFile
→ bounded provider-specific GitHub Actions workflow-definition IR
→ separate CI interpretation
→ separate Target interpretation

runtime WorkflowRun / WorkflowJob / WorkflowStep
→ separate evidence family

possible later static↔runtime correlation
→ explicit bounded responsibility, not part of the base static IR
```

Career interpretation:

> The earlier conceptual/design-heavy period was not wasted: it produced consequential model corrections and was followed by real implementation. The current Career risk is now different. UpgradePilot is progressing through multiple mechanisms and architecture decisions faster than Ali can reasonably consolidate every concept, rejected option, and source change. The next objective is **selective ownership**, not total catch-up.

## 3. Operating rules for this week

### Rule A — do not turn repository history into a memorization burden

Ali does not need to retain every rejected alternative, working-memory finding, simulation case, or intermediate architectural formulation.

Prioritize three knowledge classes:

```text
1. CORE INVARIANTS
   retain strongly

2. CURRENT ACCEPTED/LEADING SYSTEM SHAPE
   understand operationally

3. HISTORICAL OPTION EXPLORATION
   repository remains the archive; recall only when needed
```

### Rule B — preserve architecture discipline, but prefer executable feedback for reversible decisions

Use deeper pre-implementation reasoning when a wrong decision could create high-cost semantic/ownership debt, especially:

- trust/evidence strength;
- domain/public contracts;
- cross-package ownership;
- shared abstractions;
- static-versus-runtime proof semantics.

For bounded/reversible implementation details, prefer:

```text
understand enough
→ predict
→ implement small slice
→ test
→ inspect reality
→ revise
```

Do not seek near-perfect certainty for low-cost reversible decisions.

### Rule C — every active UpgradePilot day should contain one ownership-bearing action

Examples:

- reconstruct a responsibility before rereading it;
- predict a behavior or test outcome;
- challenge an AI design/implementation decision and state why;
- explain a representative source function or contract;
- understand and influence a bounded source/test change;
- state the likely failure layer before AI diagnosis;
- inspect the resulting diff/tests rather than accepting only an AI summary;
- identify explicitly where understanding stops.

AI-heavy coding remains allowed. Manual typing volume is not the ownership metric.

### Rule D — the August-18 checkpoint remains frozen

Do **not** expand [`2026-08-18_TECHNICAL_CAPABILITY_CHECKPOINT.md`](2026-08-18_TECHNICAL_CAPABILITY_CHECKPOINT.md) to include every new UpgradePilot responsibility.

The B2/Step-7-era core remains the formal assessment baseline.

Recent implementation and architecture work is supplementary moving-frontier evidence. Strong understanding may improve the assessment; incomplete mastery of very recent work does not automatically count as failure.

## 4. Work pattern

Maintain the existing **24 focused-hour Green weekly ceiling**. It is not a quota.

For the three pre-review days, approximately **8–12 focused hours total** is a strong range if energy and normal life allow. Do not compensate for previous days by forcing hours.

A productive day can remain approximately four focused hours.

### Block A — laptop/desktop, about 45–75 minutes

Use for high-value consolidation:

- delayed reconstruction;
- actual source reading;
- representative test reading;
- syntax/mechanism repair;
- reconnecting one concept to its implementation.

Default: attempt recall/prediction first, then inspect source/notes.

### Block B — phone/outside, about 90–120 minutes

Use the phone as a work terminal for:

- conceptual reconstruction;
- current architecture reasoning;
- explaining a mechanism in your own words;
- comparing two responsibilities;
- challenge/prediction before implementation;
- reviewing outputs/failures;
- project-local AI teaching of one exact gap.

Do not force large multi-file source study into this block.

### Block C — laptop/desktop, about 60–120 minutes

Use for real UpgradePilot continuation:

- implementation when authorized by UpgradePilot;
- tests;
- terminal execution;
- diffs;
- debugging;
- verification;
- tracing what changed after AI work.

The project may remain in architecture decision classification during part of this period. If source changes are not yet technically authorized, do not invent coding exercises merely to satisfy Career.

## 5. Pre-review technical consolidation priorities

### Priority 1 — frozen Step-7 system remains the formal core

Use the technical checkpoint as the full rubric. Before August 18, make sure the older core can still be reconstructed coherently enough to explain:

```text
public PR / exact identity
→ dependency change
├── CI evidence
└── upstream/PyPI/release/changelog evidence
    → bounded semantic extraction
    → deterministic grounding
    → conditional target-Python evidence
    → bounded relevance
```

Emphasize the reasons behind the evidence boundaries, not memorized filenames.

### Priority 2 — own `impact/applicability.py` unusually well

This is the best current source-level learning target because it is small, central, deterministic, and directly implements concepts previously discussed abstractly.

Ali should understand:

```text
PropositionAssessment
ApplicabilityPathAssessment
CandidateApplicabilityAssessment

evaluate_applicability_path(...)
evaluate_candidate_applicability(...)
```

and be able to explain:

```text
one refuted necessary proposition
→ conjunctive path refuted

all necessary propositions established
→ path established

one complete established alternative path
→ candidate established applicable

all represented paths refuted
+ sufficient path-model coverage
→ established not applicable

all represented paths refuted
+ insufficient/unresolved path-model coverage
→ candidate remains unresolved
```

Source-level mechanisms worth recognizing here:

```text
Literal type aliases
frozen/slots dataclasses
tuple[...] typing
set comprehension
any(...)
all(...)
keyword-only argument after *
explicit ValueError contract checks
```

Do not expand this into studying every impact file line-by-line.

### Priority 3 — understand the first real investigation loop

Ali should explain the implemented distinction:

```text
candidate unresolved because target evidence has not yet been acquired
→ exact target declaration is discriminating
→ select bounded read-only acquisition
→ acquire/interpret
→ reevaluate candidate
```

versus:

```text
same acquisition already attempted and returned unavailable/problem evidence
→ do not blindly select the identical investigation again
```

The main learning target is why uncertainty can activate a specific investigation and why attempted/unavailable is different from not-yet-checked.

### Priority 4 — understand artifact serviceability at bounded depth

Ali should be able to explain these distinctions:

```text
package/interpreter support
!= compatible binary wheel availability

one published wheel tag removed
!= target lost all compatible wheels

sdist/source distribution exists
!= source build succeeds
```

Understand the current applicability comparison conceptually:

```text
old published wheel tags ∩ exact target-supported tags
versus
proposed published wheel tags ∩ exact target-supported tags
```

Do not require independent wheel-tag/environment reconstruction before August 18.

### Priority 5 — understand the Target artifact-environment proof boundary

Ali should understand what the first Target workflow slice can preserve:

- exact repository/revision/workflow/job provenance;
- literal runner where visible;
- literal setup-python version where visible;
- statically visible direct dependency-source installation;
- explicit unresolved/dynamic/unsupported limitations.

Most important distinctions:

```text
static workflow declaration
!= runtime execution
!= runtime success
!= runtime environment formation
!= behavior exercise

not_observed
!= established absent

runner + Python version
!= exact wheel compatibility tag set
```

The recent architecture pressure found that runtime-sounding `formation` wording can be stronger than the underlying static evidence. Ali should understand the problem; memorizing the eventual renamed contract is not required before it exists.

### Priority 6 — current architecture gate only at operational depth

By August 18, Ali should understand why the architecture checkpoint exists:

```text
CI and Target both parse overlapping GitHub Actions source structure
+
share some structural facts
+
have different domain questions/proof requirements
→ compare actual implementations before deciding what should be shared
```

Understand the three broad options:

```text
A — keep local parsers
B — shared bounded GitHub Actions static IR + separate CI/Target interpreters
C — broader combined static/runtime Actions model
```

Current evidence favors B with constraints.

Ali should be able to explain why:

```text
same syntax != same domain conclusion

raw source
!= normalized provider structure
!= CI interpretation
!= Target interpretation
!= runtime evidence
```

### Explicitly deferred architecture details

Do not make these August-18 mastery requirements:

- complete IR field taxonomy;
- PyYAML node-composition details;
- YAML alias/cycle internals;
- duplicate-key implementation;
- `SourceSpan` design details;
- matrix/reusable-workflow implementation semantics;
- static↔runtime step-correlation algorithm;
- exact ADR disposition;
- all Phase-D seams and historical findings.

If UpgradePilot needs one of these during actual continuation, learn it just in time.

## 6. Day-by-day plan before the review

### 2026-08-15 — re-anchor and select, do not catch up on everything

**Block A**

- reconstruct the Step-7 core from memory;
- read `impact/applicability.py` carefully;
- explain the two composition functions without relying on the learning note.

**Block B**

- explain in your own words the progression:

```text
A/B/C theory
→ first impact/applicability implementation
→ first discriminating-investigation loop
→ second artifact mechanism
→ target evidence
→ cross-responsibility architecture gate
```

- identify the three areas you currently feel least confident about.

**Block C**

- continue UpgradePilot exactly from its live `MEMORY.md` Phase-D architecture decision-classification state;
- before one material decision, state your own preferred direction/reason or at least the tradeoff you think matters;
- inspect what the AI records/changes afterward.

Ownership target: **one source explanation + one architecture/design challenge or prediction.**

### 2026-08-16 — implementation-backed consolidation

**Block A**

Choose one:

- first investigation loop; or
- artifact-serviceability evaluator.

Trace it from inputs → state changes → output → failure/unresolved boundaries.

Then inspect one representative test and explain:

```text
setup
→ action
→ assertion
→ protected behavior
→ what the test does NOT prove
```

**Block B**

Use one changed case rather than rereading notes. For example, reason about why a removed wheel tag does or does not matter to a target, or why static workflow installation text does not prove runtime exercise.

**Block C**

Normal project continuation. If Phase D/Phase E authorizes a source migration/refactor, use that real work as the ownership opportunity. If no source change is authorized, stay with legitimate architecture work rather than manufacturing code.

Ownership target: **one representative test responsibility + one changed-case reasoning example.**

### 2026-08-17 — pre-assessment consolidation, not cramming

Keep this day lighter if the preceding days were strong.

**Block A**

Without immediately opening notes:

1. reconstruct the frozen Step-7 flow;
2. explain impact/applicability composition;
3. explain the first investigation loop;
4. explain artifact serviceability;
5. explain the current CI/Target architecture problem.

Then check only the gaps.

**Block B**

Sample questions from the August-18 checkpoint. Do not attempt all questions.

Also prepare explicit calibration:

```text
What I can explain confidently:
What I can explain with some support:
What I have only been exposed to:
What I currently do not own:
```

**Block C**

Optional normal UpgradePilot continuation if energy is good. Otherwise use the time for Career review preparation: focused-hour evidence, project progress evidence, ownership examples, market/JobHunter status, and portfolio/application-readiness inputs.

Ownership target: **delayed reconstruction + explicit non-ownership boundary.**

## 7. 2026-08-18 — formal Day-30 Career review

The review must separately assess:

```text
1. UpgradePilot product/portfolio progress
2. Ali demonstrated capability and ownership
3. workload/sustainability
4. market evidence
5. portfolio/explanation readiness
6. application readiness
```

Do not infer Ali capability directly from repository sophistication or AI-generated code.

Use [`2026-08-18_TECHNICAL_CAPABILITY_CHECKPOINT.md`](2026-08-18_TECHNICAL_CAPABILITY_CHECKPOINT.md) as the frozen technical rubric and use recent A/B/C, artifact-serviceability, target-evidence, and architecture work only as supplementary evidence.

The review should result in explicit decisions rather than another indefinite "keep learning" state, including:

- what capability claims are currently defensible;
- the top remaining ownership/capability gaps;
- whether SQL or another common market gap now requires a bounded intervention;
- whether application/market calibration should activate or remain blocked;
- the next Career review/reassessment target.

## 8. 2026-08-19 through 2026-08-21 — conditional post-review execution

Do not predefine a detailed technical curriculum before the August-18 review.

After the review, execute its outcome under one of these broad shapes:

### If market/application calibration is activated

Protect UpgradePilot as the flagship while reserving bounded time for real market contact, role analysis, CV/GitHub positioning, or applications according to the review decision.

### If a small number of capability blockers are identified

Keep UpgradePilot as the primary vehicle where possible and target only the exact blocker(s), with reassessment dates rather than opening broad courses/projects.

### If the review finds ownership evidence insufficient despite strong repository progress

Shift some flagship time from further conceptual breadth toward selected source/test/modification/debugging repetition. Do not respond by abandoning UpgradePilot or starting a second flagship.

### If the review materially changes career direction or allocation

Update `CAREER_STATE.md`, the current cycle/portfolio records if required by governance, and then rewrite this active execution plan accordingly.

## 9. Evidence to preserve for the August-18 review

Keep this lightweight. Career does not need a productivity diary.

For active days, preserve enough information to recover:

```text
Date — focused time
Main allocation
One ownership-bearing action or observation
Energy: good | acceptable | overloaded
```

Before the review also collect:

- current UpgradePilot live state;
- representative implementation/test progress since August 5;
- at least two concrete Ali ownership examples;
- one debugging/challenge/pushback example;
- one representative test Ali can explain;
- one source responsibility Ali can explain beyond high-level architecture;
- explicit current non-ownership/gaps;
- JobHunter/market evidence status;
- current portfolio/CV/application-preparation status.

## 10. Success condition for this week

This week is successful if:

- UpgradePilot continues according to its own evidence-gated technical authority;
- Ali does not attempt to memorize the entire recent architecture/design history;
- the frozen Step-7 core is more coherent and retrievable;
- at least one current source responsibility becomes substantially better understood;
- recent A/B/C concepts are connected to actual implemented code/tests rather than remaining only conceptual exposure;
- the current architecture gate is understood at the level of problem, alternatives, evidence boundary, and leading direction without demanding fresh mastery of implementation details;
- Career has enough workload, capability, ownership, market, and portfolio evidence for a real August-18 decision;
- the post-review direction is selected from evidence rather than fear, repository size, or calendar pressure.

The operating principle is:

```text
DO NOT MASTER EVERYTHING THE PROJECT DISCUSSED.

RETAIN THE CORE.
OWN SELECTED REAL RESPONSIBILITIES.
LEARN NEW MATERIAL JUST IN TIME.
USE IMPLEMENTATION AND TESTS TO TURN EXPOSURE INTO CAPABILITY.
LET AUGUST 18 DECIDE THE NEXT CAREER EMPHASIS.
```
