# Current Near-Term Personal Execution Plan

**Owner:** Ali Rajabi  
**Status:** Active Career execution aid  
**Period:** 2026-08-10 through 2026-08-18  
**Career authority:** [`../CAREER_STATE.md`](../CAREER_STATE.md) and [`CURRENT_CAREER_CYCLE.md`](CURRENT_CAREER_CYCLE.md)  
**Technical capability checkpoint:** [`2026-08-18_TECHNICAL_CAPABILITY_CHECKPOINT.md`](2026-08-18_TECHNICAL_CAPABILITY_CHECKPOINT.md)  
**Technical truth owner:** `motafegh/UpgradePilot` `MEMORY.md`, current plan, source, tests, ADRs, learning evidence, and working memory

## 1. Purpose

Use the remaining period before the 2026-08-18 Day-30 Career review to convert the last five days of substantial UpgradePilot conceptual reconciliation into **retained understanding, executable feedback, and bounded Ali ownership** without slowing legitimate project progress or turning the next week into another theory phase.

This plan is a **Career execution and evidence plan**, not an UpgradePilot implementation plan. Career defines what capability/evidence should exist by August 18. UpgradePilot alone decides its technical continuation, exact source changes, tests, implementation slices, and project-local teaching method.

The active technical checkpoint remains frozen around the B2/Step-7 system established on August 5. The newer A→C product-decision model is treated as a **moving frontier**: it must become coherent and operational enough to support current work, but August 18 does not require independent mastery of the entire A→C theory.

## 2. What changed since the previous plan

The previous execution plan assumed UpgradePilot would move directly from Step 7F into the next implementation responsibility. Actual project progress was different and must now be reflected honestly.

By August 10:

- the Step-7 bounded semantic-extractor/runtime integration and parent Target-Python Support Relevance responsibility are complete and live-proven;
- the normal S001 public CLI path exposed and corrected real integration/generalization defects;
- UpgradePilot then spent several days reconciling its higher-level product-decision model rather than expanding product source;
- Conversations A, B, and C are closed;
- a cumulative A→C learning snapshot exists but explicitly does not certify mastery;
- post-C AUDIT-003 was reviewed and its accepted amendments were incorporated into the reconciliation record;
- Conversation D is not open;
- the selected `B2_TRANSPARENT_DECISION_METHOD_PLAN.md` is now materially stale against accepted A–C semantics and must be reconciled before generic decision-layer implementation;
- UpgradePilot's current expected sequence is:

```text
reconcile existing Transparent Decision plan
→ select smallest credible pre-D A–C implementation/evaluation slice
→ implement + test + inspect real behavior
→ use that evidence to decide whether a concrete Conversation-D dependency exists
```

Career interpretation:

> The August 6–10 conceptual phase was substantially justified, but its value now depends on returning accepted concepts to executable feedback. The immediate Career risk is no longer only implementation outrunning Ali's understanding; it is also the product's conceptual model growing faster than Ali can consolidate it while executable practice temporarily lags both.

The correction is:

```text
concept
→ bounded implementation/evaluation
→ test
→ real result/failure
→ correction
→ retained explanation
```

not another broad study phase.

## 3. Capacity and work pattern for August 10–17

### Weekly capacity

Maintain the existing **24 focused-hour Green ceiling**. Do not convert it into a quota.

For August 11–17, a strong target is approximately **18–22 focused hours**, with 24 remaining the ceiling. This is an execution target, not a success metric. A lower total with strong executable/ownership evidence is better than extra low-quality hours.

Use approximately four strong technical days plus one lighter/flexible day. Keep at least one meaningful recovery period over the weekend.

### Ali's three-block structure

#### Block A — laptop/desktop, about 45–75 minutes

Best use:

- delayed recall;
- source reading;
- syntax/mechanism learning;
- test reading;
- reconnecting an abstract concept to actual code;
- targeted repair of one fuzzy area.

Default rule:

> Start from memory/prediction before opening the explanation or source whenever practical.

#### Block B — phone/outside, about 90–120 minutes

This block is legitimately phone-based and should be used for what the context is good at:

- conceptual reasoning with project-local AI;
- A→C case reasoning;
- architecture explanation;
- challenge and decision discussion;
- retrieval practice;
- predicting implementation effects;
- interpreting outputs/failures;
- planning the next bounded technical move.

