# Agent Instructions — Career

## Purpose

Operate this repository as Ali Rajabi's durable, public-safe career operating system.

Career is broader than one project or one 90-day cycle. It governs Ali's professional profile, strategy, project portfolio, capability evidence, employability, market transition, workload, reviews, and long-term decisions.

Do not operate UpgradePilot, JobHunter, or any other technical project from Career.

## Instruction precedence

When instructions conflict, use:

1. safety, legal, privacy, credential, financial, health, cost, and platform constraints;
2. Ali's explicit current instruction;
3. [`CAREER_CHARTER.md`](CAREER_CHARTER.md);
4. [`governance/CAREER_OPERATING_CONTRACT.md`](governance/CAREER_OPERATING_CONTRACT.md);
5. applicable Career strategy and portfolio policy;
6. [`plans/CURRENT_CAREER_CYCLE.md`](plans/CURRENT_CAREER_CYCLE.md);
7. [`CAREER_STATE.md`](CAREER_STATE.md) for live career position;
8. the canonical capability, portfolio, market, or review record for the question;
9. AI suggestions.

A lower-level file may add detail but may not silently change a higher authority.

## Single live-state owner

`CAREER_STATE.md` is the only Career file permitted to state the live career position and exact next career-level action.

It owns:

- current career cycle;
- working identity;
- active project allocation;
- current capability and employability emphasis;
- current workload decision;
- current portfolio phase;
- material career-level risks;
- exact next Career action;
- next review trigger.

Do not duplicate these status statements across strategy, portfolio, market, capability, or review files.

Do not put UpgradePilot or JobHunter technical next actions in `CAREER_STATE.md`.

## Truth routing

| Question | Owner |
|---|---|
| Durable Career mission and repository boundary | `CAREER_CHARTER.md` |
| Current career position and next Career action | `CAREER_STATE.md` |
| Public-safe facts about Ali | `profile/CAREER_PROFILE.md` |
| Direction, roles, priorities, geography, and change logic | `strategy/CAREER_STRATEGY.md` |
| Workload, reviews, allocation, and anti-diversion rules | `governance/CAREER_OPERATING_CONTRACT.md` |
| Current bounded career-cycle outcomes | `plans/CURRENT_CAREER_CYCLE.md` |
| Project roles and career contribution | `portfolio/PROJECT_PORTFOLIO.md` and project records |
| New-project admission or retirement | `strategy/PROJECT_PORTFOLIO_AND_SELECTION_POLICY.md` |
| Cross-project capability evidence | `tracking/CAPABILITY_EVIDENCE_LEDGER.md` |
| Employability and market transition | `market/EMPLOYABILITY_AND_MARKET_PLAN.md` |
| Career-facing JobHunter requirements and use rules | `market/jobhunter/CAREER_REQUIREMENTS.md` and `market/jobhunter/CAREER_INTEGRATION_AND_USE.md` |
| Career review decisions | `tracking/CAREER_REVIEW_LOG.md` |
| UpgradePilot current technical continuation | UpgradePilot `MEMORY.md` |
| UpgradePilot implemented behavior | UpgradePilot source, tests, commands, outputs, and environment |
| JobHunter current technical continuation and implementation | `motafegh/jobhunter` source, tests, plans, evidence, database/runtime, and project-local docs |

One kind of truth should have one normal owner. Link rather than duplicate.

## Career responsibilities

Career owns:

- honest public-safe profile and current professional state;
- long-term and current career direction;
- role, location, and work-mode targeting;
- current cycle and workload commitments;
- project portfolio roles and allocation;
- formal capability assessment and transfer limits;
- portfolio claims and professional positioning;
- application-readiness and market strategy;
- Career-facing market-intelligence requirements and review rules;
- formal and event-triggered reviews;
- cycle-to-cycle continuity.

Career does not own:

- project live state or exact next actions;
- project routes, milestones, sessions, or blockers;
- source, tests, specifications, ADRs, dependencies, or implementation;
- ordinary project learning decisions;
- detailed project evidence, databases, runtime artifacts, or working memory.

## Career review behavior

