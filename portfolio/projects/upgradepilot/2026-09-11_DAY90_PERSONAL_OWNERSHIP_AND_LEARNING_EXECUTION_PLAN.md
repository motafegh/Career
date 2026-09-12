# UpgradePilot — Day-90 Personal Ownership and Learning Plan

**Date:** 2026-09-11  
**Horizon:** 2026-09-11 through 2026-10-17  
**Owner:** Ali Rajabi / Career  
**Status:** Active Career-level personal-outcome plan; technical continuation intentionally delegated to UpgradePilot  
**Technical authority:** `motafegh/UpgradePilot` root governance, `MEMORY.md`, selected project plan/working memory, source/tests, and project-local Learning-by-Doing system  
**Career authority:** `../../../CAREER_STATE.md`, `../../../plans/CURRENT_CAREER_CYCLE.md`, and this project's `CAREER_RECORD.md`

## 1. Purpose

Use UpgradePilot as Ali's sole primary capability-building flagship for the remainder of the current Career cycle while converting repository sophistication into stronger **personal engineering ownership**.

This plan answers:

> What should Ali personally become better able to understand, verify, modify, diagnose, transfer, and explain through legitimate UpgradePilot work before the Day-90 Career review?

It does **not** own UpgradePilot's exact technical continuation, implementation order, source/test TODO, proof debt, active phase, or next slice.

Use the separation:

```text
Career plan
→ personal outcomes / depth / evidence opportunities / allocation / stop lines

UpgradePilot
→ exact current responsibility
→ learning / implementation / source / tests / commands / proof
→ technical next slice
```

Every project session must begin from UpgradePilot's **current** project-local owners. Do not recover technical continuation from this Career plan.

---

## 2. Day-90 target

By 2026-10-17, UpgradePilot should have helped Ali move from broad AI-assisted exposure toward a smaller set of **defensible current engineering responsibilities**.

A strong cycle result is:

```text
several current source/test responsibilities genuinely understood
+ representative tests/evaluations Ali can reason through
+ at least one legitimate ownership-bearing modification if real project work creates the opportunity
+ at least one credible current causal-diagnosis case if a real failure occurs
+ changed-context transfer beyond memorized examples
+ concise technical explanation of UpgradePilot at multiple depths
+ continued strong AI-agent direction with explicit verification/accountability
```

These are directional evidence targets, not quotas. Do not manufacture changes, failures, or exercises merely to satisfy this list.

The AI-era resilience lens is:

> **Use AI aggressively for execution while increasing Ali's ownership of intent, technical mental model, acceptance criteria, verification, diagnosis, meaningful correction, transfer, risk and explanation.**

This does not replace technical depth with management-only thinking.

---

## 3. Session-start rule

At the start of each UpgradePilot session:

1. read UpgradePilot's current root governance and `MEMORY.md`;
2. follow the project-local owner selected there;
3. identify the one current engineering responsibility Ali should personally understand better;
4. decide the personal outcome for the session without changing the project's technical route from Career.

Career may read through project state to make Ali's plan usable, but volatile project continuation must remain project-local and must not be copied back into this file.

---

## 4. Ali's ownership loop for substantive slices

UpgradePilot's own Learning-by-Doing procedure remains controlling. Career adds only this personal ownership lens.

### Before consequential work

Ali should be able to state proportionately:

- what responsibility is being changed, investigated, or proved;
- where its important input/evidence comes from;
- what output/state matters;
- the main failure, uncertainty, or trust boundary;
- what useful proof would look like;
- one stronger claim or non-goal that is not earned.

Do not require full implementation knowledge before work begins.

### During work

AI may write substantial or most code.

Ali should engage materially when work contains:

- consequential behavior or contract choices;
- important data/state representation;
- new failure/uncertainty semantics;
- tests/evaluations that establish a product claim;
- security/trust/provenance boundaries;
- potentially unnecessary abstractions/frameworks;
- meaningful implementation alternatives.

Manual typing is not the ownership metric.

### After work

For the selected responsibility, Ali should increasingly be able to answer:

```text
What enters this responsibility?
What important types/states exist?
What branches or transformations matter?
What leaves it?
What does the representative test/evaluation establish?
What does it not establish?
What can fail or remain unresolved?
Why is this responsibility placed here?
```

