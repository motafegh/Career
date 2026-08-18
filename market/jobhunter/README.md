# JobHunter — Career-Side Integration

**Status:** Career-side requirements and integration area  
**External implementation repository:** `motafegh/jobhunter`  
**Career owner:** `market/EMPLOYABILITY_AND_MARKET_PLAN.md`  
**Role:** Market-intelligence and career-decision support infrastructure

## Purpose

This folder defines what the Career system needs from JobHunter and how Career interprets its role.

It does **not** control JobHunter implementation, architecture, milestones, source code, or technical continuation. Those remain owned by `motafegh/jobhunter`.

Career uses JobHunter as an evidence-producing instrument that can help answer:

- what work employers are actually hiring for;
- which responsibilities recur across realistic target roles;
- which skills, knowledge, tools, practices, credentials, and constraints recur;
- which expectations are required, preferred, contextual, or merely inferred;
- how demand differs by role family, seniority, geography, industry, company type, and time;
- which role families are realistically accessible to Ali now or after bounded improvement;
- which capability, evidence, portfolio, CV, interview, and application gaps matter most;
- which apparent gaps are employer-specific noise and should **not** redirect the Career plan;
- whether market evidence supports changing learning priorities, project responsibilities, role targeting, or application timing.

## Permanent authority boundary

JobHunter does not decide Ali's career.

Use this authority chain:

```text
employer/public source evidence
→ JobHunter deterministic source representation
→ JobHunter translation or model-derived interpretation
→ JobHunter aggregate market signal
→ Career review
→ Career decision
```

The Career repository remains authoritative for:

- Ali's capability and ownership claims;
- career strategy and current working identity;
- project allocation;
- capability priorities;
- portfolio claims;
- application readiness;
- CV claims;
- exact current Career action.

JobHunter must not automatically rewrite Career files or silently change those decisions.

## Capability-evidence boundary

JobHunter is currently a career-support tool, not a capability-building flagship.

Ali currently classifies its implementation as full AI vibe coding. Repository sophistication, AI-generated implementation, passing tests, architecture, or feature count in `motafegh/jobhunter` must therefore not be treated as evidence that Ali independently owns those engineering capabilities.

If Ali later deliberately studies, modifies, tests, diagnoses, and owns bounded JobHunter responsibilities, that evidence may be assessed separately through the normal Career capability process.

## Files

- [`JOBHUNTER_CAREER_RECORD.md`](JOBHUNTER_CAREER_RECORD.md) — JobHunter's Career role, current ownership boundary, Career-facing value, CV/portfolio treatment, and review triggers.
- [`CAREER_REQUIREMENTS.md`](CAREER_REQUIREMENTS.md) — complete Career-side product and information requirements for JobHunter, including future capabilities that may not exist yet.
- [`CAREER_INTEGRATION_AND_USE.md`](CAREER_INTEGRATION_AND_USE.md) — how JobHunter evidence may enter Career decisions, what quality gates apply, and what it may never decide automatically.

## Design principle

The desired JobHunter is not a generic job scraper and not a résumé-keyword matcher.

The target is an explainable personal market-intelligence system:

```text
real vacancies
→ trustworthy source evidence
→ responsibilities and requirements
→ normalized market patterns
→ role-family and geography comparisons
→ Career capability/evidence comparison
→ explainable gaps and opportunities
→ reviewed Career actions
```

The implementation may evolve substantially. This folder should remain focused on the **Career outcomes, ownership boundary, and evidence contract** rather than prescribing unnecessary technical architecture.
