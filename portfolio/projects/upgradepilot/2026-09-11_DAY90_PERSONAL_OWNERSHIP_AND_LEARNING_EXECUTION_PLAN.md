# UpgradePilot — Day-90 Personal Ownership and Learning Execution Plan

**Date:** 2026-09-11  
**Horizon:** 2026-09-11 through 2026-10-17  
**Owner:** Ali Rajabi / Career  
**Status:** Active Career-level personal execution plan; AI-era resilience refinements adopted 2026-09-11  
**Technical authority:** `motafegh/UpgradePilot` root governance, `MEMORY.md`, selected project plan, active working memory, source/tests, and project-local Learning-by-Doing system  
**Career authority:** `../../../CAREER_STATE.md`, `../../../plans/CURRENT_CAREER_CYCLE.md`, `../../../plans/CURRENT_WEEK.md`, and this project's `CAREER_RECORD.md`

## 1. Purpose

Use UpgradePilot as Ali's sole primary capability-building flagship for the remainder of the current Career cycle while converting repository sophistication into stronger **personal engineering ownership**.

This plan answers:

> What should Ali personally learn, understand, practice, verify, modify, diagnose, and be able to explain through legitimate UpgradePilot work before the Day-90 Career review?

It does **not** own UpgradePilot's exact technical continuation, implementation order, source/test TODO, or project gate sequence.

Use the separation:

```text
Career plan
→ personal outcomes / depth / evidence opportunities / allocation / stop lines

UpgradePilot
→ exact current responsibility
→ A→B→C→D→E Learning-by-Doing sequence
→ source/tests/commands/proof
→ technical next slice
```

When this file and UpgradePilot's current `MEMORY.md` differ about technical continuation, UpgradePilot wins.

---

## 2. Day-90 target

By 2026-10-17, UpgradePilot should have helped Ali move from broad AI-assisted exposure toward a smaller set of **defensible current engineering responsibilities**.

A strong cycle result is:

```text
several current source/test responsibilities genuinely understood
+ representative tests Ali can reason through
+ at least one legitimate ownership-bearing modification if project work creates the opportunity
+ at least one credible current causal-diagnosis case if a real failure occurs
+ changed-context transfer beyond memorized examples
+ concise technical explanation of UpgradePilot at multiple depths
+ continued strong AI-agent direction without pretending AI output is personal implementation ownership
```

These are directional evidence targets, not quotas. Do not manufacture changes, failures, or exercises merely to satisfy this list.

The AI-era resilience lens is:

> **Use AI aggressively for execution, but make Ali's learning increasingly about the engineering responsibility that remains: intent, technical mental model, acceptance criteria, verification, diagnosis, meaningful correction, transfer, risk and explanation.**

This does not replace technical depth with management-only thinking.

---

## 3. Current entry point — 2026-09-11 snapshot

At plan creation, UpgradePilot `main` has advanced into the overall maintainer-action synthesis responsibility.

Current project-local state, for orientation only:

- the accepted synthesis layer consumes `PublicPullRequestInvestigation` and produces bounded maintainer-facing action reasoning;
- the first deterministic evaluator is implemented in `src/upgradepilot/maintainer_action.py`;
- the first evaluator currently admits only explained `abstain`;
- focused tests exist in `tests/test_maintainer_action.py`;
- source/static validation is recorded, while focused execution against the actual repository environment and broader regression proof remain explicit debt;
- the active project-local Learning-by-Doing record places the current slice in D/E ownership learning before selecting the next implementation slice.

This snapshot is **not** a durable technical continuation rule. Re-read UpgradePilot `MEMORY.md` whenever resuming project work.

---

## 4. Ali's operating rule for every substantive UpgradePilot slice

UpgradePilot's own A→B→C→D→E loop remains controlling. Ali should use it with the following personal ownership emphasis.

### A — Before real work

Ali should be able to state, in his own words:

1. what responsibility is being changed, investigated, or proved;
2. where its input comes from;
3. what output/state it is expected to produce;
4. the main decision, uncertainty, or failure boundary;
5. what would count as useful proof for this slice.

For a consequential new responsibility, also state proportionately:

- what **success** means;
- what important **failure / unresolved state** must remain distinguishable;
- one important **non-goal or stronger claim that is not earned**;
- what evidence/test/evaluation would justify acceptance;
- one changed case that could discriminate a weak design from a good one.

Do not require full implementation knowledge before work begins. The goal is enough mental model and acceptance intent to make the action meaningful, not to pre-design every line before learning from real implementation.

### B — During real work

AI may write substantial or most code.

Ali should personally engage when the slice contains:

- a consequential behavior or contract choice;
- a new data/state representation;
- a new failure or uncertainty rule;
- a test that establishes an important product claim;
- a potentially overengineered abstraction/framework;
- a security/trust/provenance boundary;
- a meaningful implementation alternative.

Ali does not need to type code manually merely to create ownership evidence.

### C — Preserve project truth

Let UpgradePilot maintain its own working memory and technical state.

Career should only retain the resulting capability/portfolio conclusion when something materially changes Ali's demonstrated evidence.

### D — After implementation/investigation

Ali should trace the **real** result rather than only reread the plan.

For the selected responsibility, Ali should be able to answer:

```text
What enters this responsibility?
What important types/states exist?
What branches or transformations matter?
What leaves it?
What does the representative test establish?
What does it NOT establish?
What can fail or remain unresolved?
Why is this design placed here rather than somewhere else?
```

For consequential slices, use the **automation-compression reflection** when it adds value:

> **If implementation became nearly free, what engineering responsibility would still be mine — and what technical understanding would I still need to verify, diagnose, modify, transfer and defend that responsibility?**

The answer must name technical substrate, not only management or review language. Skip or compress this reflection for familiar/repetitive child work.

### E — Repair and transfer

Repair only important understanding gaps.

Then ask at least one changed-context question, such as:

- What changes if this input is missing instead of malformed?
- What changes if evidence conflicts instead of being unavailable?
- Which test would fail if this invariant were removed?
- Would the same design still work for a nearby but different case?
- What evidence would be needed before a stronger action/claim became justified?

For selected important slices, add the bounded **transferability reflection**:

```text
What is the transferable engineering responsibility here?
What UpgradePilot-specific/domain knowledge only supports it?
Where else would the same responsibility appear?
```

Do not manufacture a generic lesson from every file/function. The objective is transfer, not memorization or ceremony.

---

## 5. What Ali should become strong in through UpgradePilot

These are the primary transferable engineering anchors.

### 5.1 Python / software engineering

Target: increasingly strong working depth.

Prioritize when encountered in real source:

- functions, parameters, return values;
- modules/import boundaries;
- classes and dataclasses;
- collections and immutable/mutable data structures;
- `None`, unions, `Literal`, enums/state vocabularies where used;
- practical type annotations and their runtime limits;
- control flow and branching;
- helper/private functions;
- exceptions and typed problem states;
- interfaces between application/domain/provider layers;
- reading unfamiliar code;
- making bounded changes without losing the surrounding contract;
- predicting representative behavior before execution;
- understanding and reviewing AI-generated diffs rather than only final output.

Do not turn this into a detached Python curriculum. Learn syntax/concepts just in time from active source. Strength means engineering mental-model ownership, not syntax recall or blank-page boilerplate speed.

### 5.2 Testing, verification, and evaluation

Target: strong early-career working depth.

Ali should increasingly understand:

- test setup / fixture / action / assertion;
- why one test exists;
- what product claim a test can and cannot support;
- whether the test/eval oracle actually matches the intended requirement;
- positive, negative, unresolved, malformed, changed and useful adversarial cases;
- regression tests;
- source bug vs fixture bug vs environment failure vs provider failure;
- focused proof vs broader suite/system proof;
- static validation vs executable validation;
- false confidence from green checks;
- model/agent evaluation where AI behavior is part of the responsibility;
- why green tests do not prove production safety or personal ownership.