Do not force large source-file study or complex multi-file diff inspection into the phone block. Keep non-work notifications/apps suppressed as practical so the phone functions as a work terminal during this period.

#### Block C — laptop/desktop, normally 60–120 minutes

Best use:

- implementation;
- terminal work;
- tests;
- diff inspection;
- live proofs;
- debugging;
- verifying what AI changed.

AI-heavy implementation remains acceptable. The goal is not manual-code purity; the goal is increasing Ali understanding, prediction, modification, testing, and diagnosis behind the AI-assisted work.

### Day-length rule

- about 4 focused hours = full strong day;
- 5 hours = strong extension;
- 6 hours = exceptional, not default;
- do not extend the evening merely to make the stopwatch look better.

## 4. August-18 target — frozen Step-7 core

The detailed rubric remains [`2026-08-18_TECHNICAL_CAPABILITY_CHECKPOINT.md`](2026-08-18_TECHNICAL_CAPABILITY_CHECKPOINT.md). Do not replace or continuously expand it as UpgradePilot advances.

By August 18, the following Step-7-era core should be coherent at approximately the depth defined in that checkpoint.

### Must own strongly enough to explain and reason about

1. UpgradePilot's current mission and bounded-claim doctrine: evidence-backed decision support, not autonomous maintainer authority.
2. The complete request-to-current-result flow:

```text
public PR
→ exact PR/base/head identity
→ changed files
→ trusted dependency transition or explicit problem
├── independent exact-head CI evidence branch
└── upstream evidence branch
    → exact PyPI release
    → trusted upstream repository
    → package-wide release index
    → crossed releases
    → exact tag/commit
    → exact changelog
    → deterministic source window
    → bounded LLM candidate extraction
    → deterministic reconstruction/validation
    → grounded support-drop claim?
        ├── no → target remains inactive/unresolved for this responsibility
        └── yes → exact-head pyproject.toml
                  → requires-python
                  → bounded target relevance
```

3. Evidence identity, authority, provenance, and why exact revisions/SHAs/blobs matter.
4. Explicit problem/evidence states rather than collapsing expected uncertainty into booleans or exceptions.
5. CI independence and the difference among successful CI, dependency consumption/exercise, coverage, compatibility, and safety.
6. Old-exclusive/proposed-inclusive crossed-release reasoning and why only inspecting the final release is insufficient.
7. Deterministic versus semantic responsibility and the bounded LLM trust boundary.
8. Conditional target-Python activation and why it encodes relevance, not merely optimization.
9. Basic `pyproject.toml` / `requires-python` / PEP 440 relevance reasoning and why `outside_declared_python_range` is not `safe to merge`.
10. Application orchestration versus provider/domain logic versus CLI responsibility.
11. Generality versus authority, using the provenance-backed PyPI `Homepage` correction as the concrete example.
12. The LM Studio/proxy incident, loopback, `requests.Session`, and why `trust_env=False` was used.

### Python mechanisms that should be comfortable to read in the current code

```text
functions and returns
if/elif/else
for loops
try/except
raise/assert
list/tuple/dict/set
comprehensions
isinstance/type/getattr
@dataclass(frozen=True, slots=True)
Foo | Bar
str | None
Literal[...]
Sequence[...]
Callable[[...], ...]
keyword-only arguments after *
relative imports
injected clients/evaluators
expected problem values versus exceptions
```

Representative standard/library/tool mechanisms:

```text
requests.Session / HTTP status / timeout
json.loads and JSON structures
tomllib
packaging.version.Version
packaging.specifiers.SpecifierSet
argparse / os.getenv
unittest.TestCase
Mock / patch
assertEqual / assertIsNone / assert_called_once_with / assert_not_called
```

### Tools that should be operational rather than theoretical

Ali should be able to use or correctly interpret:

```text
python / python -m upgradepilot
targeted tests and the relevant active regression command
git status
git diff
git log
git show
basic source/test navigation
LM Studio local endpoint context
```

Career does not require memorizing every command flag or every repository file.

## 5. August-18 target — A→C moving frontier

