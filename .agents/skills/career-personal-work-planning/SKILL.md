---
name: career-personal-work-planning
description: >
  Create Ali-facing personal work plans for the next session, day, week, or month from current Career priorities, workload/capacity, review gates, and the active project's authoritative live continuation. Use when Ali asks what he should personally focus on or work on next, especially when translating current project state into Career-aligned outcomes. Preserve project-owned technical routes, use rolling-wave planning across unresolved gates, and never manufacture capability evidence. Do not use for direct state lookups, project implementation/design/teaching, capability assessment, market analysis, claim audit, or formal Career review.
compatibility: Designed for the motafegh/Career repository and agents that can inspect Career authorities plus the active project's authoritative governance and live continuation when project-grounded planning is requested.
---

# Career Personal Work Planning

## Purpose

Create a practical plan for **Ali's personal work and attention** at Career level.

The skill answers:

> Given Career's current priorities and constraints, plus the authoritative live state of the active project, what should Ali personally focus on during the requested horizon?

It does **not** become the active project's implementation, learning, debugging, or technical-planning authority.

Use the separation:

```text
Career
→ why the work matters
→ personal outcome / priority / capacity / evidence opportunity / gate

active project
→ exact technical continuation
→ implementation / learning / source / tests / commands / proof sequence
```

Project details may be shown as **read-through project state** so the personal plan is usable. They remain project-owned instructions.

## 1. Establish the planning horizon and decision boundary

Identify the requested horizon:

- next session;
- rest of today / next day;
- next week;
- month or longer bounded period.

Also identify any current Career or project decision gate that occurs inside that horizon.

Use rolling-wave planning:

```text
near-term state is known
→ plan concretely

future work depends on an unresolved gate
→ stop detailed planning at the gate
→ make later outcomes conditional
```

Never plan through an unresolved formal Career review, project disposition, major blocker, or other decision boundary as if its result were already known.

## 2. Load the minimum Career context

Follow [`../../../AGENTS.md`](../../../AGENTS.md) and Career's authority order.

Normally inspect only what the personal plan needs:

1. [`../../../CAREER_STATE.md`](../../../CAREER_STATE.md) — live Career position, active allocation, exact Career action, risks, and review triggers.
2. [`../../../plans/CURRENT_CAREER_CYCLE.md`](../../../plans/CURRENT_CAREER_CYCLE.md) — current bounded outcomes, allocation principles, and scheduled gates when the horizon reaches them.
3. [`../../../governance/CAREER_OPERATING_CONTRACT.md`](../../../governance/CAREER_OPERATING_CONTRACT.md) — workload/capacity, Career-to-project boundary, anti-diversion, and proportionality.
4. The active Career directive/plan only when it materially affects the requested horizon.
5. Capability, market, portfolio, or claim records only when a current recorded conclusion is necessary to choose personal priorities.

Do not reread the whole Career repository merely because planning is requested.

## 3. Read the active project's continuation without taking ownership of it

When the plan is grounded in an active technical project:

1. identify the current project from Career's live state;
2. read that project's root governance first;
3. read the project's canonical live-state / continuation owner;
4. follow only the currently selected plan, learning map, working-memory handoff, or other owner needed to understand the immediate route;
5. inspect source/tests only when their actual size, complexity, learning burden, proof obligation, or current failure materially affects the personal plan.

For current UpgradePilot operation, its root `AGENTS.md` defines project routing and `MEMORY.md` owns live continuation. Follow whatever those authorities currently select rather than reconstructing the route from historical plans or broad repository search.

Do not copy the active project's TODO, plan, source-study sequence, implementation steps, commands, tests, or working memory into Career as a new owner.

## 4. Translate project continuation into Ali-facing outcomes

Start from the legitimate project route and ask what Ali should personally gain from it.

A useful personal outcome may concern:

- understanding/tracing a current responsibility;
- reasoning, prediction, challenge, or design judgment;
- representative test/proof interpretation;
- meaningful direction or modification when the project naturally reaches it;
- diagnosis when a real relevant failure occurs;
- explanation/ownership transfer;
- portfolio or market-facing Career work when Career currently requires it.

Prefer **1–3 personal outcomes** for a normal session/day.

For each selected outcome, state briefly:

```text
what Ali should get from the work
why it matters now
which current Career priority it serves
which project-owned continuation it relies on, when applicable
what nearby work should remain deferred
```

Do not turn a Career capability gap into an artificial project exercise.

## 5. Respect capacity rather than filling time

Treat Career workload values as ceilings/capacity containers, not quotas.

If Ali has limited time or reduced capacity:

```text
choose the smallest high-value outcome
→ keep the project stop line intact
→ add secondary work only if the primary outcome closes naturally
```

