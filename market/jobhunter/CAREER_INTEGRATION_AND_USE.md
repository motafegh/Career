# JobHunter Career Integration and Use

**Status:** Approved Career-side integration contract  
**Applies to:** Any JobHunter output used to influence Career decisions  
**External implementation repository:** `motafegh/jobhunter`

## 1. Purpose

This file defines how Career may use JobHunter evidence without allowing a market-analysis tool to become an unreviewed career authority.

The rule is simple:

> JobHunter produces observations, interpretations, aggregates, and proposals. Career reviews them and decides.

## 2. Authority chain

Use the following order when JobHunter contributes to a Career decision:

```text
1. original employer/public source
2. deterministic source representation
3. translation, clearly marked as derived
4. evidence-backed semantic analysis
5. normalized/taxonomy mapping
6. aggregate market calculation
7. Ali-specific comparison using Career-approved evidence
8. Career review
9. Career decision
```

A lower layer may add convenience or interpretation but may not silently overwrite the meaning of a higher layer.

## 3. Truth ownership

### JobHunter owns

Within its repository and runtime, JobHunter owns:

- source acquisition implementation;
- source adapters;
- raw/source evidence storage;
- job identity and semantic version implementation;
- fetch/check history;
- translation artifacts;
- semantic-analysis artifacts;
- taxonomy implementation;
- market calculations;
- search-effectiveness calculations;
- local UI/CLI/API/export implementation;
- JobHunter-specific tests and operational evidence.

### Career owns

Career owns:

- target role strategy;
- long-term and working career identity;
- Ali capability evidence and claim limits;
- project portfolio allocation;
- learning/capability priorities;
- application-readiness stage;
- portfolio and CV claims;
- current Career action;
- final interpretation of JobHunter market evidence.

## 4. JobHunter is not automatic capability evidence

JobHunter's own source code, architecture, features, tests, or sophistication do not establish Ali capability merely because the repository belongs to Ali or was built under Ali's direction.

Career may credit JobHunter implementation only after a normal capability review establishes a bounded responsibility Ali can explain, modify, test, diagnose, and defend at the claimed assistance level.

Until then, JobHunter is a **career-support system**, not a capability-building flagship.

## 5. Market evidence versus personal evidence

Never merge these concepts silently.

```text
Market evidence
= what employers appear to want

Personal evidence
= what Ali can currently defend
```

Examples:

- High SQL demand does not mean Ali may list SQL as a skill.
- Weak current Docker evidence does not mean Docker should be removed from the market analysis.
- A repository importing FastAPI does not prove Ali independently owns API design.
- A job asking for Kubernetes does not make Kubernetes a Career priority unless the broader evidence and Career context justify it.

## 6. Career-use gates

JobHunter outputs may be used at different levels of consequence.

### Gate A — exploratory observation

Appropriate for:

- discovering titles;
- noticing unfamiliar requirements;
- finding possible role families;
- deciding what to inspect manually next.

A small or imperfect sample is acceptable when clearly labeled exploratory.

### Gate B — repeated market pattern

Required before changing:

- role-family emphasis;
- capability priority;
- interview preparation focus;
- broad CV positioning.

The pattern should use multiple distinct jobs and expose the sample, source, time window, and uncertainty.

### Gate C — material Career decision

Required before materially changing:

- strategy;
- flagship/supporting project allocation;
- current cycle outcomes;
- application-readiness decision;
- geographic direction.

Career should inspect the underlying JobHunter artifact, sample quality, representative source examples, Ali capability evidence, and the smallest reasonable change.

### Gate D — individual application decision

For one vacancy, a smaller sample is naturally acceptable because the question is specific to that employer.

The decision must still distinguish:

- employer-explicit requirements;
- inferred supporting capabilities;
- Ali evidence;
- Ali gaps;
- hard constraints;
- uncertainty.

## 7. Minimum information required for a market pattern

A JobHunter aggregate should not influence Career materially unless it provides, or allows Career to recover:

- report/snapshot date;
- source(s);
- search/sample scope;
- geography;
- time window;
- distinct jobs analyzed;
- exclusions and major missing data;
- duplicate/repost treatment;
- requirement/responsibility denominator;
- required/preferred/contextual/inferred distinction;
- native/translated distribution when relevant;
- parser/translation/analysis/taxonomy versions;
- quality or uncertainty warnings;
- representative source postings.

## 8. Representative-sample standard

No universal fixed job count is required.

The required sample depends on the question.

Examples:

- `What does this employer require?` — one current posting may be sufficient.
- `Is SQL common in junior data roles in the UAE?` — requires multiple current postings from a reasonable source mix.
- `Should Career change its primary role direction?` — requires a materially stronger and broader body of evidence plus Ali capability/interest/feasibility review.

Career should prefer diversity across companies and sources over many near-duplicate postings.

## 9. Search-selection bias control

Every JobHunter market conclusion must be interpreted relative to how the jobs were found.

If the active search catalog intentionally emphasizes AI, Python, and security, the resulting sample cannot be described as a neutral sample of all junior technology employment.

For important comparisons, JobHunter should expose targeted profiles and broader control profiles.

Career should ask:

- Did we search for the thing we later claimed was common?
- Are we comparing equivalent search methods across role families or geographies?
- Did one source or company dominate the sample?
- Did a search-catalog change create an apparent trend?

## 10. Translation and model-output rule

Translation and semantic LLM analysis are derived data.

Career may use them for scale and convenience only when provenance remains available.

For material or surprising conclusions, Career should be able to inspect representative original source passages.

Model-derived `inferred` requirements must never be aggregated together with employer-explicit `required` requirements without visible separation.

## 11. Taxonomy rule

Normalized concepts improve aggregation but can also distort employer intent.

Career should require:

- original wording retained;
- mapping version retained;
- uncertain mappings visible;
- tools separated from underlying capabilities when possible;
- no aggressive merging merely to improve charts.

When a Career decision depends on one canonical concept, representative aliases and source examples should remain inspectable.

## 12. Career capability snapshot boundary

Any Ali-specific JobHunter comparison must use a Career-approved capability/evidence snapshot rather than inferring capability directly from GitHub.

The snapshot should preserve:

- exact responsibility/capability;
- evidence depth;
- assistance;
- recency;
- confidence;
- transfer limit;
- claim boundary.

JobHunter may compute comparisons from this snapshot, but Career remains authoritative for the underlying personal evidence.

## 13. Allowed Career effects

Reviewed JobHunter evidence may support changes to:

### Strategy

- role-family priority;
- geographic emphasis;
- work-mode emphasis;
- long-term specialization hypotheses.

### Capability planning

- increase/decrease priority of a recurring capability;
- identify a new employment-critical gap;
- distinguish core foundations from fashionable optional tools;
- decide whether standalone study is justified.

### Project portfolio

- identify natural responsibilities that could create missing evidence;
- justify a bounded supporting exercise;
- reject unnecessary project scope;
- decide which historical project evidence is relevant to a role.

### Employability

- determine realistic role bands;
- identify application blockers;
- activate or narrow calibration applications;
- identify target companies/roles for testing positioning.

### CV and GitHub

- tailor emphasis and terminology when evidence exists;
- reorder project/skill emphasis;
- identify presentation gaps;
- identify unsupported keywords that must not be added.

### Interview preparation

- prioritize recurring technical and responsibility areas;
- prepare project-defense topics;
- create changed-case/debugging practice around actual employer expectations.

## 14. Effects JobHunter may not perform automatically

JobHunter must not automatically:

- change `CAREER_STATE.md`;
- change `CAREER_STRATEGY.md`;
- change project allocation;
- add or strengthen capability claims;
- update the Capability Evidence Ledger;
- add technologies to UpgradePilot or another project;
- activate applications;
- edit the master CV;
- publish personal/private data;
- create a new Career project;
- convert one employer requirement into a curriculum change.

It may produce proposals for review.

## 15. Recommended Career review packet

When JobHunter evidence is brought into a Career review, prefer a compact packet containing:

