# Career Repository Refoundation Plan

**Owner:** Ali Rajabi  
**Prepared:** 2026-07-27  
**Status:** Proposed; requires Ali review and explicit approval before execution  
**Scope:** `motafegh/Career` only  
**Implementation boundary:** This plan does not itself authorize changes to any existing Career file. It does not modify UpgradePilot.

## 1. Executive decision

The Career repository should be transformed from a narrow 90-day UpgradePilot review layer into Ali's durable, personalized career operating system.

The correct separation remains:

```text
Career
= Ali's career direction, profile, capability evidence, project portfolio,
  employability, market transition, workload, reviews, and long-term decisions

UpgradePilot
= the product mission, technical route, live project state, source, tests,
  specifications, ADRs, working evidence, and exact technical continuation
```

The current separation between the repositories is valid and must be preserved. The required correction is not to move UpgradePilot operation back into Career. The correction is to restore the broader Career responsibilities that were lost when Career was aggressively reduced to formal reviews and 90-day controls.

The refounded repository must help answer, at any meaningful point:

1. Who is Ali professionally now?
2. What long-term direction is being pursued?
3. What current career cycle is active?
4. Which projects exist, and what career role does each serve?
5. What capability has actually been demonstrated?
6. What remains AI-dependent, unassessed, or weak?
7. How employable is Ali for the current target roles?
8. What portfolio evidence and claims are defensible?
9. What market, application, and interview work is active or pending?
10. What is the next career-level action or review trigger?

## 2. Current-state diagnosis

### 2.1 What is correct now

- UpgradePilot has become an independent technical repository.
- Career no longer duplicates project sessions, technical plans, blockers, source, tests, ADRs, or exact next actions.
- Career preserves a realistic working identity and conservative capability claims.
- The repository contains useful workload, security, learning-style, project-selection, capability, and advanced-exposure material.
- Career correctly distinguishes project progress from personal capability.

### 2.2 What is missing or over-narrowed

Career currently behaves mainly as:

- a 90-day execution contract;
- an UpgradePilot allocation record;
- a coarse formal-review store;
- a conservative capability-assessment record.

That is insufficient for the original mission. Missing or underdeveloped responsibilities include:

- a durable career charter beyond one 90-day period;
- one live career-state owner;
- an active public-safe personal career profile;
- complete project-portfolio governance;
- cross-project capability evidence;
- employability and role-gap analysis;
- portfolio and professional-presence development;
- job-search, application, and interview transition planning;
- long-term cycle-to-cycle continuity;
- event-triggered career decisions outside fixed formal reviews;
- explicit evaluation of whether current work is improving employability.

### 2.3 Main structural risk

The previous correction solved duplication by making Career passive. The new design must avoid both extremes:

```text
Wrong extreme A:
Career operates UpgradePilot and duplicates project truth

Wrong extreme B:
Career becomes a static archive that rarely helps Ali navigate his future

Required balance:
Career actively governs career-level truth and decisions,
while project repositories own technical operation
```

## 3. Target mission of the Career repository

The Career repository will be Ali's durable, public-safe career-management system.

Its mission is to:

> Maintain an honest model of Ali's current professional state, direct capability-building and project allocation toward realistic employment, preserve evidence and assistance boundaries, govern the portfolio and market transition, and support repeated career cycles without duplicating project operation.

The repository must support both:

```text
durable multi-year career direction
+
current bounded execution cycle
```

The current 2026-07-20 to 2026-10-17 cycle remains important, but it must no longer define the entire identity of the repository.

## 4. Non-goals

The refoundation must not:

- restore UpgradePilot's live route, `MEMORY.md`, plans, source, tests, ADRs, blockers, or session logs into Career;
- update Career after every project commit, test, or sub-gate;
- create a second technical tracker for UpgradePilot;
- create daily bureaucracy or duplicate project worklogs;
- claim that repository documentation proves Ali's capability;
- expose medical, medication, financial, credential, or private-routine details;
- turn Career into a generic motivational journal;
- create a fixed technology checklist disconnected from employment or project evidence;
- require all future projects to use one architecture or learning sequence;
- treat the current 90-day identity as a permanent final career identity;
- create application trackers before the application phase is actually activated;
- create multiple files that own the same live state.