### 5.3 Debugging and causal diagnosis

Target: meaningful evidence before Day 90 if real failures arise.

When a real failure occurs, Ali should participate before accepting a complete AI diagnosis:

```text
observe symptom
→ form one or more plausible cause families
→ choose useful discriminating evidence
→ narrow the failing boundary
→ distinguish code/test/environment/external-system causes
→ choose or challenge the repair
→ verify the repair or unresolved state
```

AI may run commands and inspect code. Ali's evidence comes from useful causal participation, not manual keystrokes.

### 5.4 System/data/evidence reasoning

Target: maintain as a relative strength and connect it more tightly to implementation.

Become comfortable reasoning about:

- exact identity and revisions;
- provenance/authority;
- missing vs negative evidence;
- unsupported vs unresolved vs conflicted states;
- data/state composition across modules;
- external-provider boundaries;
- evidence strength versus decision permission;
- explicit abstention/claim limits;
- responsibility ownership between layers.

Do not allow conceptual evidence reasoning to substitute for being able to inspect, change, test and diagnose the implementation carrying that evidence.

### 5.5 Intent / specification / acceptance ownership

Target: explicit cross-cutting engineering responsibility, not a detached curriculum.

On consequential work Ali should increasingly be able to state:

```text
what problem/responsibility is actually owned
what success means
what failure/unresolved state matters
what stronger claim is intentionally not earned
what evidence would justify acceptance
what changed case would pressure the design
```

This is technical responsibility ownership. It must remain tied to real source/tests/evidence rather than becoming abstract product-management prose.

### 5.6 AI-agent engineering

Target: preserve as a differentiator while strengthening technical accountability.

Continue practicing:

- scoping tasks for agents;
- supplying the right repository context;
- selecting the right operation/Skill;
- preventing scope drift and overengineering;
- challenging model assumptions;
- demanding evidence rather than polished prose;
- using tests/evals as feedback;
- preserving durable working state;
- selecting tools/models proportionately where relevant;
- setting permissions/human checkpoints where relevant;
- deciding what requires human judgment;
- checking that the produced source/test behavior matches the intended responsibility.

Avoid reducing this to "prompting skill". The professional claim is engineering leverage with verification and accountability.

---

## 6. What Ali only needs at working/domain depth

Understand these well enough to reason about and defend UpgradePilot, but do not make them standalone specialization goals this cycle:

- Dependabot behavior;
- Python packaging/PyPI specifics;
- dependency-update evidence;
- GitHub Actions/CI consumption details;
- upstream changelog/release evidence;
- Python-support-drop reasoning;
- artifact serviceability;
- target-environment composition;
- maintainer-action synthesis;
- product-specific evidence-state vocabularies.

These are the **domain vehicle** for learning engineering, not the target profession.

---

## 7. What should remain deferred unless real project pressure appears

Do not spend the remaining cycle mastering or re-opening these merely for breadth:

- LangGraph internals;
- LangChain internals;
- generic multi-agent architecture;
- broad cloud/Kubernetes infrastructure;
- advanced Python metaprogramming/type-theory rabbit holes;
- every GitHub API endpoint;
- every UpgradePilot module or historical plan;
- persistence/database machinery merely to create SQL résumé keywords;
- new frameworks or abstractions without demonstrated product need.

If UpgradePilot later re-admits one of these for a real responsibility, reassess proportionately.

---

## 8. Evidence opportunities to use when they naturally occur

### Priority A — ownership-bearing modification

A high-value case has this shape:

```text
Ali understands the pre-change responsibility
→ real project need requires a change
→ Ali predicts/helps decide intended behavior
→ AI may implement substantial code
→ Ali inspects source/tests/results
→ Ali can explain why the change is correct and what remains limited
```

Do not count commits under Ali's GitHub identity without this responsibility evidence.

### Priority B — real causal diagnosis

Use a real current failure when one appears.

