---
name: career-review
description: >
  Run formal or event-triggered Career reviews that may change Career state, strategy, project role/allocation, workload, capability conclusions, portfolio positioning, employability/application readiness, or review triggers. Use when Ali requests a Career review or a repository-defined review trigger occurs. Define the Career question, inspect the minimum current evidence, compose the relevant capability/market/claim procedures, accept no-change as a valid outcome, update only canonical owners, and keep project remediation at macro directive level. Do not use for ordinary project progress, a narrow capability/market/claim question that does not require a Career review, or project implementation/teaching.
compatibility: Designed for the motafegh/Career repository and agents that can inspect Career authorities plus the minimum underlying project or market evidence required by the review question.
---

# Career Review

## Purpose

Conduct a bounded Career-level review that turns current evidence into explicit decisions without recreating project operation or rewriting strategy merely because a review occurred.

This skill orchestrates Career review work. It does not replace the canonical capability, market, portfolio, strategy, state, or project authorities.

A valid review may conclude **no material Career change**.

## Load only the review authorities and evidence you need

1. Follow [`../../../AGENTS.md`](../../../AGENTS.md) and the Career authority order.
2. Read the relevant sections of [`../../../governance/CAREER_OPERATING_CONTRACT.md`](../../../governance/CAREER_OPERATING_CONTRACT.md) for review triggers, Career-to-project handoff, workload, evidence, and change discipline.
3. Read [`../../../CAREER_STATE.md`](../../../CAREER_STATE.md) for the current live Career position and current review triggers.
4. Read [`../../../plans/CURRENT_CAREER_CYCLE.md`](../../../plans/CURRENT_CAREER_CYCLE.md) when the review is scheduled, cycle-related, or may change current-cycle outcomes/allocation.
5. Read the relevant portion of [`../../../tracking/CAREER_REVIEW_LOG.md`](../../../tracking/CAREER_REVIEW_LOG.md) when prior review conclusions or the review record format matter.
6. Load only the domain owners required by the review question: capability ledger, market plan/evidence, portfolio record, strategy, profile, CV/claim records, or workload evidence as applicable.
7. Inspect the minimum underlying project or external evidence needed to answer the Career question. Do not re-open a whole project repository when a registered handoff or exact evidence package is sufficient.

## Review workflow

### 1. Identify the trigger and Career question

State why the review is happening and what Career-level decision is actually at issue.

Valid triggers include repository-defined scheduled/event triggers and Ali's explicit request for a Career review.

Examples:

- Has returned project evidence changed the current implementation-ownership conclusion?
- Is normal application readiness now supportable?
- Should a project's Career role or allocation change?
- Has current market evidence materially changed role priorities?
- Is the current workload model still sustainable?

Do not turn an ordinary project commit into a Career question merely because new work exists.

### 2. Define the minimum evidence package

Before loading files or tools, identify what evidence is necessary to answer the question and what would be irrelevant.

Distinguish:

- current evidence from stale evidence;
- project/product progress from Ali capability;
- Career-facing evidence from project-local continuation;
- market observation from Ali-specific evidence;
- proposed claims from demonstrated ownership.

Prefer the smallest sufficient evidence package over broad repository rereading.

### 3. Apply the relevant specialist procedure

Use the appropriate Career procedure for each material sub-question rather than improvising a new standard inside the review.

Examples:

- capability/ownership question → use the canonical capability-evidence model and capability-assessment procedure;
- market pattern/question → use the canonical market-evidence method and market-calibration procedure;
- external wording/portfolio claim → use claim-evidence and assistance boundaries rather than promotional judgment;
- project-role/admission question → use the controlling portfolio policy;
- workload question → use the operating contract and actual bounded workload evidence.

Do not duplicate those specialist standards inside the review record.

### 4. Determine what changed and what did not

For each review domain, explicitly classify:

- material conclusion changed;
- confidence/transfer limit changed but headline conclusion did not;
- evidence improved without yet crossing the decision threshold;
- evidence weakened/staled enough to narrow a current claim;
- no material change;
- unresolved because evidence is insufficient.

A review is not required to generate a new strategy, identity, project, plan, or document.

### 5. Choose the smallest justified Career correction

When evidence supports change, prefer the minimum correction that solves the Career problem.

Possible changes include:

- update one capability record;
- adjust a claim boundary;
- change application-readiness status;
- adjust project role/allocation;
- revise a capability priority;
- change workload mode/ceiling;
- revise role/geographic emphasis;
- change the next review trigger.

Do not rewrite unrelated Career architecture around one finding.

### 6. Preserve the Career-to-project boundary

When a project-addressable gap is identified, Career may define:

- the required outcome;
- evidence class;
- claim boundary;
- allocation ceiling;
- acceptance condition;
- reassessment trigger.

Do **not** prescribe the project's exact source file, function, test, command, lesson, debugging sequence, implementation method, or project-local plan unless such detail is itself necessary to define a Career-facing acceptance criterion.

Project repositories decide how to satisfy the Career directive.

### 7. Update only canonical owners

If the review changes a material Career truth, update only the files that own that truth.

Typical owners include:

- `CAREER_STATE.md` for live Career position and exact next Career action;
- capability ledger for capability conclusions;
- project portfolio/project record for project role or claim boundaries;
- market artifacts/plan for reviewed market conclusions where appropriate;
- strategy only for material strategy changes;
- current cycle only for current-cycle outcome/allocation/review changes.

Link rather than duplicate.

Do not update files just to prove the review happened.

### 8. Record the review proportionately

When repository governance requires a formal/event-triggered review record, add the Career-level question, evidence inspected, conclusions/decisions, assistance/transfer limits where material, and next trigger to the canonical review log.

Do not copy detailed project evidence, technical continuation, or long source summaries into the review log.

A light pulse or conversational check does not need a repository entry unless a material Career fact or decision changed.

### 9. Set the next trigger

Every consequential review should end with a clear next reassessment condition or scheduled trigger.

Prefer event-based triggers when meaningful evidence may arrive before a calendar date. Preserve mandatory calendar reviews where the current cycle requires them.

Do not leave a bounded hold open-ended.

## Invalid shortcuts

Never use these shortcuts:

- review happened = something must change;
- project progress = capability progress;
- more documentation = stronger evidence;
- one vacancy = strategy change;
- one failed session = flagship failure;
- one interesting technology = new working identity;
- capability gap = Career should design the project lesson;
- stale state = rewrite every downstream file;
- no change = failed review.

## Output

Keep the review proportional to its scope.

For a formal review, summarize when relevant:

- Trigger
- Career question
- Evidence inspected
- Project contribution conclusion
- Capability conclusion
- Assistance/transfer limits
- Workload decision
- Portfolio decision
- Role/market/application decision
- Claim changes
- Career state changes
- What did not change
- Next review trigger

Use only the fields relevant to the actual review.

## Final checks

Before finalizing, verify that:

- the review had a real Career trigger/question;
- only the minimum relevant evidence was loaded;
- specialist evidence standards were respected rather than reinvented;
- project progress was not converted into Ali capability;
- no-change was allowed where evidence supported no change;
- any correction was the smallest justified one;
- project-addressable gaps were handed off at macro level;
- only canonical truth owners were updated;
- the next trigger is explicit where the review is consequential;
- public Career records remain public-safe.