## 5. Design principles

### 5.1 Ali-centered, not project-centered

UpgradePilot is the current flagship, but Career is about Ali's complete future. The repository must remain useful when UpgradePilot ends, changes, succeeds, or fails.

### 5.2 One owner per kind of truth

Each important question must have one normal owner. Other files link to it rather than repeating status.

### 5.3 Evidence over optimism

Capability, employability, ownership, and role-readiness claims require specific evidence, assistance labels, recency, and transfer limits.

### 5.4 Project progress is not capability progress

A sophisticated repository or passing test can establish product progress without establishing independent Ali capability.

### 5.5 Active but proportional Career management

Career should change when a career-level fact or decision changes, not after every technical event.

### 5.6 Durable profile plus current state

Stable personal and strategic facts belong in durable files. Current position and next career action belong in one live state file.

### 5.7 Market connection

Career planning must connect learning and projects to real role requirements, portfolio claims, applications, and feedback.

### 5.8 Public-safe by construction

Only public-safe personal and professional information belongs in the public repository. Sensitive context may inform decisions externally but must not be copied into GitHub.

### 5.9 Lean authority

A file must exist because it owns a durable responsibility. No file should exist merely because a complete system could theoretically have it.

### 5.10 Git history is the default archive

Do not preserve every superseded document in an active `archive/` tree. Git history already preserves removed content. Keep explicit historical files only when they remain useful evidence or orientation.

## 6. Target truth-routing model

| Question | Canonical owner after refoundation |
|---|---|
| What is the Career repository for? | `CAREER_CHARTER.md` |
| What is Ali's current career position and next career-level action? | `CAREER_STATE.md` |
| What public-safe facts describe Ali, his experience, constraints, strengths, and gaps? | `profile/CAREER_PROFILE.md` |
| What is the long-term direction, target roles, priority capability stack, and decision logic? | `strategy/CAREER_STRATEGY.md` |
| What rules govern workload, reviews, changes, and anti-diversion behavior? | `governance/CAREER_OPERATING_CONTRACT.md` |
| What does the current bounded career cycle require? | `plans/CURRENT_CAREER_CYCLE.md` |
| Which projects exist and what career role does each serve? | `portfolio/PROJECT_PORTFOLIO.md` |
| How are future projects selected, limited, or retired? | `strategy/PROJECT_PORTFOLIO_AND_SELECTION_POLICY.md` |
| What capability has Ali demonstrated across projects? | `tracking/CAPABILITY_EVIDENCE_LEDGER.md` |
| What roles are targeted and what employability gaps remain? | `market/EMPLOYABILITY_AND_MARKET_PLAN.md` |
| What formal or event-triggered Career reviews occurred? | `tracking/CAREER_REVIEW_LOG.md` |
| What current technical work should happen in UpgradePilot? | UpgradePilot `MEMORY.md`, not Career |
| What is actually implemented in UpgradePilot? | UpgradePilot source, tests, commands, outputs, and environment |

## 7. Proposed active repository structure

```text
Career/
├── README.md
├── AGENTS.md
├── CAREER_CHARTER.md
├── CAREER_STATE.md
├── CAREER_REPOSITORY_REFOUNDATION_PLAN.md
├── governance/
│   ├── CAREER_OPERATING_CONTRACT.md
│   └── SECURITY_AND_PRIVACY.md
├── profile/
│   └── CAREER_PROFILE.md
├── strategy/
│   ├── CAREER_STRATEGY.md
│   ├── PROJECT_PORTFOLIO_AND_SELECTION_POLICY.md
│   └── ADVANCED_CAPABILITY_EXPOSURE_POLICY.md
├── plans/
│   └── CURRENT_CAREER_CYCLE.md
├── portfolio/
│   ├── PROJECT_PORTFOLIO.md
│   └── projects/
│       ├── UPGRADEPILOT.md
│       ├── SENTINEL.md
│       └── AEGISLAB.md
├── market/
│   └── EMPLOYABILITY_AND_MARKET_PLAN.md
└── tracking/
    ├── CAPABILITY_EVIDENCE_LEDGER.md
    └── CAREER_REVIEW_LOG.md
```