A→C is new material and must not move the entire frozen checkpoint. The target here is **coherent operational understanding plus the first implementation-backed ownership evidence**, not independent mastery of all A→C concepts.

### 5.1 Compact invariants to make automatic

These should become highly retrievable because they prevent serious reasoning errors:

```text
observation != interpretation != evidence quality != decision
upstream change != target impact
target relevance != target ownership
missing evidence != negative evidence
relevant evidence != sufficient/discriminating evidence
LLM confidence != source authority != evidence completeness != semantic sufficiency
uses dependency != participates in affected mechanism != relies on specific changed property
successful investigation execution != valid evidence for the proposition
proxy evidence != exact-context evidence
no further justified investigation != not applicable != safe != overall evidence sufficient
```

Do not spend hours memorizing wording. The goal is to recall and apply the distinctions.

### 5.2 Conversation A — should be operationally coherent

Ali should be able to explain and use this model with project-local support:

```text
upstream change mechanism
+ target-relevant exposure/path
+ activation condition(s)
+ possible target-relevant consequence
= mechanism-specific impact candidate
```

Required understanding:

- upstream change alone does not establish target impact;
- exposure is the path through which the changed mechanism can matter to the target;
- activation is what must hold in the exact context for that path to matter;
- consequence is the possible target-relevant technical difference;
- one dependency transition can produce multiple mechanism-specific candidates;
- candidate formulation does not establish the truth of its own exposure/activation/component hypotheses.

Independent formulation of complete candidates across unfamiliar ecosystems is deferred.

### 5.3 Conversation B — should be operationally coherent

Ali should understand:

```text
established applicable
established not applicable
unresolved
conflicted
```

and be able to reason about:

- candidate-specific applicability propositions;
- necessary versus sufficient conditions;
- `AND` versus alternative `OR` paths;
- why one established complete viable path can establish positive applicability;
- why non-applicability requires closing every represented viable path;
- missing evidence versus negative evidence;
- open-world reasoning as the safe default;
- when a proposition-local closed boundary can justify absence;
- why completeness is itself an evidence claim.

The post-C audit adds one especially important August-18 guard:

```text
EVIDENCE COVERAGE
!= PATH-MODEL COVERAGE
!= CANDIDATE-DISCOVERY COVERAGE
```

Ali should understand the difference conceptually. Independent proof of complete negative conclusions is deferred.

### 5.4 Conversation C — understand the operating skeleton, not every refinement

Ali should be able to explain:

```text
material non-final proposition state
+ location/reason for uncertainty or conflict
→ discriminating target
→ candidate investigations
→ hard admissibility/context-validity boundary
→ qualitative comparison/pruning/complementarity
→ selected next investigation / bounded conditional sequence
   OR no further justified investigation
   OR multiple admissible non-dominated alternatives
→ execute/observe if authorized
→ validate the observation as evidence
→ reevaluate proposition or refine candidate
```

Prioritize these concepts before August 18:

- uncertainty/conflict location;
- discriminating target;
- relevant versus discriminating evidence;
- resolution versus material reduction/pruning;
- admissibility versus preference;
- hard/non-compensatory constraints;
- qualitative dominance/Pareto reasoning;
- pruning/shared-gate leverage;
- adaptive/conditional sequencing and bounded lookahead;
- observational versus interventional evidence;
- contrast validity;
- proxy evidence and reconstruction fidelity;
- successful execution versus valid evidence;
- candidate refinement/lineage;
- `no further justified investigation`;
- C stopping versus D overall sufficiency/action.

Ali does **not** need independent investigation planning across arbitrary cases by August 18.

### 5.5 Post-audit guards that must be recognized

By the review Ali should at least understand why these matter:

1. candidate formulation must not smuggle established truth;
2. evidence/path/discovery completeness are different;
3. C can start from genuine conflict as well as unresolved state;
4. epistemic usefulness, UpgradePilot execution admissibility, and later maintainer-facing recommendability are separate;
5. several non-dominated investigations may remain rather than one fake unique winner;
6. a C stop based on cost/value/policy trade-offs must not silently decide later maintainer policy;
7. implementation should use only the minimum bounded proposition/path composition semantics needed by the selected slice, not a universal Boolean engine;
8. candidate refinement should preserve lineage rather than silently rewriting history;
9. the old Transparent Decision plan must be reconciled before implementation;
10. B2 should implement a thin credible A–C manifestation, not a universal planner;
11. pre-D implementation is allowed only as an A–C feedback slice, not as a disguised final recommendation engine.