A Career review may be scheduled, user-requested, or event-triggered.

Before reviewing:

1. state the career-level question;
2. identify the minimum project or market evidence needed;
3. inspect actual source, tests, evidence, or external requirements as appropriate;
4. distinguish project progress from Ali capability;
5. distinguish current evidence from stale evidence;
6. record only career-level conclusions.

A review may update:

- `CAREER_STATE.md`;
- capability records;
- project portfolio roles or claims;
- workload decision;
- role or geographic strategy;
- market/application phase;
- current career-cycle outcomes;
- next review trigger.

Do not copy project continuation into Career.

## Capability assessment

Assess specific responsibilities, not broad technology names.

Never infer ownership from:

- exposure;
- documentation;
- repository size;
- successful commands;
- immediate repetition;
- reading and agreeing with code;
- AI-generated implementation;
- passing AI-generated tests;
- one guided case.

Record:

- evidence;
- assistance;
- date and recency;
- confidence;
- transfer limit;
- next reassessment.

Use changed-case, failure, delayed, and reduced-prompt evidence when stronger claims require it.

## Project portfolio behavior

- One primary flagship is the default.
- Supporting projects need a named career gap and bounded allocation.
- Experiments need a question, ceiling, and stop condition.
- Historical projects remain inactive unless Career explicitly assigns a bounded role.
- Do not revive Sentinel or AegisLab because their repositories exist.
- Do not start another major project to escape a difficult UpgradePilot responsibility.
- Do not import project architecture across repositories without a current justified need.
- A career-support tool such as JobHunter is not automatically a learning or portfolio project; treat its implementation as capability evidence only after explicit assessment.

## Employability behavior

Connect capability and portfolio evidence to representative real roles.

Do not:

- claim readiness from project branding;
- wait for total mastery before market calibration;
- create application bureaucracy before application activation;
- write inflated resumes or project claims;
- ignore assistance and transfer limits;
- turn one job description into a new curriculum;
- treat a narrowly searched JobHunter sample as the neutral technology market;
- allow JobHunter output to overwrite Career decisions automatically.

Use representative samples, identify common requirements, map evidence and gaps, and update strategy only from material patterns or feedback.

When JobHunter is used, follow [`market/jobhunter/CAREER_INTEGRATION_AND_USE.md`](market/jobhunter/CAREER_INTEGRATION_AND_USE.md): preserve source/sample context, distinguish employer evidence from translation/model/taxonomy output, and use Career-approved personal capability evidence for Ali-specific comparisons.

For current laws, job-market conditions, role requirements, companies, salaries, visa rules, or hiring practices, verify current public information before making decisions.

## Advanced capability exposure

Advanced systems remain legitimate interests, but no technology quota may force artificial architecture.

Require a career or project question, a simpler baseline, bounded evidence, costs, failure modes, and an adopt/pilot/reject/defer result.

Exposure is not ownership. A project-integrated pilot is not professional mastery.

## Document discipline

Before editing or creating a Career file, ask:

1. Is this a career-level responsibility?
2. Which file owns this truth?
3. Did a material career fact or decision change?
4. Would this fact change after an ordinary project session?
5. Is the content public-safe?
6. Can an existing file hold it without ambiguity?

If an ordinary project event would change the fact, it usually belongs in the project repository.

Use Git history as the default archive. Do not keep compatibility pointers or historical templates without a current need.

## Security and privacy

- Keep all Career records public-safe.
- Do not expose medical, medication, legal, financial, credential, address, phone, private family, or private routine details.
- Do not store confidential applications, recruiter messages, or employer correspondence in the public repository.
- Do not publish personal contact details merely for portfolio completeness.
- Sanitize linked project evidence and market records.
- Preserve uncertainty and limitations.

## Refoundation status

The Career repository refoundation completed on 2026-07-27.

`CAREER_REPOSITORY_REFOUNDATION_PLAN.md` is a completed transformation and audit record, not an active source of routine tasks.

Do not recreate removed compatibility routes, project-specific Career trackers, AegisLab reporting templates, or UpgradePilot technical evidence in Career.

The next Career action is owned by `CAREER_STATE.md`.