Do not compress a full normal workday into a short session.

Do not extend work merely to consume the available hours.

For a normal day, prefer:

```text
PRIMARY
→ the outcome that makes the day worthwhile

SECONDARY
→ only if primary closes naturally and capacity remains

OPTIONAL
→ only if still aligned and no stronger gate/priority appears
```

## 6. Do not manufacture Career evidence

Career may want stronger evidence in several capability classes. A personal plan must not force the active project to generate each class immediately.

Never instruct Ali or the project to manufacture:

- fake failures for debugging evidence;
- arbitrary source changes for modification evidence;
- detached exercises solely to satisfy a Career checklist;
- unnecessary technologies for résumé breadth;
- repeated or memorization-heavy work that the project does not currently justify.

Instead:

```text
legitimate current project opportunity
→ use it well
→ preserve relevant evidence if it naturally occurs

missing evidence class with no legitimate current opportunity
→ leave it open
→ revisit when real project work produces the opportunity or Career formally changes the directive
```

## 7. Scale detail by horizon

### Session

Most concrete. Usually include:

- Career purpose;
- project-owned starting point;
- 1–3 personal outcomes;
- focus/deferred depth;
- evidence worth noticing;
- stop condition;
- return-to-Career trigger when material.

### Day

Prioritize primary / secondary / optional outcomes. Avoid minute-by-minute scheduling unless Ali explicitly requests calendar-style planning and it is useful.

### Week

Plan a small set of outcomes across current Career lanes and capacity. Preserve the flagship's dominant allocation when Career currently requires it. Name what is intentionally deferred. Do not create seven technical daily plans by default.

### Month or longer

Use high-level outcomes, allocation, known review gates, and conditional branches. Do not predict detailed project implementation far beyond current authoritative continuation.

The farther the horizon, the less technical detail the Career plan should own.

## 8. Route material decisions to the correct Career skill/owner

Personal planning consumes current Career decisions; it does not silently make new material ones.

If planning exposes an unresolved material Career decision such as application readiness, project reclassification, major allocation change, workload-model change, or strategy change:

```text
stop detailed planning through that decision
→ use [`../career-review/SKILL.md`](../career-review/SKILL.md) when a formal/event-triggered review is warranted
→ resume planning from the resulting Career decision
```

If the user's actual question is instead:

- "What have I demonstrated?" → [`../career-capability-assessment/SKILL.md`](../career-capability-assessment/SKILL.md);
- "What does the market evidence establish?" → [`../career-market-calibration/SKILL.md`](../career-market-calibration/SKILL.md);
- "What may I truthfully say externally?" → [`../career-claim-audit/SKILL.md`](../career-claim-audit/SKILL.md);
- "What is the exact current Career action/state?" → read the canonical owner directly; no planning procedure is needed.

Do not load these sibling skills merely because they exist. Compose only when their responsibility is materially part of the request.

## 9. Persistence boundary

The normal output is the plan in conversation.

Session/day plans are chat-first by default. Weekly/monthly plans are also chat-first in v1 unless Ali explicitly requests a durable artifact or a material Career decision requires an existing canonical owner to change.

Do not create a new rolling live-state or personal-plan file merely because planning occurred.

If Ali explicitly requests a durable Career planning artifact, first verify that:

- the content is genuinely Career-level;
- an existing canonical Career owner cannot hold the durable decision more clearly;
- volatile project continuation is referenced rather than duplicated;
- the artifact will not become a second live-state owner.

Planning alone does not authorize changes to the active project repository.

## 10. Output discipline

Keep personal plans practical and compact.

A normal plan should make these recoverable at a glance:

```text
HORIZON
why this period matters

STARTING POINT
current Career priority + project-owned continuation

PERSONAL OUTCOMES
1–3 outcomes, ordered

FOCUS / DEFER
what matters now and what should wait

CAPACITY
only when relevant

STOP / GATE
when to stop or where the plan becomes conditional

RETURN TO CAREER
only when a review/evidence/decision trigger is material
```

Do not pad the plan with generic productivity advice, repeated governance summaries, or technical details owned by the project.

## Completion check

Before returning the plan, verify:

- it is grounded in current Career state rather than stale history;
- active-project continuation came from that project's authoritative owner;
- project details are read-through context, not Career-owned technical instructions;
- the plan contains a small number of meaningful personal outcomes;
- available capacity is treated proportionately;
- unresolved gates stop or conditionalize farther planning;
- no evidence, failure, implementation change, or technology was manufactured for Career;
- the plan did not silently perform a Career review;
- volatile session/day planning was not persisted by default.

If those conditions hold, return the plan and stop.