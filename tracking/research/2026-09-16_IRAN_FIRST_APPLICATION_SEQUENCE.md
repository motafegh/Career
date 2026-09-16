# Iran Market — First Application Sequence

**Date:** 2026-09-16  
**Status:** Active Iran-only vacancy resolution sequence; application decisions remain provisional until native-detail and private-access checks are complete  
**Owner:** Career market-calibration evidence  
**Parent evidence:** `2026-09-16_IRAN_MARKET_CURRENT_VACANCY_REFRESH.md`  
**Readiness authority:** `../../CAREER_STATE.md`

## 1. Purpose

Convert the current Iranian market refresh into a bounded application sequence without mass-applying, guessing access eligibility, or overstating Ali's technical ownership.

For every candidate use the same sequence:

```text
1. CURRENT / OPEN?
2. EXACT NATIVE DUTIES?
3. ACCESS GATES?
4. RESPONSIBILITY FIT?
5. ALI EVIDENCE / CLAIM FIT?
6. MINIMUM APPLICATION MATERIALS READY?
7. APPLY / HOLD / REJECT
```

A role is not promoted to `APPLY` merely because its title looks relevant.

---

## 2. Decision vocabulary

### Current/open

- `CONFIRMED` — sufficiently current source evidence supports an active listing.
- `LIKELY CURRENT` — very recent evidence exists but native listing state still needs final verification.
- `UNRESOLVED` — current status cannot yet be established reliably.
- `CLOSED/STALE` — do not apply.

### Access gate

- `PASS` — no known access blocker after checking the actual vacancy and relevant private facts.
- `FAIL` — a hard employer gate is not satisfied.
- `UNRESOLVED` — one or more private or vacancy-specific facts are still missing.

### Responsibility fit

- `STRONG` — directly matches an approved narrow E3 responsibility family.
- `PLAUSIBLE` — meaningful overlap but not a direct fit.
- `WEAK` — poor current strategic fit.

### Evidence / claim fit

- `DEFENSIBLE` — Ali can apply honestly at the role's stated level without implying capabilities Career does not support.
- `STRETCH` — a junior/mentored application may still be reasonable, but a central responsibility is weaker than the role asks.
- `NOT DEFENSIBLE` — applying would require ignoring a known central gap or overclaiming.

### Final decision

- `APPLY` — current/open + access passes + responsibility/evidence fit is defensible + minimum private materials are ready.
- `APPLY IF ACCESS PASSES` — role/capability shape is sufficient; only unresolved access/material checks remain.
- `HOLD` — one or more high-information missing facts prevent a sound decision.
- `REJECT FIRST BATCH` — low-information application or current responsibility mismatch.

---

# 3. Priority sequence

## Candidate 1 — Data Mining Energy Avisa

**Original title:** `کارآموز توسعه نرم‌افزار (Python/Django)`  
**Source:** JobVision current vacancy evidence  
**Freshness at refresh:** approximately two days  
**Normalized family:** Junior Python / software-development internship

### What we know

- explicitly an internship;
- explicitly Python/Django;
- current/recent vacancy evidence is strong enough to justify native-detail inspection;
- internship framing materially reduces the expectation of established professional ownership compared with a normal backend-engineer role.

### Missing before application

- native/current application state;
- exact Python/Django expectations;
- whether current university enrollment or a specific degree is mandatory;
- location and on-site/remote arrangement;
- weekly schedule / internship duration;
- whether prior project evidence is acceptable;
- any gender, age, military-service or other explicit gate.

### Four-way filter

- Current/open: `LIKELY CURRENT`.
- Access: `UNRESOLVED`.
- Responsibility fit: `STRONG / PLAUSIBLE`.
- Evidence fit: `DEFENSIBLE STRETCH`.
- Decision: **HOLD FOR NATIVE DETAIL → APPLY IF ACCESS PASSES.**

### Why first

It is the cleanest fresh Iranian entry-level technical route in the current evidence set. If the access gates are reasonable, it can test Ali's current Python/project story without pretending broad production-backend ownership.

---

## Candidate 2 — Fara Samaneh / Hamkaran System

**Original title:** `کارشناس استقرار و پشتیبانی نرم افزار (ERP)`  
**Source:** JobVision official current/urgent feed  
**Location evidence:** Tehran  
**Normalized family:** ERP implementation / software support / customer-process translation

### What we know