Good evidence includes Ali selecting a useful cause family, inspection step, or boundary that materially advances diagnosis.

Do not inject fake bugs for Career evidence.

### Priority C — changed-context transfer

After learning one responsibility, use a nearby changed case to test whether the mental model transfers.

This is especially valuable for:

- missing vs conflicting evidence;
- different dependency source shapes;
- different CI/static-consumption states;
- different applicability states;
- different synthesis permissions/abstention boundaries.

### Priority D — technical explanation

Periodically practice explaining one selected responsibility without reading the implementation line-by-line.

Aim for:

- concise architecture/data-flow explanation;
- one representative test;
- one failure/uncertainty case;
- one design decision/tradeoff;
- the transferable responsibility when useful;
- accurate AI-assistance boundary.

---

## 9. Calendar route to Day 90

### Phase 1 — 2026-09-11 through 2026-09-17

**Primary UpgradePilot outcome:** close the current legitimate synthesis slice properly and continue only through project-owned gates.

Ali focus:

- complete the current D/E ownership check on the active maintainer-action synthesis slice;
- understand the current source/test flow at practical depth;
- participate in pending executable proof when an eligible project environment is available;
- if proof fails, participate in the diagnosis before accepting a fix;
- let UpgradePilot choose the next justified technical slice after the gate closes.

Career parallel lane:

- finish the very small remaining E2 GitHub UI work;
- do not let portfolio work displace meaningful UpgradePilot work.

**September 17 checkpoint:** inspect whether E2/application activation or a material UpgradePilot ownership event requires a Career update. Do not run a duplicate full review automatically.

### Phase 2 — 2026-09-18 through 2026-09-30

**Primary UpgradePilot outcome:** convert continuing legitimate project work into stronger implementation/test ownership.

Ali focus:

- continue the real project route, not a Career-invented exercise sequence;
- select the most important current source/test responsibility in each substantive slice;
- use real modifications and real failures as ownership opportunities;
- practice changed-context reasoning after important slices;
- increasingly explain why tests/proof are sufficient for a bounded claim and insufficient for stronger claims;
- use automation-compression/transfer reflections only on consequential slices where they sharpen ownership.

Career parallel lane:

- after E2 closure, begin the pre-authorized narrow application-calibration band;
- keep SQL/Git work bounded and secondary to the flagship.

### Phase 3 — 2026-10-01 through 2026-10-12

**Primary UpgradePilot outcome:** consolidate transferable engineering depth and interview-defensible project ownership.

Ali focus:

- continue only high-value legitimate project work;
- revisit selected central responsibilities if needed for integrated understanding, not memorization;
- practice explaining UpgradePilot at multiple depths;
- use classified application/interview feedback to identify only high-value gaps that UpgradePilot can legitimately improve;
- avoid new frameworks/architecture simply because Day 90 is approaching.

Career parallel lane:

- refine role targeting from real market response;
- strengthen SQL/Git/interview skills only where evidence shows value.

### Phase 4 — 2026-10-13 through 2026-10-17

**Primary UpgradePilot outcome:** consolidate and assess, not expand.

Ali should be able to present:

1. **30-second explanation** — user/problem/product value;
2. **2-minute explanation** — main evidence flow, current behavior, why trust/abstention matters, Ali-vs-AI contribution;
3. **technical discussion** — selected source/test responsibilities, a real design decision, a real modification/diagnosis if available, proof limits, one changed-context example, and the transferable engineering responsibility behind selected project-specific mechanisms.

Do not chase project completion for its own sake during this closeout window.

Day 90 assesses capability, evidence, market feedback, and next-cycle direction—not feature count.

---

## 10. Weekly capacity guidance

Career's Green ceiling remains up to **24 focused hours/week**, not a quota.

Default allocation:

```text
UpgradePilot personal technical attention: approximately 18–20 hours
Career / E2 / applications / SQL / Git:    approximately 4–6 hours combined
```

Use the range flexibly.

A meaningful UpgradePilot slice may justify more flagship time in one week. Career administration should not consume a technical week.