This is the recommended maximum active structure for the refoundation. Additional files require a demonstrated owner and need.

A job-application tracker, interview tracker, resume package, or networking tracker should be created later only when the relevant phase is activated.

## 8. New root-level files

### 8.1 `CAREER_CHARTER.md`

Create a durable charter that defines:

- repository mission;
- Ali as the owner and primary subject;
- long-term hybrid-engineering direction;
- relationship between career strategy, projects, learning, portfolio, and employment;
- responsibility boundary between Career and project repositories;
- evidence and honesty doctrine;
- public/private boundary;
- what success means across repeated career cycles;
- change-control conditions.

The charter must not contain current project continuation or fixed daily work.

### 8.2 `CAREER_STATE.md`

Create the sole owner of live career position.

It should contain only current career-level facts:

- current career cycle;
- working identity;
- active flagship allocation;
- other project roles;
- current capability-development emphasis;
- current employability phase;
- current portfolio phase;
- current workload decision;
- latest Career-reviewed evidence date;
- current career-level risks;
- exact next career-level action;
- next review trigger.

It must not contain UpgradePilot's technical next action.

Update `CAREER_STATE.md` when a meaningful career-level fact changes, including:

- project allocation;
- career identity or target-role direction;
- material capability assessment;
- workload/capacity decision;
- employability or application phase;
- portfolio claim boundary;
- major project gate that changes career interpretation;
- user-requested Career review;
- next-cycle activation.

Do not update it for ordinary project commits or sessions.

## 9. Existing-file transformation matrix

### 9.1 Root files

| Current file | Proposed action | Result |
|---|---|---|
| `README.md` | Rewrite | Clear public orientation, repository map, start order, current Career state link, and explicit project boundary |
| `AGENTS.md` | Rewrite | Direct AI assistants to Career responsibilities, truth routing, proportional review behavior, and no project-operation duplication |
| `UpgradePilot.md` | Move and refactor | Become `portfolio/projects/UPGRADEPILOT.md`, focused on project career role, evidence contribution, claim limits, and review trigger |
| No current Career charter | Add | `CAREER_CHARTER.md` |
| No current live Career state | Add | `CAREER_STATE.md` |

A temporary compatibility pointer at root `UpgradePilot.md` may be retained during migration only if current links require it. Remove it after link validation unless it remains genuinely useful.

### 9.2 Governance

| Current file | Proposed action | Result |
|---|---|---|
| `governance/90_DAY_EXECUTION_CONTRACT.md` | Refactor and rename | `governance/CAREER_OPERATING_CONTRACT.md`; retain workload and anti-diversion rules while separating durable rules from one cycle's dates |
| `governance/EXECUTION_CONTRACT.md` | Remove compatibility route after link audit | One canonical operating contract |
| `governance/SECURITY_AND_PRIVACY.md` | Retain and enhance | Public-safe profile, project-linking, job-market evidence, contacts, credentials, and sensitive-data rules |

The operating contract should define:

- workload modes and safe capacity;
- review cadence and triggers;
- change-control requirements;
- anti-diversion behavior;
- relationship to project repositories;
- evidence and claim discipline;
- no forced work during unsafe health or personal conditions.

It should not define UpgradePilot sessions or technical commands.

### 9.3 Profile and learning evidence

| Current file | Proposed action | Result |
|---|---|---|
| `strategy/LEARNING_AND_PROJECT_DESIGN_PROFILE.md` | Distill and migrate | Relevant durable content becomes part of `profile/CAREER_PROFILE.md`; obsolete project-selection framing is removed |
| No concise active personal profile | Add | `profile/CAREER_PROFILE.md` |

The active profile should include public-safe sections for:

- current employment and education status;
- prior family-business experience and transferable responsibilities;
- technical exposure and demonstrated evidence;
- current capability limitations;
- career interests and long-term ambition;
- preferred learning and working method;
- AI-assisted work philosophy;
- motivation and execution conditions;
- location and work-mode preferences;
- time availability;
- portfolio assets;
- known career risks;
- facts requiring reassessment.

