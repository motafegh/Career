---
name: career-market-calibration
description: >
  Evaluate current vacancy and job-market evidence for Career decisions. Use when deciding what employers appear to require, whether a JobHunter snapshot or public role sample establishes a repeated market pattern, whether role/geography/capability priorities should change, or what one vacancy versus a broader sample actually proves. Preserve source and sample scope, freshness, duplicate treatment, search-selection bias, and required/preferred/contextual/inferred distinctions. Do not use for JobHunter implementation, Ali capability assessment, CV wording, or generic job collection with no Career interpretation.
compatibility: Designed for the motafegh/Career repository and agents with access to current public vacancy evidence or reviewed JobHunter Career-facing artifacts when the decision depends on them.
---

# Career Market Calibration

## Purpose

Turn current vacancy evidence into a bounded Career-level market conclusion without allowing one listing, a biased search, derived model output, or a large opaque corpus to masquerade as neutral labor-market truth.

This skill defines the market-calibration procedure. It does **not** own Career strategy, Ali capability, JobHunter implementation, or current Career state.

## Load only the controlling context you need

1. Follow [`../../../AGENTS.md`](../../../AGENTS.md) and the Career authority order.
2. Read the relevant sections of [`../../../market/EMPLOYABILITY_AND_MARKET_PLAN.md`](../../../market/EMPLOYABILITY_AND_MARKET_PLAN.md) for the canonical market-evidence and requirement-to-evidence method.
3. When JobHunter evidence is involved, read the relevant sections of [`../../../market/jobhunter/CAREER_INTEGRATION_AND_USE.md`](../../../market/jobhunter/CAREER_INTEGRATION_AND_USE.md). Treat JobHunter as an evidence instrument, not an automatic Career authority.
4. Read [`../../../CAREER_STATE.md`](../../../CAREER_STATE.md), [`../../../strategy/CAREER_STRATEGY.md`](../../../strategy/CAREER_STRATEGY.md), or a prior market baseline only when the market conclusion could change or compare against those Career-owned decisions.
5. Inspect the smallest sufficient original or reviewed market evidence. For material or surprising conclusions, preserve a path back to representative employer-authored source evidence.

For current laws, visa rules, salaries, hiring practices, active vacancies, or other time-sensitive market facts, verify current public information before deciding.

## Calibration workflow

### 1. State the Career market question

Define what the evidence is supposed to answer before collecting or interpreting jobs.

Examples:

- Is SQL recurring strongly enough in current junior data roles in the UAE to remain a material Career priority?
- Does this one vacancy plausibly fit Ali's current target band?
- Has the current role sample changed enough to reconsider primary role emphasis?

Do not begin with a technology you want to justify.

### 2. Match evidence strength to decision consequence

Use the consequence/gate model in the Career JobHunter integration contract when applicable.

A single vacancy can answer an employer-specific question. A repeated market pattern needs multiple distinct current jobs and visible sample context. A material strategy, application-readiness, geographic, cycle, or project-allocation change requires stronger evidence plus the relevant Career context.

Do not demand a large sample for a narrow employer question, and do not use a narrow sample for a broad market claim.

### 3. Define the sampling frame

Before interpreting frequency, establish the relevant scope where available:

- role family or search profile;
- seniority/entry band;
- geography;
- work mode;
- time window/freshness;
- sources searched;
- search terms or selection method;
- inclusion/exclusion rules.

A conclusion is only as broad as this frame permits.

### 4. Inspect source quality and sample composition

Identify, where material:

- distinct jobs rather than raw result count;
- duplicate/repost treatment;
- company or source concentration;
- missing/inaccessible descriptions;
- stale or closed postings;
- native versus translated evidence;
- search or catalog changes that could create apparent trends.

Prefer diversity across companies and source types over many near-duplicate postings.

### 5. Control search-selection bias

Ask explicitly:

- Did the acquisition method search for the same technology or title later claimed to be common?
- Is the sample intentionally targeted rather than neutral?
- Are compared role families/geographies using materially comparable search methods?
- Did one source, company, recruiter, or search profile dominate the result?

If the sample is targeted, describe conclusions as targeted-sample findings. Do not relabel them as the neutral technology market.