1. **Career question** — the decision we are considering.
2. **JobHunter artifact** — snapshot/report/version.
3. **Sample** — source, time window, geography, role scope, distinct job count.
4. **Pattern** — what appears repeatedly true.
5. **Counterevidence/outliers** — what does not fit the pattern.
6. **Quality limits** — source/search/model/taxonomy uncertainty.
7. **Ali evidence** — relevant Career-approved capability evidence.
8. **Current gap** — if any.
9. **Proposed smallest Career change** — learn, practise, build, document, apply, monitor, defer, or no change.
10. **Reassessment trigger** — what future market/capability evidence would confirm or reverse it.

## 16. Decision examples

### Example: market evidence changes a capability priority

```text
Question:
Should SQL move higher in the current capability stack?

JobHunter evidence:
SQL is repeatedly explicit and frequently required across current realistic Python/data/backend roles.

Career evidence:
Ali's relational-data evidence remains weak.

Decision:
Increase SQL priority when a bounded responsibility can create real evidence.

Non-decision:
Do not call Ali SQL-capable yet.
```

### Example: market evidence prevents project bloat

```text
Question:
Should a new advanced platform be added to the flagship?

JobHunter evidence:
The platform is uncommon in current realistic junior roles; testing, SQL, APIs, and debugging recur much more often.

Career evidence:
Those core responsibilities remain under-evidenced.

Decision:
Do not add the advanced platform merely for résumé breadth.
```

### Example: individual application

```text
Question:
Should Ali apply to this AI application role?

Employer evidence:
Python/API integration required; SQL required; Docker preferred; Kubernetes not mentioned.

Ali evidence:
Python/API project evidence exists with assistance limits; SQL evidence weak; Docker introductory.

Decision:
Potentially reasonable stretch if other constraints fit. Tailor toward API/evidence work and prepare SQL honestly.
```

## 17. Career record placement

JobHunter raw evidence and detailed artifacts remain in JobHunter.

Career should normally record only durable conclusions.

Examples:

- recurring role pattern → `market/EMPLOYABILITY_AND_MARKET_PLAN.md` or a formal review conclusion;
- changed role strategy → `strategy/CAREER_STRATEGY.md` through review;
- changed live employability phase → `CAREER_STATE.md`;
- changed capability conclusion → `tracking/CAPABILITY_EVIDENCE_LEDGER.md` only when Ali evidence changes;
- project allocation change → portfolio/strategy owners;
- application-specific private detail → outside the public Career repository.

Do not copy JobHunter's database or large job dumps into Career.

## 18. Stable bridge requirement

The preferred long-term integration is a simple, explicit bridge:

```text
JobHunter
→ versioned Career-facing export/API
→ human/AI Career review
→ optional Career update
```

Career should not depend directly on JobHunter's internal SQLite tables or UI markup.

The bridge should support reproducible snapshot references so a later Career review can determine what evidence produced an earlier decision.

## 19. Review cadence

Do not create market-analysis bureaucracy merely because JobHunter can automate it.

Use JobHunter:

- when a scheduled Career market/review decision needs current evidence;
- before meaningful role-strategy changes;
- before application activation;
- during active applications for vacancy-specific analysis;
- when repeated job/interview feedback suggests the market model is wrong;
- when enough new evidence exists to make a prior snapshot stale.

A dashboard changing every day does not require a Career commit every day.

## 20. First practical Career use

Before relying on advanced personal recommendations, the first useful sequence is:

```text
1. validate JobHunter source/translation/analysis quality on reviewed jobs
2. accumulate a representative sample for selected role families
3. produce a first Market Evidence Snapshot
4. manually review representative postings and aggregates
5. compare recurring requirements/responsibilities with the Career evidence ledger
6. record only the resulting Career conclusions
```

This creates value before every future JobHunter feature exists.

## 21. Success condition

This integration is successful when JobHunter helps Career make smaller, better-supported decisions while preserving the distinction between:

- market demand;
- model interpretation;
- Ali's real capability;
- Career judgment.

The system should reduce guesswork without replacing judgment.