It must distinguish:

```text
stated preference
observed pattern
preserved evidence
working assumption
unknown or unassessed
```

Sensitive medical and medication details remain outside the public repository.

### 9.4 Strategy

| Current file | Proposed action | Result |
|---|---|---|
| `strategy/STRATEGY_AND_SCOPE.md` | Rewrite and rename | `strategy/CAREER_STRATEGY.md` |
| `strategy/PROJECT_SELECTION_AND_CAPABILITY_SPECIFICATION.md` | Distill and generalize | `strategy/PROJECT_PORTFOLIO_AND_SELECTION_POLICY.md` |
| `strategy/ADVANCED_SYSTEMS_EXPOSURE_AND_ADOPTION_POLICY.md` | Substantially revise | `strategy/ADVANCED_CAPABILITY_EXPOSURE_POLICY.md` |
| `strategy/UPGRADEPILOT_CAPABILITY_AND_PREREQUISITE_SPECIFICATION.md` | Remove from active Career after migration | General capability rules move to `tracking/CAPABILITY_EVIDENCE_LEDGER.md`; UpgradePilot-specific capability detail remains project-local |

#### Career strategy content

The strategy should control:

- long-term direction;
- current working identity;
- target role families;
- geographic and work-mode preferences;
- priority capability stack;
- portfolio strategy;
- market-entry logic;
- decision criteria for changing direction;
- realistic non-claims.

#### Project portfolio and selection policy

This policy should govern:

- primary, supporting, experimental, historical, and retired project roles;
- admission criteria for a new project;
- evidence required to change flagship allocation;
- limits on simultaneous active projects;
- reuse of prior projects;
- project closure and portfolio extraction;
- prevention of technology-collection projects;
- fit with Ali's mission-driven learning mode;
- requirement for a real user, decision, or external objective where appropriate.

#### Advanced capability policy correction

The current policy contains useful A0-A4 distinctions and anti-expansion rules, but its fixed requirement for A1 exposure across six advanced areas plus two A2 pilots can distort the flagship and recreate a technology checklist.

The recommended replacement should:

- retain exposure/adoption level definitions;
- retain baseline, cost, failure, cleanup, and adopt/reject/defer requirements;
- maintain Ali's interest in queues, MLOps, microservices, Kubernetes, cloud, and agent systems;
- replace a mandatory all-six 90-day quota with an evidence-based exposure portfolio;
- let a Career review prioritize areas based on target roles, project need, capacity, and learning value;
- permit later cycles or separate bounded labs when forcing an area into UpgradePilot would be artificial;
- prevent exposure from becoming an unsupported professional claim.

This strategic change must receive explicit Ali approval during implementation.

### 9.5 Current-cycle planning

| Current file | Proposed action | Result |
|---|---|---|
| `plans/90_DAY_CAREER_PLAN.md` | Refactor and rename | `plans/CURRENT_CAREER_CYCLE.md` |

The current cycle plan should include four parallel career tracks:

1. **Flagship delivery** — UpgradePilot remains the primary technical vehicle.
2. **Capability and ownership** — specific responsibilities to strengthen, not broad topic completion.
3. **Portfolio and explanation** — evidence, claims, README quality, demonstrations, and ownership defense.
4. **Employability and market transition** — job evidence, role calibration, resume readiness, applications, and feedback when activated.

The cycle plan should control career-level outcomes and review points. It must not duplicate UpgradePilot's route or next implementation action.

The current dates may remain for this cycle, but the repository must support creating a later cycle without rewriting the durable charter or profile.

### 9.6 Portfolio governance

Add `portfolio/PROJECT_PORTFOLIO.md` as the canonical portfolio register.

Each project entry should record:

- project name and repository;
- current role: primary, supporting, experimental, historical, or retired;
- stable purpose;
- intended career contribution;
- strongest verified evidence;
- assistance and ownership boundary;
- defensible portfolio claims;
- important limitations;
- whether the project deserves further career attention;
- next Career review trigger.