- current repeated listing evidence exists;
- the responsibility family strongly matches Career's implementation/support lane;
- Ali's prior business/operational/customer responsibility may transfer meaningfully here.

### Missing before application

- exact current employer-authored duties;
- degree and field requirement;
- years of experience;
- ERP/domain experience requirement;
- SQL/database expectation;
- customer-site/travel expectation;
- age/gender/military-service constraints if explicitly stated;
- current application state.

Historical postings from the same employer are not valid substitutes for the current job description.

### Four-way filter

- Current/open: `LIKELY CURRENT`.
- Access: `UNRESOLVED`.
- Responsibility fit: `STRONG`.
- Evidence fit: `DEFENSIBLE / STRETCH`.
- Decision: **HOLD FOR CURRENT NATIVE JD → APPLY IF ACCESS PASSES.**

### Why second

This role family may use Ali's nontechnical professional history as an asset rather than treating it as irrelevant, while still providing a genuine technical/system responsibility path.

---

## Candidate 3 — Tabansoft

**Original title:** `کارشناس پشتیبان نرم افزار`  
**Source:** JobVision fresh current/indexed evidence  
**Freshness:** surfaced within hours during the September 16 refresh  
**Normalized family:** Software/product support

### What we know

- very fresh vacancy existence;
- software-support responsibility is inside the approved E3 band.

### Key unknown

The title alone is insufficient. We need to distinguish:

```text
technical product support
(logs / database / APIs / integrations / defect reproduction / diagnosis)

from

generic customer support
(ticket handling without meaningful technical responsibility)
```

### Missing before application

- exact product/domain;
- technical investigation depth;
- SQL/API/log/integration responsibilities;
- experience and education requirements;
- work location/mode;
- access constraints;
- current-open state.

### Four-way filter

- Current/open: `LIKELY CURRENT`.
- Access: `UNRESOLVED`.
- Responsibility fit: `STRONG` **if technically diagnostic**, otherwise `WEAK/PLAUSIBLE`.
- Evidence fit: `potentially DEFENSIBLE`.
- Decision: **HOLD FOR NATIVE DETAIL.**

---

## Candidate 4 — Novo Nordisk Pars

### 4A — ERP Functional Support

**Original title:** `کارشناس پشتیبانی عملکردی ERP در حوزه فناوری اطلاعات`  
**Source:** IranTalent current root listing  
**Freshness:** same-day evidence at refresh  
**Normalized family:** ERP functional support / process-to-system translation

Potential value if the native duties confirm it:

- business/process interpretation;
- system support;
- stakeholder communication;
- issue/requirement translation;
- coordination with technical teams.

#### Four-way filter

- Current/open: `CONFIRMED at root-listing level; recheck before submission`.
- Access: `UNRESOLVED`.
- Responsibility fit: `potentially STRONG`.
- Evidence fit: `potentially DEFENSIBLE / STRETCH`.
- Decision: **HOLD FOR NATIVE DETAIL.**

### 4B — ERP Technical Support Engineer

**Original title:** `مهندس پشتیبانی فنی ERP`  
**Source:** IranTalent current root listing  
**Freshness:** same-day evidence at refresh  
**Normalized family:** ERP technical support / troubleshooting

The role could become attractive if the actual depth centers on bounded troubleshooting, configuration and integrations. It becomes a poor first-batch fit if it expects established ERP administration, deep SQL/database ownership, enterprise-integration ownership or several years of specialist experience.

#### Four-way filter

- Current/open: `CONFIRMED at root-listing level; recheck before submission`.
- Access: `UNRESOLVED`.
- Responsibility fit: `STRONG shape`.
- Evidence fit: `STRETCH until duties are known`.
- Decision: **HOLD FOR NATIVE DETAIL.**

### Resolution order

Inspect the **functional-support** role first because its likely responsibility shape may align more strongly with Ali's combined business/process + growing technical profile.

---

## Candidate 5 — Digify

**Original title:** `Technical Support`  
**Source:** Jobinja current jobs surface + recent employer/public hiring evidence  
**Location evidence:** Tehran  
**Normalized family:** Technical product/support

### Missing before application

- product and customer context;
- whether troubleshooting reaches logs/data/API/integration layers;
- experience requirement;
- technical stack;
- on-site/hybrid/remote condition;
- access constraints;
- actual current-open state at submission.

### Four-way filter