For consequential slices, also ask:

> If implementation became nearly free, what engineering responsibility would still be mine, and what technical understanding would I need to verify, diagnose, modify, transfer and defend it?

The answer must include technical substrate, not only review/management language.

### Transfer

After important learning, use one changed-context question when useful:

- What changes if the input is missing instead of malformed?
- What changes if evidence conflicts instead of being unavailable?
- Which test would fail if this invariant disappeared?
- Would the same design work for a nearby but different case?
- What evidence would justify a stronger action or claim?

Then distinguish:

```text
transferable engineering responsibility
vs
UpgradePilot-specific supporting/domain knowledge
```

Do not create ceremony around every small function or repetitive child task.

---

## 5. What Ali should become strong in through UpgradePilot

### 5.1 Python / software engineering

Target: increasingly strong working depth in responsibilities such as:

- tracing control/data flow across modules;
- functions/classes/dataclasses/types and their practical contracts;
- interfaces and responsibility boundaries;
- explicit state and error/failure handling;
- reading and modifying unfamiliar relevant code;
- understanding why a representation or abstraction exists;
- spotting unnecessary or case-shaped implementation.

### 5.2 Testing / evaluation / proof reasoning

Target: strong working depth in:

- fixture/input → action → assertion;
- what a test proves and does not prove;
- semantic faithfulness of test doubles/fixtures;
- positive, negative, missing, conflicting and changed cases;
- regression reasoning;
- acceptance criteria and oracle quality;
- executable proof versus static/documented claims.

### 5.3 Debugging / causal diagnosis

Target: stronger responsibility for:

```text
symptom
→ plausible cause families
→ evidence selection
→ boundary localization
→ repair choice
→ verification
```

Use real failures when they occur. Do not inject fake bugs for Career evidence.

### 5.4 External systems / data / evidence

Target: practical depth in:

- API/external-source boundaries;
- identity/revision/provenance;
- validation and typed states;
- missing versus negative versus conflicting evidence;
- trust boundaries;
- composition of evidence from independent sources;
- retries/errors/timeouts only where current project work legitimately requires them.

### 5.5 System design judgment

Target: stronger judgment about:

- responsibility placement;
- module/layer boundaries;
- when abstraction is earned;
- deterministic versus model authority;
- preserving uncertainty;
- avoiding hard-coded special cases;
- avoiding unnecessary framework/infrastructure expansion.

### 5.6 AI-agent engineering as a differentiator

Continue improving:

- repository/context selection;
- decomposition and scope control;
- agent/harness instructions;
- evidence demands and acceptance checks;
- review of generated source/tests;
- overengineering detection;
- context/memory/state design;
- human checkpoints and escalation;
- accountability for the final technical claim.

This is not reducible to prompting skill and does not replace the technical anchors above.

---

## 6. What should remain working-depth or deferred

UpgradePilot-specific details such as dependency-update mechanics, PyPI/package metadata, CI-consumption details, artifact serviceability, support-drop reasoning, and maintainer-action semantics are primarily the **domain vehicle** for learning engineering. Learn them deeply enough to understand and defend the project, not as separate career specializations.

Do not reopen or pursue these merely for breadth unless the project legitimately requires them:

- LangGraph/LangChain internals;
- generic multi-agent architecture;
- broad cloud/Kubernetes infrastructure;
- advanced Python metaprogramming/type-theory rabbit holes;
- every GitHub/PyPI API detail;
- every UpgradePilot module or historical plan;
- SQL/persistence machinery inserted only for résumé keywords;
- new frameworks/abstractions without product pressure.

---

## 7. Evidence opportunities to use when they naturally occur

### Ownership-bearing modification

High-value shape:

```text
Ali understands pre-change responsibility
→ real project need requires change
→ Ali predicts/helps decide intended behavior
→ AI may implement substantial code
→ Ali inspects source/tests/result
→ Ali explains why it is correct and what remains limited
```

### Real causal diagnosis

When a real failure appears, high-value evidence includes Ali selecting a useful cause family, inspection step, or boundary that materially advances diagnosis.

### Changed-context transfer

After learning one responsibility, use a nearby changed case to test whether the mental model transfers.