Add concise project records for:

- UpgradePilot;
- Sentinel;
- AegisLab.

These files must not contain technical continuation. They explain each project's career role.

Future project records should be created only when a project receives a defined portfolio role.

### 9.7 Capability and evidence

| Current file | Proposed action | Result |
|---|---|---|
| `tracking/UPGRADEPILOT_EVIDENCE_AND_PROGRESS_TRACKER.md` | Split and replace | Project allocation moves to portfolio; capability conclusions move to capability ledger; review history moves to Career review log |
| UpgradePilot-specific capability specification | Generalize | Cross-project capability and evidence rules become Career-wide |

Create `tracking/CAPABILITY_EVIDENCE_LEDGER.md`.

It should contain:

- the general D0-D5 model or a revised equivalent;
- assessment dimensions: responsibility, evidence, assistance, recency, confidence, transfer limit;
- rules distinguishing exposure, guided application, independent bounded application, ownership, and advanced capability;
- cross-project capability records;
- reassessment triggers;
- portfolio claim boundaries.

Primary capability families should include:

- Python application engineering;
- testing and debugging;
- data acquisition, parsing, validation, and provenance;
- data modeling, persistence, and SQL;
- reproducibility, packaging, CI, and operational engineering;
- deterministic analysis and evaluation;
- ML and AI experimentation;
- secure engineering;
- systems, cloud, and distributed exposure;
- AI-assisted engineering direction, verification, and ownership;
- technical communication and portfolio defense;
- professional execution and collaboration where evidence exists.

Records must assess specific responsibilities, not mark entire technologies complete.

### 9.8 Career review log

Create `tracking/CAREER_REVIEW_LOG.md`.

It should record only career-level review results:

- review date and trigger;
- question being answered;
- project evidence inspected;
- capability conclusions;
- workload decision;
- portfolio decision;
- role or market decision;
- claim changes;
- next review trigger.

Do not copy project continuation or detailed technical state.

Migrate useful conclusions from the existing UpgradePilot Career review record, then remove the old tracker after validation.

### 9.9 Employability and market system

Create `market/EMPLOYABILITY_AND_MARKET_PLAN.md`.

It should define:

- primary and secondary role families;
- representative job-description evidence process;
- requirement-to-evidence gap mapping;
- current strengths and blockers;
- portfolio artifact requirements;
- resume and GitHub positioning requirements;
- application-readiness gates;
- application activation timing;
- interview-preparation and feedback loop;
- geographic and work-mode strategy;
- evidence required to change target roles.

Recommended career-transition flow:

```text
current profile
→ representative role requirements
→ evidence and gap map
→ capability and portfolio work
→ defensible resume/GitHub claims
→ application-readiness review
→ applications and interviews
→ feedback-driven correction
→ first technical role
```

Do not create a detailed application tracker until applications are authorized by the market plan or Ali explicitly activates them.

### 9.10 Project evidence stored in Career

`tracking/evidence/UP-S01_pydantic-13432_manual-evidence-report.md` is technical project evidence.

Proposed action:

1. confirm the canonical evidence or equivalent history exists in UpgradePilot;
2. preserve its Career-level significance in the UpgradePilot portfolio record and capability ledger;
3. remove the technical evidence file from active Career;
4. rely on the UpgradePilot repository and Git history for technical details.

No project evidence should be deleted until its canonical project location and Career-level conclusion are verified.

## 10. Update cadence after refoundation

### 10.1 Continuous project operation

Occurs in project repositories only.

### 10.2 Light Career pulse

A short Career check may occur weekly or biweekly without requiring a repository change. It asks:

- Is the flagship still producing meaningful capability and portfolio evidence?
- Is workload sustainable?
- Is a career-level decision emerging?
- Is market or portfolio work being neglected?

Update Career only when the answer produces a material career-level change.

### 10.3 Formal or event-triggered review

A Career review occurs when:

- a scheduled review date arrives;
- Ali requests one;
- a major project gate changes portfolio interpretation;
- workload becomes materially unrealistic;
- a capability claim is proposed;
- application readiness is being considered;
- target roles or geography may change;
- the flagship becomes infeasible or misaligned;
- a new project is proposed;
- a career cycle ends.

### 10.4 Career state maintenance

`CAREER_STATE.md` changes only after a material career event or review. It is more active than the current formal-review-only system, but remains far less granular than a project tracker.

## 11. Refoundation execution phases

No phase begins until this plan is approved.

### Phase 0 — Safeguard and complete inventory

Actions:

- record the pre-refoundation commit SHA;
- enumerate every current file and classify it as active, historical, duplicate, project-specific, compatibility-only, or unknown;
- verify all current links to files proposed for rename or removal;
- confirm which project evidence already exists in UpgradePilot;
- identify any public-sensitive content requiring special handling;
- create a migration checklist.

Gate:

- every current file has a proposed disposition;
- no deletion is authorized without a replacement or explicit historical decision.

### Phase 1 — Establish the new authority foundation

Create:

- `CAREER_CHARTER.md`;
- `CAREER_STATE.md`;
- `governance/CAREER_OPERATING_CONTRACT.md`.

Rewrite:

- `README.md`;
- `AGENTS.md`;
- `governance/SECURITY_AND_PRIVACY.md` as needed.

Gate:

- repository mission, live state, and authority routing are unambiguous;
- UpgradePilot remains independently controlled.

### Phase 2 — Restore the personal and strategic core

Create or migrate:

- `profile/CAREER_PROFILE.md`;
- `strategy/CAREER_STRATEGY.md`;
- `strategy/PROJECT_PORTFOLIO_AND_SELECTION_POLICY.md`;
- `strategy/ADVANCED_CAPABILITY_EXPOSURE_POLICY.md`.

Gate:

- the repository is clearly about Ali's complete career rather than only UpgradePilot;
- profile statements distinguish evidence, preferences, assumptions, and unknowns;
- advanced exposure no longer forces artificial architecture.

### Phase 3 — Build portfolio and capability truth

Create:

- `portfolio/PROJECT_PORTFOLIO.md`;
- project records for UpgradePilot, Sentinel, and AegisLab;
- `tracking/CAPABILITY_EVIDENCE_LEDGER.md`;
- `tracking/CAREER_REVIEW_LOG.md`.

Migrate conservative conclusions from current Career records.

Gate:

- every current project has a defined career role;
- capability records are cross-project and evidence-based;
- project progress and Ali capability remain separate.

### Phase 4 — Add employability and current-cycle control

Create:

- `market/EMPLOYABILITY_AND_MARKET_PLAN.md`;
- `plans/CURRENT_CAREER_CYCLE.md`.

Gate:

- the current cycle contains project, capability, portfolio, and market outcomes;
- target roles are connected to actual evidence gaps;
- the route toward applications is explicit without prematurely creating application bureaucracy.

### Phase 5 — Migrate and remove obsolete active files

After replacements pass review:

- remove compatibility routes;
- remove old project-specific Career trackers and capability specifications;
- move or replace the root UpgradePilot record;
- remove duplicated or stale 90-day/project files;
- remove Career-hosted technical evidence after canonical verification;
- update all links;
- rely on Git history for superseded content unless an explicit historical file remains useful.

Gate:

- no active file has an unclear owner;
- no obsolete file redirects agents to project operation;
- no required historical conclusion is lost.

### Phase 6 — Conduct the first refounded Career review

Inspect current UpgradePilot evidence only to answer career-level questions.

Produce:

- current coarse project contribution;
- current capability assessment and transfer limits;
- workload decision;
- portfolio status;
- employability phase;
- market and portfolio gaps;
- next Career review trigger;
- updated `CAREER_STATE.md`.

This review must not change UpgradePilot's technical continuation.

### Phase 7 — Final audit and activation

Audit:

- authority and links;
- duplication;
- public-safety;
- project boundary;
- evidence and claim discipline;
- usefulness for Ali;
- long-term continuity beyond October 17;
- document count and ceremony.

Mark the refoundation complete only after Ali reviews the final structure and the acceptance criteria pass.