- Current/open: `LIKELY CURRENT`.
- Access: `UNRESOLVED`.
- Responsibility fit: `PLAUSIBLE → STRONG depending on JD`.
- Evidence fit: `potentially DEFENSIBLE`.
- Decision: **HOLD FOR EXACT JD.**

---

# 4. Conditional QA lane

Do not expand QA into a large separate search yet.

A fresh QA/testing vacancy enters this batch only when its native job description is reasonably junior and emphasizes responsibilities such as:

- manual/API validation;
- test-case reasoning;
- defect reproduction;
- bug documentation;
- product-quality investigation;
- basic tooling or bounded automation.

Reject first-batch QA roles that centrally require established automation/SDET ownership, several years of professional QA, or deep framework expertise.

Current JobVision evidence confirms fresh QA/testing vacancies exist, so this lane remains a fallback after Candidates 1–5 are resolved.

---

# 5. Explicit first-batch benchmark / reject

## Serita — Junior Software Developer

**Known current/recent duties include:**

- Python + FastAPI;
- JavaScript/frontend;
- PostgreSQL;
- REST APIs;
- Git;
- Docker/Tailwind as pluses;
- OpenAI/Gemini API exposure as a plus;
- on-site Tehran;
- junior/learning orientation.

### Four-way filter

- Responsibility fit: `PLAUSIBLE`.
- Evidence fit: `NOT DEFENSIBLE / excessive STRETCH for this first calibration batch` because the role combines broad full-stack/backend/database implementation beyond current ownership evidence.
- Decision: **REJECT FIRST BATCH — keep as a benchmark for later readiness.**

This is not evidence that Ali cannot become suitable. It is a current claim/readiness boundary.

---

# 6. e-estekhdam status

**No current technical candidate from e-estekhdam is promoted into this sequence yet.**

Reason:

- the accessible search/index layer repeatedly surfaced stale historical posts with recent crawl dates;
- actual publication date and current-open status could not be established strongly enough for the targeted technical examples.

Interpretation:

```text
acquisition unresolved
!= no technical jobs exist
```

Keep e-estekhdam active as a discovery source, but require native/current publication evidence before adding a vacancy to the application sequence.

---

# 7. Iran-specific access checks

For a candidate that survives responsibility/evidence screening, resolve only the actual employer-stated gates that matter:

- city / on-site presence;
- degree and field;
- student or recent-graduate status for internships;
- work experience;
- prior software-company/ERP/support experience;
- military-service status where explicitly required;
- gender/age only when explicitly employer-stated;
- language;
- customer-site/travel expectations;
- working hours / internship schedule;
- any other hard employer condition.

Never convert a failed access gate into a technical-learning task.

---

# 8. Application-material gate

The Career repository currently has no canonical role-tailored CV/resume artifact for this Iran-only application lane.

Therefore the sequence is deliberately:

```text
vacancy survives native-detail + access review
→ select first real application candidate(s)
→ create one minimal claim-bounded Iran-appropriate CV package
→ adapt only what the actual vacancy requires
→ final claim check
→ submit privately
```

Minimum package when activated:

- Persian/Iran-appropriate CV or resume;
- English variant only where employer/job language warrants it;
- concise UpgradePilot/project explanation with accurate AI-assistance boundary;
- transferable business/operations experience represented honestly;
- private contact/location/access facts;
- short role-specific note only where useful.

Do **not** create multiple speculative resume variants before the first candidate survives screening.

---

# 9. Execution order

Resolve candidates in this order unless one expires first:

1. Avisa — Python/Django internship.
2. Fara Samaneh — ERP implementation/support.
3. Tabansoft — software support.
4. Novo Nordisk Pars — ERP functional support, then ERP technical support.
5. Digify — Technical Support.
6. One or two fresh QA/testing candidates only if the first five do not yield enough viable applications.
7. e-estekhdam candidate only after current publication/detail evidence becomes reliable.

International candidates from the September 14 shortlist are **deferred during this Iran-only operating focus**, not rejected and not erased.

---

# 10. Stop condition

Do not broaden to another large Iran search while these candidates remain unresolved.

Broaden only when:

- the current candidates are resolved/expired;
- fewer than roughly 2–3 credible application candidates survive;
- one responsibility family proves systematically inaccessible;
- a new very fresh high-information vacancy appears;
- Ali changes the market-focus instruction.

The purpose of this sequence is to generate **real Iranian market feedback**, not maximize vacancy count.