### 6. Keep evidence layers separate

Preserve distinctions among:

- employer-authored source evidence;
- deterministic parsing;
- translation;
- semantic/model interpretation;
- taxonomy normalization;
- aggregate calculation;
- Ali-specific Career comparison.

Do not aggregate model-inferred requirements as though they were employer-explicit requirements. Do not present translated text as employer-authored wording.

### 7. Analyze responsibilities, not keyword counts alone

For each material pattern, ask what work the employee is expected to perform and what depth/ownership the wording implies.

Distinguish:

- required versus preferred versus contextual mentions;
- tools/frameworks versus underlying responsibilities;
- role purpose and deliverables versus incidental technology names;
- hard eligibility constraints versus technical requirements.

A technology mention does not by itself establish that the technology is central to the role.

### 8. Quantify only as strongly as the denominator allows

When reporting recurrence, preserve the denominator and sample boundary.

Good:

> SQL was explicitly required or strongly expected in 14 of 18 distinct current postings in this bounded UAE junior Python/data sample.

Bad:

> 78% of junior tech jobs require SQL.

Do not claim population-level frequency from a convenience or targeted sample unless the sampling design supports it.

### 9. Separate market evidence from Ali capability

Market evidence answers what employers appear to want. It does not establish what Ali can currently defend.

If an Ali-specific gap comparison is needed, use Career-approved capability evidence and assistance/transfer limits. Do not infer capability from GitHub ownership, project technology stacks, or JobHunter implementation.

A common requirement may justify capability prioritization without becoming a demonstrated skill claim.

### 10. Choose the smallest justified Career implication

Possible results include:

- exploratory observation only;
- repeated pattern worth monitoring;
- capability priority remains justified;
- capability priority should increase/decrease;
- one role family appears more/less plausible;
- vacancy-specific application review is justified;
- sample is too biased or weak to change Career;
- material Career review is warranted.

Do not automatically start a project, change identity, add a technology to a project, or activate applications because one skill appears in the market sample.

### 11. State limits and refresh conditions

Record the important non-conclusions:

- what geographies/roles were not sampled;
- source or search bias;
- small or uneven sample;
- missing data;
- derived/model uncertainty;
- freshness limits;
- eligibility unknowns.

State when the evidence should be refreshed or what stronger sample would be needed for a broader decision.

### 12. Persist only when a Career decision requires it

Do not edit Career strategy, state, capability priorities, portfolio allocation, or market records merely because this skill produced an observation.

Persist a market conclusion only when Ali explicitly asks to record/update it or an active Career review/decision procedure requires canonical persistence under repository governance. Update only the file that owns the changed Career truth. If the evidence does not materially change a Career conclusion, preserve existing canonical records.

## Invalid shortcuts

Never use these shortcuts:

- one vacancy = market trend;
- many duplicates = representative sample;
- targeted search prevalence = neutral market prevalence;
- LLM-inferred requirement = employer-required requirement;
- tool mention = core responsibility or required depth;
- current bounded sample = universal labor market;
- market demand = Ali capability;
- market demand = automatic project/technology admission;
- old posting = current market evidence;
- large JobHunter corpus = automatic Career authority.

## Output

Keep the output proportional to the question. For a material market-calibration result, include when relevant:

- Career market question
- Sample/scope and freshness
- Sources/search method
- Distinct-job and duplicate treatment
- Strongest recurring responsibilities/requirements
- Required/preferred/contextual/inferred separation
- Representative source evidence
- Search-selection and data-quality limits
- Career implication
- What the evidence does not justify
- Refresh/reassessment trigger

If the evidence is too weak or biased for the requested conclusion, say so and identify the smallest additional evidence needed. Do not manufacture certainty from volume.

## Final checks

Before finalizing, verify that:

- the market question was defined before the conclusion;
- the conclusion is no broader than the sampling frame;
- duplicate/repost and source concentration were considered where material;
- search-selection bias was considered;
- employer-explicit and model-derived evidence were not silently merged;
- market evidence and Ali capability remained separate;
- time-sensitive facts are current enough for the decision;
- the Career implication is the smallest one justified by the evidence;
- JobHunter output did not overwrite Career authority automatically;
- no Career record was changed merely because the skill ran.