## 12. Recommended commit strategy

Use small, reviewable commits:

1. `Establish Career charter and live state`
2. `Restore Career profile and strategy`
3. `Add portfolio and capability governance`
4. `Add employability and current-cycle system`
5. `Migrate historical conclusions and remove obsolete controls`
6. `Record first refounded Career review`
7. `Finalize Career repository refoundation`

Do not combine all changes into one opaque commit.

Do not force-push or rewrite history.

## 13. Acceptance criteria

The refoundation passes only when all are true.

### 13.1 Mission and scope

- Career clearly governs Ali's complete career, not only UpgradePilot.
- The repository remains useful after the current 90-day cycle.
- UpgradePilot remains the current flagship but not the repository's sole meaning.

### 13.2 Truth routing

- one file owns live career state;
- no Career file owns UpgradePilot technical continuation;
- one file owns the project portfolio;
- one file owns capability evidence;
- one file owns market and employability planning;
- no material current fact is duplicated across several files.

### 13.3 Personalization

- a current public-safe career profile exists;
- real background, strengths, gaps, preferences, constraints, and uncertainties are represented honestly;
- sensitive details are excluded;
- the system reflects Ali's mission-driven, learning-by-building method.

### 13.4 Career progression

- project work connects to capability goals;
- capability evidence connects to target roles;
- target roles connect to portfolio and market actions;
- an application-readiness path exists;
- feedback can change the strategy through controlled review.

### 13.5 Portfolio

- UpgradePilot, Sentinel, and AegisLab have clear career roles;
- historical projects are neither ignored nor accidentally reactivated;
- portfolio claims include assistance and limitations;
- future projects require explicit admission.

### 13.6 Evidence and honesty

- no capability is inferred from documentation volume, AI-generated code, successful commands, or passing AI-generated tests alone;
- records include assistance, recency, confidence, and transfer limits;
- product progress and personal capability remain separate.

### 13.7 Advanced capabilities

- advanced interests remain visible;
- exposure is evidence-led and role-relevant;
- no artificial all-technology architecture is required;
- negative and rejected experiments remain valid evidence.

### 13.8 Lean operation

- no daily Career bureaucracy exists;
- no duplicate project tracker exists;
- no compatibility pointer remains without a real need;
- every active file has a clear durable owner;
- repository navigation answers common questions within two links from `README.md`.

### 13.9 Safety

- all active content is public-safe;
- no credentials, private routines, medical details, or unnecessary personal identifiers are included;
- market and application records follow the privacy policy.

## 14. Decisions requiring Ali approval

Approval of this plan should explicitly confirm or revise:

1. creation of `CAREER_CHARTER.md` and `CAREER_STATE.md`;
2. the proposed active directory structure;
3. migration of the learning profile into a concise active career profile;
4. moving `UpgradePilot.md` into the project portfolio area;
5. replacing the UpgradePilot-specific Career tracker and capability specification with general Career-wide records;
6. adding the employability and market system;
7. replacing the mandatory all-six advanced-system 90-day quota with an evidence-based exposure portfolio;
8. removing technical UP-S01 evidence from Career after canonical verification;
9. using Git history rather than retaining every superseded file in an archive directory;
10. preserving the current Career–UpgradePilot operational boundary.

## 15. Work explicitly deferred until after refoundation

Do not perform these during the structural refoundation unless Ali separately authorizes them:

- rewrite the UpgradePilot technical route;
- change UpgradePilot source or tests;
- select a new flagship;
- begin a second major project;
- generate a resume;
- begin job applications;
- create interview drills;
- create a networking campaign;
- add new advanced-system experiments;
- claim increased capability from the refoundation itself.

These become later Career actions only after the corrected system can govern them.

## 16. Approval and next action

**Current status:** Proposed.

No existing Career file should be edited, renamed, moved, or deleted until Ali reviews and approves this plan.

After approval, the next action is:

> **Phase 0 — Safeguard and complete inventory**, followed by Phase 1 authority foundation.

The implementation must follow the phases and gates above, with Ali able to review and correct the structure before obsolete files are removed.