Autonomous JobHunter/Sentinel AI work is not Ali's personal learning time.

---

## 11. Relationship to applications, SQL, and Git

### Applications

UpgradePilot should **continue while applications begin** after E2 closure.

Do not wait for UpgradePilot completion or broad D3 ownership before collecting bounded market feedback.

Application evidence may later change what deserves emphasis inside this plan, but only after Career classifies whether the signal is a transferable technical gap, positioning issue, access gate, role-fit issue, or low-information noise. Career must not distort UpgradePilot's technical route for one vacancy keyword or unexplained rejection.

### SQL

SQL remains a material role-widening gap.

Do not force relational persistence into UpgradePilot if the product does not need it.

If no legitimate UpgradePilot responsibility supplies relational evidence, Career may run the separately authorized bounded SQL intervention after E2 closure.

### Git / review

When legitimate UpgradePilot work naturally supports branch/PR/review practice, use it.

Do not create synthetic collaboration ceremony solely to satisfy Career evidence.

---

## 12. Practical session template for Ali

For an ordinary UpgradePilot session, recover only these questions:

```text
1. What does UpgradePilot MEMORY.md say is current?
2. What is the current A/B/C/D/E stage?
3. What one engineering responsibility should I personally understand better today?
4. What source/test/proof should I be able to explain afterward?
5. What acceptance boundary or stronger non-claim matters for this responsibility?
6. Is there a legitimate modification or real failure where I should take more responsibility?
7. For a consequential slice, would the automation-compression or transferability question sharpen my ownership?
8. What depth is enough today, and what should remain deferred?
9. Did anything happen that materially changes my Career capability/portfolio evidence?
```

If question 9 is no, do not update Career merely because a project session happened.

---

## 13. Stop lines

Do not:

- try to master the whole repository;
- manually rewrite AI-generated code merely to prove effort;
- count repository progress as Ali capability automatically;
- manufacture bugs or arbitrary modifications;
- turn automation-compression into management-only learning or repetitive ceremony;
- force a generic transfer lesson from every implementation detail;
- force SQL/cloud/frameworks into UpgradePilot for résumé breadth;
- reopen LangGraph/LangChain without real project justification;
- spend days rereading historical plans when current source/plan is enough;
- let documentation/governance replace real source/test/proof work;
- wait until UpgradePilot is "finished" before applying for jobs;
- let applications consume the flagship learning route;
- pursue mid/senior claims unsupported by current evidence.

---

## 14. Day-90 evidence review questions

At the 2026-10-17 Career review, ask:

1. Which current UpgradePilot responsibilities can Ali now trace and explain without heavy prompting?
2. Which representative tests/evaluations can he interpret correctly, including oracle quality and proof limits?
3. Did a legitimate ownership-bearing modification occur? What exactly was Ali's responsibility?
4. Did a real current failure diagnosis occur? What causal contribution was Ali's?
5. Can Ali transfer reasoning to a changed case and distinguish transferable responsibility from project-domain detail?
6. Has Ali become better at stating acceptance/non-goal/claim boundaries before consequential work?
7. Has AI-agent direction become more technically accountable rather than merely more elaborate?
8. Can Ali defend UpgradePilot clearly to an employer without overclaiming authorship?
9. Which gaps remain genuinely employment-relevant after **classified** application feedback?
10. Should UpgradePilot remain the primary flagship for the next Career cycle?

---

## 15. Exact immediate action

Resume UpgradePilot from its current project-local owner, not from this Career plan.

At the 2026-09-11 snapshot that means:

```text
complete the active maintainer-action synthesis D/E ownership stage
→ obtain the pending focused executable proof when the real environment permits
→ participate in diagnosis if proof fails
→ let UpgradePilot select the next legitimate bounded slice
→ repeat the project A→B→C→D→E loop with increasing Ali ownership
```

In parallel, close the remaining E2 GitHub UI actions and then activate the already-authorized narrow application-calibration lane.