### Technical explanation

Periodically practice explaining selected responsibilities through:

- concise architecture/data flow;
- one representative test/evaluation;
- one failure/uncertainty case;
- one design trade-off;
- transferable responsibility;
- accurate AI-assistance boundary.

Career should preserve evidence only when the resulting event is material enough to change a capability/portfolio conclusion.

---

## 8. Remaining-cycle Career expectations

### Through the September checkpoint

- keep UpgradePilot dominant;
- continue the project-owned route;
- convert current legitimate work into stronger source/test/proof understanding;
- close remaining E2 Career work in parallel without displacing the flagship;
- return to Career if project evidence materially changes an ownership conclusion.

### Late September

- continue legitimate project work and increasingly use real modification/failure opportunities for ownership;
- begin/continue the pre-authorized narrow application-calibration lane once the live Career gate clears;
- keep SQL/Git work bounded and secondary.

### Early October

- consolidate transferable engineering depth;
- use classified application/interview evidence to prioritize only high-value gaps;
- strengthen employer-defensible project explanation;
- avoid new architecture/framework expansion for its own sake.

### Final Day-90 window

Consolidate and assess rather than expand.

Ali should be able to present:

1. a 30-second user/problem/product explanation;
2. a 2-minute evidence-flow and Ali-versus-AI explanation;
3. a deeper technical discussion of selected responsibilities, tests/evaluations, design trade-offs, proof limits, changed-context reasoning, and any legitimate modification/diagnosis evidence that occurred.

Exact technical work inside each period remains UpgradePilot-owned and may change without requiring edits to this plan.

---

## 9. Capacity and parallel Career work

Career's Green ceiling remains up to **24 focused hours/week**, not a quota.

The controlling cycle allocation is approximately:

```text
75–85%  UpgradePilot / flagship technical responsibility
15–25%  Career-owned positioning / applications / SQL / Git / market work combined
```

Use the current Career state/directive for exact macro priorities in the non-flagship lane.

Applications should proceed in parallel once their approved gate clears; do not wait for UpgradePilot to finish. SQL/Git should remain bounded role-widening work rather than distort UpgradePilot's product route.

---

## 10. Stop lines

Do not:

- try to master the whole repository;
- manually rewrite AI-generated code merely to prove effort;
- count repository progress as Ali capability automatically;
- manufacture bugs or arbitrary modifications;
- turn AI-era reflection into management-only learning or repetitive ceremony;
- force generic transfer lessons from every implementation detail;
- force SQL/cloud/frameworks into UpgradePilot for résumé breadth;
- reopen deferred frameworks without real project justification;
- spend days rereading historical plans when current project owners are sufficient;
- let documentation/governance replace real source/test/proof work;
- wait until UpgradePilot is finished before applying for jobs;
- let applications consume the flagship learning route;
- pursue unsupported mid/senior claims;
- copy UpgradePilot's volatile technical next action into Career.

---

## 11. Day-90 evidence review questions

At the 2026-10-17 Career review, ask:

1. Which current UpgradePilot responsibilities can Ali trace and explain without heavy prompting?
2. Which representative tests/evaluations can he interpret correctly, including proof limits?
3. Did a legitimate ownership-bearing modification occur? What was Ali's responsibility?
4. Did a real current failure diagnosis occur? What causal contribution was Ali's?
5. Can Ali transfer reasoning to changed cases and distinguish transferable responsibility from domain detail?
6. Has Ali improved at stating acceptance/non-goal/claim boundaries before consequential work?
7. Has AI-agent direction become more technically accountable rather than merely more elaborate?
8. Can Ali defend UpgradePilot clearly to an employer without overclaiming authorship?
9. Which gaps remain employment-relevant after classified market feedback?
10. Should UpgradePilot remain the primary flagship for the next Career cycle?

---

## 12. Technical handoff

There is intentionally **no exact immediate UpgradePilot technical action in this Career file**.

Resume every technical session from UpgradePilot's current project-local authority chain, beginning with its root governance and `MEMORY.md`, then follow whatever current plan/working-memory/source/test owner that repository selects.

Career defines the personal outcome and later evaluates evidence. UpgradePilot defines the technical continuation.