These guards are operational boundaries, not a new memorization exam.

## 6. What is explicitly deferred beyond August 18

Do not spend the next week trying to master:

- every one of the 45 A→C recall questions;
- all sections of the 3,000+ line learning note;
- independent complete candidate discovery on unfamiliar ecosystems;
- independent proof of negative propositions under arbitrary evidence universes;
- designing general differential experiments without support;
- universal investigation selection;
- generic Boolean/rule engines;
- universal dependency graphs or plugin/framework analysis;
- historical-environment reconstruction as a general capability;
- Conversation-D final sufficiency/policy/action semantics unless UpgradePilot exposes a concrete dependency;
- final maintainer recommendation architecture;
- broad cross-ecosystem transfer;
- every source file or test in UpgradePilot.

If a deferred concept becomes necessary for the real selected project slice, learn the minimum needed then.

## 7. Ownership evidence required before August 18

Career should try to obtain **several distinct pieces of evidence**, not a point score.

### Required or strongly preferred evidence

1. **Delayed reconstruction:** at least once, reconstruct the frozen Step-7 flow after a meaningful delay before opening source/notes.
2. **A→C reconstruction:** explain A, B, and C in your own words and connect them to at least one concrete UpgradePilot case.
3. **Prediction:** before one meaningful implementation/test/change, state what you expect to change and what outcome would support/refute the expectation.
4. **Meaningful source/test participation:** understand and materially influence at least one bounded implementation or test responsibility when the project reaches the selected pre-D slice.
5. **Test reasoning:** explain one representative test as setup → action → assertion → protected behavior → what it does not prove.
6. **Changed-case/transfer evidence:** use the accepted model on at least one case or changed condition not identical to the memorized S001 path, with project-local support.
7. **Debugging evidence:** if a real failure occurs, state the initial likely layer/cause before AI diagnosis. Do not manufacture a failure merely for Career.
8. **Explicit non-ownership:** identify at least one important current responsibility you still do not own instead of inflating the claim.

The proxy incident remains valid earlier diagnostic evidence, but new evidence is preferred where the real project naturally provides it.

## 8. Anti-drift rules for August 10–17

### Rule A — no second broad theory phase by default

Conversation D must not open merely because A–C are closed. Follow UpgradePilot `MEMORY.md` and require a concrete dependency before broad D theory.

### Rule B — after plan reconciliation, executable feedback should return quickly

Once the Transparent Decision plan is reconciled and a bounded slice is selected, implementation/testing should begin under UpgradePilot without another prolonged conceptual preface.

Career correction signal:

> If two consecutive active technical days pass after plan reconciliation with no executable/test/changed-case feedback and no concrete blocker, treat that as potential theory/documentation drift and ask UpgradePilot to justify why implementation is still not the highest-value next feedback source.

Career does not dictate the technical answer; it requires the project to justify the delay.

### Rule C — learning note is a reference, not a course

Do not reread the full mastery note sequentially.

Use its own efficient modes:

- quick recall from the one-page memory sheet;
- selected question sampling;
- one concrete case;
- one transfer/diagnosis exercise when useful;
- implementation feedback.

Default deliberate A→C consolidation should remain roughly **30–60 minutes on an active day**, unless a real project blocker requires more.

### Rule D — concepts must reconnect to code/evidence

Whenever a concept is reviewed, connect it to at least one concrete UpgradePilot artifact, case, source responsibility, test, or observed failure when possible.

### Rule E — do not punish the conceptual phase by overcorrecting

Do not suddenly force large manual coding quotas because August 6–10 was conceptual. AI-assisted implementation remains the accepted work model. The correction is more executable/ownership density, not artificial typing volume.

## 9. Daily execution plan

The dates below define emphasis, not technical sequencing. UpgradePilot `MEMORY.md` always owns the actual project gate.

### August 10 — close the conceptual phase cleanly

The day has already contained substantial A–C/audit work. Do not chase more hours tonight merely because the Career plan was updated.

If doing any final work, keep it short:

- explain A, B, and C in one or two sentences each from memory;
- name the current UpgradePilot continuation correctly;
- identify the single concept currently most fuzzy;
- stop.

Do not start broad Conversation D or another deep learning pass tonight.

### August 11 — re-anchor the frozen core and reconnect to implementation

**Block A:** reconstruct the Step-7 request-to-result flow from memory. Then check only the mistakes. Review one central source/test responsibility rather than rereading everything.

**Block B:** A-focused recall. Use the one-page memory sheet, then explain one impact candidate using a real case. Spend more time applying than rereading.

**Block C:** follow current UpgradePilot continuation. The project currently expects reconciliation of the stale Transparent Decision plan and selection of the smallest credible pre-D A–C slice. Before a meaningful project decision, state what you think the bounded slice should need to prove and why, then compare with project reasoning.

Ownership target: one prediction or meaningful challenge.

### August 12 — B reasoning plus return to source/test feedback

**Block A:** inspect a representative Step-7 source path and one relevant test. Be able to explain the code/test at responsibility level.

**Block B:** B-focused operational review:

```text
four states
positive path versus non-applicability
AND/OR paths
missing versus negative evidence
open/closed world
three completeness questions
```

Use a concrete case rather than only definitions.

**Block C:** if the reconciled plan/slice is ready, implementation/testing should now receive substantial time. If it is still not ready, require a concrete project reason rather than adding theory automatically.

Ownership target: explain or influence one test/contract boundary.

### August 13 — C skeleton and changed-case reasoning

**Block A:** brief code/test review from whatever the current real implementation slice now touches. Do not study every new module equally.

**Block B:** C-focused operational review:

```text
where is uncertainty/conflict?
what exact discriminating target matters?
what evidence would materially discriminate it?
what is admissible?
what options are dominated/non-dominated?
what would different outcomes prune or activate?
when should C stop?
```

Use one of the recorded C01/C203 cases or the real current implementation case.

**Block C:** normal implementation/test work. If a real failure occurs, use error → Ali hypothesis → AI investigation.

Ownership target: one changed-case prediction, investigation-choice explanation, or diagnosis.

### August 14 — integrate the old evidence engine with the new decision model

**Block A:** delayed full reconstruction:

```text
PR → Step-7 evidence path → bounded result
```

then add:

```text
A: what possible target impact are we even considering?
B: does it apply to this exact target/context?
C: if non-final, what investigation would discriminate it?
```

Do this before opening the full notes.

**Block B:** explain two cases from memory:

- S001 as the concrete evidence-engine case;
- one A→C challenge/pressure-test case.

Focus on why the evidence supports some claims and not others.

**Block C:** continue actual implementation/testing. Inspect `git diff`/test results and explain what changed rather than only accepting the AI summary.

Reserve **45–90 minutes** somewhere in the day for Career-market preparation if JobHunter/current market evidence still needs representative coverage for August 18.

Ownership target: one coherent end-to-end explanation plus one source/test effect you can defend.

### August 15 — recovery by default

Default to recovery and normal life.

Optional 30–60 minute fast recall only if you genuinely want it:

- one-page A→C memory sheet;
- five random A→C questions;
- one frozen-core question cluster.

Do not use the day for a giant catch-up session.

### August 16 — flexible/replacement day

If August 11–14 produced four strong days, keep this mostly recovery or use at most one bounded 1–2 hour session.

If a weekday was lost or the real project has a valuable bounded gate/proof, use one 3–4 hour technical day without exceeding the weekly ceiling.

Best optional use:

- implementation/test ownership;
- one transfer case;
- filling one genuine frozen-core gap;
- finishing representative JobHunter/market evidence.

Do not spend the day rereading all A–C material.

### August 17 — pre-review consolidation, not cramming

Use approximately 3–4 focused hours maximum unless normal project work genuinely requires more.

#### Part 1 — technical reconstruction

Without immediately opening notes:

- explain UpgradePilot mission and current bounded behavior;
- reconstruct the frozen Step-7 flow;
- explain A, B, and C and their boundaries;
- explain how A–C relates to the currently selected implementation slice;
- state where your confidence drops.

#### Part 2 — question sampling

Use the August-18 checkpoint question bank as a **sampling pool**, not a memorization list.

Suggested rehearsal:

- 12–15 frozen-core questions chosen across architecture, Python, CI/API/trust/testing;
- 8–10 A→C questions chosen across A, B, C, and post-audit guards;
- answer aloud before checking notes.

Repair only the important gaps exposed by the sample.

#### Part 3 — ownership evidence summary

Prepare a concise private record:

```text
What I can now explain without help:
What I can use with some support:
What I still do not own:
Best implementation/modification evidence:
Best test evidence:
Best debugging/diagnosis evidence:
Best changed-case/transfer evidence:
One place I challenged/predicted AI/project reasoning:
```

#### Part 4 — Career evidence

Have ready:

- actual stopwatch hours since the last review;
- active days and any overload;
- current UpgradePilot stage and material progress;
- representative market/JobHunter evidence required by the Career cycle;
- current UpgradePilot portfolio explanation;
- any exact blocker to application readiness.

No major new Career document is required merely to prepare this evidence.

## 10. August 18 — assessment day

Do not spend the morning trying to memorize answers.

The Day-30 Career review should inspect five things separately:

1. **Capability:** frozen technical checkpoint plus bounded A→C moving-frontier understanding.
2. **Ownership:** explanation, prediction, modification/test participation, diagnosis, transfer, and explicit non-ownership.
3. **Project/portfolio:** what UpgradePilot materially became and what Ali can honestly claim.
4. **Workload:** actual focused-time evidence and sustainability.
5. **Market/application readiness:** representative role evidence and an explicit application decision or exact blockers.

A strong technical result does **not** require perfect recall. Career should prefer causal explanation and changed-case reasoning over memorized vocabulary.

A suitable technical assessment may include:

- reduced-prompt architecture reconstruction;
- selected checkpoint questions;
- reading/explaining a representative source fragment;
- explaining a representative test;
- changed-case reasoning;
- one debugging/modification story;
- A→C explanation and one applied case;
- explicit statement of current non-owned responsibilities.

The review must not inflate broad D3/D4 from project sophistication or from the existence of the learning note.

## 11. Success condition by August 18

This period is successful if most of the following are true:

- UpgradePilot has returned from conceptual reconciliation to executable/evaluation feedback as soon as its own method permits;
- the frozen Step-7 system is substantially more coherent and retained than on August 5;
- Ali can explain the central A→C skeleton and important guards without pretending independent mastery;
- A→C knowledge has begun connecting to implementation/tests/changed cases rather than remaining only conversational theory;
- several distinct ownership signals exist;
- the learning note functioned as a reference/retrieval tool rather than a new course;
- no broad Conversation-D theory, second flagship, or unrelated curriculum displaced higher-value work without a concrete need;
- workload remained sustainable and the 24-hour ceiling was not treated as a quota;
- enough market/portfolio evidence exists for a real application-readiness decision on August 18.

## 12. Correction signals

Apply the smallest correction if any of these appear:

- two consecutive active days after plan reconciliation with no executable/test feedback and no concrete blocker;
- repeated full-note rereading instead of retrieval/application;
- inability to explain A/B/C even at the three-question skeleton after repeated guided conversation;
- new implementation advances substantially while Ali cannot identify its responsibility, inputs/outputs, or claim limits;
- Career or JobHunter begins competing materially with UpgradePilot;
- weekend work is being used only to repair guilt about hours;
- broad D theory starts because it is intellectually interesting rather than technically required;
- AI/project sophistication is being mistaken for Ali capability.

## 13. Minimum daily evidence

Keep tracking lightweight. At the end of each active day record only:

```text
Date — focused time
Current UpgradePilot gate/responsibility:
One thing I can now explain better:
One ownership signal: prediction | challenge | modification | test | diagnosis | transfer
One important thing still fuzzy:
Energy: good | acceptable | overloaded
```

This evidence is for the August-18 review, not for productivity theater.

## 14. Authority boundary

Career may use this plan to say **what Ali should be able to demonstrate and what evidence should exist**.

Career must not use it to dictate UpgradePilot source design, select concrete implementation internals, write project-local tests, or replace UpgradePilot's own learning/execution system.

When a technical gap appears, UpgradePilot should teach/practise it locally. Career later evaluates whether the resulting capability evidence justifies a stronger claim.
