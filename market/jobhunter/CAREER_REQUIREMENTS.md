# JobHunter Career Requirements

**Status:** Career-side requirements specification  
**Scope:** What JobHunter should eventually provide to improve Career decisions  
**Implementation authority:** `motafegh/jobhunter`  
**Career authority:** `market/EMPLOYABILITY_AND_MARKET_PLAN.md`

## 1. Objective

JobHunter should become the Career system's primary market-observation and job-analysis instrument.

Its purpose is not to maximize collected advertisements or produce opaque fit scores. Its purpose is to turn representative public vacancy evidence into explainable, auditable information that helps Career make better decisions about:

- role targeting;
- capability priorities;
- learning allocation;
- project responsibilities;
- portfolio evidence;
- application readiness;
- vacancy selection;
- CV tailoring;
- interview preparation;
- geographic strategy;
- market change over time.

A useful JobHunter answer should normally be traceable from a Career conclusion back to a set of actual employer postings and, where material, to the relevant employer wording.

## 2. Core questions JobHunter must support

JobHunter should eventually make it practical to answer all of the following.

### Market structure

- Which role families are actually appearing in the markets we care about?
- Which titles are aliases for similar responsibility patterns?
- Which apparently similar titles describe materially different work?
- Which role families are growing, stable, declining, or too sparsely sampled to judge?
- Which roles are genuinely junior, trainee, graduate, or entry-accessible rather than merely titled junior?
- Which role families commonly provide mentorship, code review, team structure, and bounded ownership?

### Responsibilities

- What work is the employee actually expected to perform?
- Which responsibilities recur across postings?
- Which responsibilities are core to a role family versus employer-specific?
- Which deliverables recur: APIs, services, data pipelines, models, dashboards, automation, tests, detection rules, integrations, reports, infrastructure, or other outcomes?
- What ownership level is implied: assist, implement, maintain, design, lead, operate, troubleshoot, review, or own end-to-end?

### Requirements

- Which programming languages, tools, frameworks, platforms, practices, domains, credentials, and interpersonal capabilities recur?
- Which are explicitly required, preferred, contextual, or model-inferred supporting capabilities?
- Which requirements appear together?
- What depth is implied by the wording and responsibility, not only by a tool mention?
- What experience duration is requested, and how consistently is it enforced across comparable roles?
- Which educational, language, legal, location, travel, on-call, or work-authorization constraints matter?

### Ali-specific decisions

- Which realistic jobs overlap most strongly with capabilities Ali can actually defend?
- Which gaps are knowledge gaps, practice gaps, depth gaps, integration gaps, evidence gaps, recency gaps, presentation gaps, experience-context gaps, or constraint mismatches?
- Which gaps are true application blockers and which are reasonable learn-on-job gaps?
- Which missing capabilities have the highest market payoff for Ali's target role families?
- Which capabilities should be learned now, practiced more, demonstrated through a project, documented better, or ignored for now?
- Which role families should Career prioritize, monitor, downgrade, or stop pursuing?
- Which current projects can naturally provide missing evidence without artificial scope expansion?
- Which vacancies are credible applications, reasonable stretches, low-priority, blocked, or still uncertain?

## 3. Source and sampling requirements

### 3.1 Multi-source support

JobHunter should support multiple approved public sources rather than treating one job board as the market.

Desired source types include:

- public job boards with permitted access;
- public company career pages;
- public Applicant Tracking System vacancy pages or feeds;
- official public vacancy APIs or feeds;
- user-supplied public URLs;
- user-supplied job text or files when automated acquisition is unsuitable.

Each source must retain source identity and source-specific limitations.

### 3.2 Geographic coverage

Career should eventually be able to compare at least:

- Iran / Jobinja-type market evidence;
- United Arab Emirates;
- broader Asia markets relevant to Ali;
- remote roles when meaningfully available to Ali.

Additional geographies may be added when Career strategy requires them.

### 3.3 Sampling profiles

JobHunter should support both targeted and control samples.

Targeted profiles should include at least:

- broad junior software engineering;
- Python/backend;
- Python automation and technical implementation;
- data engineering and data-heavy software roles;
- applied AI / AI application engineering;
- ML trainee/junior roles;
- QA/test automation with Python;
- security automation;
- AI/security hybrid roles;
- cloud/platform/MLOps trainee roles when Career is actively evaluating them.

A broader control sample is needed to detect search-selection bias. The system must not conclude that a technology dominates the market merely because the search catalog was designed around that technology.

### 3.4 Search-coverage audit

For every market report, JobHunter should be able to show:

- sources included;
- search profiles, terms, filters, and URLs used;
- date range;
- geography and work-mode filters;
- number of acquisition attempts;
- jobs discovered;
- jobs with complete details;
- jobs included/excluded from analysis and why;
- overlap between searches;
- duplicate/repost handling;
- source failures or inaccessible slices;
- estimated blind spots and known sampling bias.

### 3.5 Time windows and freshness

All market aggregates should carry a clear time window and freshness status.

Useful views include:

- current snapshot;
- rolling 30/60/90-day windows when enough evidence exists;
- comparison with prior equivalent windows;
- first-seen, last-seen, and posting-lifecycle information.

Old postings must not silently dominate a current-market conclusion.

## 4. Source truth, identity, and provenance

JobHunter should preserve permanent distinctions between:

```text
source evidence
≠ deterministic parsing
≠ translation
≠ model interpretation
≠ taxonomy mapping
≠ aggregate market calculation
≠ Ali-specific assessment
```

Required capabilities include:

- stable source/job identity;
- immutable or otherwise auditable source snapshots;
- canonical source URL;
- fetch/check history;
- meaningful employer-content versions separate from raw page volatility;
- explicit duplicate and repost relationships where detectable;
- source language;
- translation provider/model/schema identity;
- analysis model/prompt/schema identity;
- exact evidence passages for material semantic claims;
- confidence/review state;
- timestamps and freshness;
- retained historical derived artifacts rather than destructive replacement.

No translation or LLM interpretation may be displayed as though it were employer-authored source text.

## 5. Job representation requirements

Each job should eventually expose a structured representation covering, when supported by evidence:

### Identity and context

- source and source job ID;
- canonical URL;
- company;
- title;
- location;
- remote/hybrid/on-site arrangement;
- employment type;
- industry/company context where available;
- posting and validity dates;
- lifecycle state;
- language;
- compensation when explicitly public;
- legal/work-authorization/location constraints;
- travel/on-call requirements;
- education/certification constraints.

### Role purpose and responsibilities

For each responsibility:

- normalized statement;
- original employer wording;
- evidence passage;
- explicit versus inferred state;
- action/object/context/outcome where useful;
- ownership signal;
- confidence;
- review status;
- linked deliverables;
- linked career concepts.

### Requirements

For each requirement:

- canonical concept candidate;
- original employer wording;
- evidence passage;
- requirement type: required, preferred, contextual, inferred;
- concept type: language, skill, tool, framework, platform, practice, knowledge, domain, experience, credential, interpersonal capability, legal/location constraint, or other justified type;
- depth signal;
- requested duration where explicit;
- rationale when inferred;
- confidence and review status;
- linked responsibilities.

### Deliverables

Where supported, JobHunter should identify expected outputs such as:

- software service;
- API;
- automation;
- data pipeline;
- ML model;
- evaluation/report;
- dashboard;
- integration;
- test suite;
- deployment;
- detection rule;
- incident response artifact;
- infrastructure/platform component;
- documentation or stakeholder deliverable.

## 6. Career-concept taxonomy

JobHunter eventually needs a versioned normalization layer so aliases do not fragment the market view.

Examples:

```text
Postgres / PostgreSQL
REST API / RESTful API / HTTP API
CI/CD / continuous integration and delivery
LLM / large language model
RAG / retrieval-augmented generation
```

The taxonomy should:

- preserve the exact original mention;
- map aliases to a canonical concept when justified;
- distinguish tool from capability;
- distinguish framework from underlying responsibility;
- preserve uncertainty rather than force weak mappings;
- support parent/child and related-concept relationships;
- be versioned because mapping changes can alter historical aggregates.

A tool mention alone must not automatically imply applied capability or required depth.

## 7. Role archetypes

Job titles are too inconsistent to be the sole Career unit.

JobHunter should derive or support reviewed **role archetypes** based on recurring responsibility and capability patterns.

Examples may eventually include patterns such as:

- Python application/backend implementer;
- Python automation/integration engineer;
- data pipeline/analytics engineer;
- applied AI application engineer;
- ML experimentation engineer;
- test/quality automation engineer;
- security automation/detection engineer;
- implementation/solutions engineer.

These are examples, not predefined buckets that every posting must fit.

For each archetype JobHunter should show:

- representative responsibilities;
- common requirements;
- common technology combinations;
- typical experience/seniority signals;
- geography/work-mode distribution;
- sample size;
- representative jobs;
- important outliers;
- uncertainty.

## 8. Market analytics requirements

All frequencies must normally use distinct jobs as the denominator, not raw mentions.

JobHunter should support:

### Requirement demand

For each concept:

- jobs mentioning it;
- share of relevant analyzed jobs;
- required count/share;
- preferred count/share;
- contextual count/share;
- inferred count/share shown separately;
- role-family distribution;
- seniority distribution;
- geography distribution;
- work-mode distribution;
- trend over time when enough history exists.

### Responsibility demand

For each normalized responsibility:

- jobs requiring it;
- role families where it appears;
- ownership/depth signals;
- associated deliverables;
- associated concepts/tools;
- geography/seniority distribution.

### Co-occurrence

Support questions such as:

- which skills commonly appear with Python;
- which technologies cluster around junior backend roles;
- whether SQL is tied to data roles only or broadly expected;
- whether Docker is usually required or merely preferred;
- which AI roles also require traditional software engineering fundamentals.

### Experience and entry barriers

Track:

- requested years of experience;
- degree requirements;
- graduate/fresh-entry language;
- professional-team experience requirements;
- location/work authorization;
- language constraints;
- independent ownership expectations;
- seniority words and responsibility signals.

Do not reduce entry accessibility to requested years alone.

### Geography and work-mode comparison

Compare:

- role availability;
- recurring requirements;
- entry barriers;
- remote/hybrid/on-site prevalence;
- language constraints;
- degree requirements;
- visa/work-authorization constraints when explicit;
- technology and responsibility differences.

### Company and industry dimensions

Where evidence permits:

- company size/type;
- industry;
- product versus consulting/implementation context;
- startup versus established company;
- internal platform versus customer-facing delivery.

These should help interpret why requirements differ rather than become unsupported company profiling.

## 9. Data-quality and uncertainty requirements

Every aggregate used for a Career decision should expose enough information to judge whether it is trustworthy.

Required quality indicators include:

- analyzed-job count and denominator;
- source count and distribution;
- date range;
- geography distribution;
- native versus translated content distribution;
- parse success/partial/failure counts;
- translation success/review state;
- analysis success/review state;
- duplicate/repost handling;
- missing-field rates;
- sampling/search bias warnings;
- small-sample warnings;
- stale-data warnings;
- model/prompt/schema version;
- taxonomy version;
- known source outages or inaccessible segments.

JobHunter must prefer `unknown` or `insufficient evidence` over manufactured precision.

## 10. Ali capability and evidence integration

JobHunter should eventually be able to consume a **Career-approved capability snapshot**.

Career remains authoritative for Ali's capability evidence.

JobHunter must not infer mastery from:

- repository size;
- repository technology list;
- documentation;
- successful commands;
- AI-generated implementation;
- project completion;
- GitHub contribution count;
- self-description alone.

A Career capability snapshot should preserve, where applicable:

- exact responsibility/capability;
- Career depth state;
- evidence references;
- assistance level;
- recency;
- confidence;
- transfer limits;
- current claim boundary.

If JobHunter internally uses another scale, it must not silently replace the Career capability scale. Any mapping must be explicit and reversible.

## 11. Gap analysis

For each target role, archetype, or market requirement, JobHunter should be able to classify the Ali-side issue as one or more of:

- **knowledge gap** — underlying concepts are missing;
- **practice gap** — concept understood but insufficient real execution;
- **depth gap** — some evidence exists below the level repeatedly demanded;
- **integration gap** — components are known separately but not combined in realistic work;
- **evidence gap** — capability may exist but is not demonstrable;
- **recency gap** — evidence is too old for a strong current claim;
- **presentation gap** — evidence exists but CV/GitHub/project explanation does not expose it;
- **experience-context gap** — employers expect team/production/customer context not established by projects;
- **constraint mismatch** — degree, location, language, authorization, schedule, or another non-skill constraint;
- **unknown** — evidence is insufficient to classify safely.

JobHunter should additionally help Career distinguish:

- blocking gaps;
- material gaps;
- differentiating gaps;
- reasonable learn-on-job gaps;
- employer-specific gaps that should not redirect the Career plan.

## 12. Learning-priority proposals

JobHunter may propose learning priorities, but proposals must be explainable.

A useful priority proposal should combine at least:

- frequency across realistic target jobs;
- required versus preferred strength;
- relevance across multiple target role families;
- current Ali gap severity;
- expected time/cost to reach useful evidence;
- transferability;
- whether the capability can be learned within active project responsibilities;
- whether the capability unlocks applications or merely adds breadth;
- uncertainty/sample quality.

It must not rank priorities by raw keyword frequency alone.

The output should be a proposal such as:

```text
Increase SQL priority
Reason:
- common across three active role families;
- frequently required rather than preferred;
- current Career evidence is weak;
- bounded practice can create reusable evidence;
- likely application blocker for data-heavy roles.
```

not:

```text
SQL score = 87.3
```

## 13. Project and portfolio guidance

JobHunter should help answer:

- which market-supported responsibilities are currently missing from Ali's evidence;
- whether an existing project can naturally provide that evidence;
- whether a small supporting exercise is enough;
- whether adding a technology would be artificial scope expansion;
- which project evidence is strongest for each role family;
- which project claims need better demonstration or explanation;
- which project is irrelevant to a particular role and should be omitted.

Desired output: **Project Evidence Opportunity Map**

| Market responsibility | Demand evidence | Current Ali evidence | Natural project opportunity | Smallest useful proof | Career decision |
|---|---|---|---|---|---|

JobHunter may suggest opportunities but does not change project scope automatically.

## 14. Application intelligence

For an individual vacancy, JobHunter should eventually provide an explainable application dossier containing:

### Employer side

- exact job identity and freshness;
- role purpose;
- responsibilities;
- required/preferred/contextual requirements;
- explicit experience/education/location/language/legal constraints;
- important inferred supporting capabilities, clearly labeled;
- representative evidence excerpts.

### Ali side

- matching Career-approved evidence;
- assistance and transfer limits;
- relevant gaps;
- unsupported requirements;
- hard or likely constraints;
- evidence uncertainty.

### Decision support

Use qualitative outcomes such as:

- credible target;
- reasonable stretch;
- low-priority stretch;
- currently blocked;
- not aligned;
- insufficient information.

Explain why.

Do **not** use a single opaque readiness percentage as the primary decision.

## 15. Vacancy prioritization

JobHunter should allow prioritization based on Career objectives rather than keyword similarity alone.

Potential decision dimensions include:

- responsibility fit;
- evidence fit;
- gap size;
- role-family priority;
- learning value;
- mentorship/team signals;
- junior accessibility;
- geographic feasibility;
- work mode;
- freshness;
- employer constraints;
- application effort;
- strategic optionality.

The user should be able to inspect and override any weighting.

## 16. CV tailoring support

For each serious application, JobHunter should produce a **CV Tailoring Pack**, not silently rewrite the master CV.

The pack should include:

- employer language worth reflecting when Ali has evidence for it;
- which verified skills should be moved higher;
- which projects are most relevant;
- which project bullets map to stated responsibilities;
- which truthful transferable-business examples matter;
- which unsupported keywords must not be added;
- suggested headline/summary emphasis;
- likely ATS terminology variations;
- gaps to prepare for rather than conceal.

Career remains authoritative for final résumé claims.

## 17. Interview preparation support

For a job or role family, JobHunter should generate an evidence-backed **Interview Preparation Pack** containing:

- recurring responsibility areas;
- likely technical topics derived from actual requirements;
- likely practical tasks;
- project-defense topics Ali should be able to explain;
- changed-case and debugging exercises;
- behavioral themes from employer responsibilities;
- missing areas that require honest disclosure;
- representative employer wording and evidence references.

Avoid generic interview-question dumps unrelated to the sampled roles.

## 18. Market-change intelligence

With enough longitudinal data, JobHunter should identify meaningful changes such as:

- rising or falling requirement frequency;
- changes in required versus preferred status;
- new technology combinations;
- shifts in role-title language;
- shifts in entry-level experience expectations;
- geography/work-mode changes;
- responsibilities moving from specialist roles into general software roles;
- emerging role archetypes;
- declining or increasingly niche titles.

Trend outputs must include baseline windows, sample sizes, source changes, and uncertainty so source/sampling changes are not mistaken for market change.

## 19. Search-effectiveness intelligence

JobHunter should explain which searches actually contribute useful new jobs.

Desired metrics include:

- distinct jobs found;
- unique contributions beyond other searches;
- overlap rate;
- relevant-job yield after semantic review;
- role-family yield;
- geography yield;
- stale/low-value search detection;
- blind-spot candidates.

This allows the acquisition strategy itself to improve over time.

## 20. Advanced Career-support features

These are desirable when enough trustworthy data exists.

### Skill adjacency and substitution graph

Show relationships such as:

- technologies often requested as alternatives;
- capabilities that transfer across role families;
- tool substitutions around the same responsibility;
- foundational capabilities that unlock multiple technologies.

### Capability bundle analysis

Identify recurring bundles such as:

```text
Python + SQL + APIs + testing
```

or:

```text
Python + LLM APIs + RAG + evaluation + Docker
```

This is more useful than isolated skill counts.

### Learning-return analysis

Estimate which bounded capability investments potentially unlock the largest realistic role set, while exposing assumptions.

### Evidence-return analysis

Identify cases where Ali may not need substantial new learning but does need a stronger project demonstration, test, explanation, deployment, or documented result.

### Career-path adjacency

Estimate which currently accessible role families preserve optionality toward longer-term AI, data, ML, and secure-engineering goals.

### Role ladder inference

Compare adjacent seniority levels to identify what responsibilities appear to change between trainee/junior, junior, and mid-level roles.

### Title drift

Detect when titles change while underlying responsibilities remain similar, preventing Career from chasing fashionable labels.

### Employer-language vocabulary

Maintain a source-backed vocabulary of common employer phrases so CV/interview language can reflect the market without inventing capabilities.

### Counterfactual gap analysis

Support questions such as:

- if Ali gained solid SQL evidence, which additional realistic jobs become plausible?
- if Docker remained only introductory, how many target roles are actually affected?
- if a degree constraint excludes a set of roles, which comparable role families remain?

### Portfolio coverage matrix

Map current portfolio evidence against recurring market responsibilities and show over-covered and under-covered areas.

### Curriculum-drift guard

Warn when current learning/project effort is moving toward low-demand advanced breadth while repeated employment-critical gaps remain unresolved.

### Market-diversification check

Warn when Career conclusions depend too heavily on one source, company type, geography, or narrowly constructed search profile.

## 21. Required Career-facing artifacts

JobHunter should eventually be able to export stable, versioned machine-readable data plus concise human-readable reports for at least these products.

### Market Evidence Snapshot

Contains:

- snapshot ID/date;
- sources and search scope;
- time window;
- analyzed sample and exclusions;
- role-family/archetype distribution;
- recurring responsibilities;
- recurring requirements;
- important constraints;
- quality/uncertainty summary;
- representative source references.

### Role Family Profile

Contains:

- role/archetype definition;
- sample size;
- titles observed;
- responsibilities;
- requirement matrix;
- experience/seniority distribution;
- geography/work mode;
- representative vacancies;
- uncertainties.

### Requirement Demand Matrix

Contains canonical concept, aliases, distinct-job count/share, required/preferred/contextual/inferred distribution, role-family distribution, geography, seniority, trend, and evidence references.

### Responsibility Matrix

Contains normalized responsibility, distinct-job demand, ownership/depth signals, linked deliverables, linked concepts, role families, geography, seniority, and representative evidence.

### Ali Gap Map

Contains market responsibility/requirement, Career-approved Ali evidence, assistance/transfer limit, gap type, blocker status, recommendation, and underlying market references.

### Learning Priority Proposal

Contains priority, market basis, Ali gap basis, expected career effect, smallest useful next evidence, uncertainty, and review decision.

### Project Evidence Opportunity Map

Maps recurring market responsibilities to current evidence and natural project opportunities without prescribing implementation.

### Application Dossier

One vacancy with employer evidence, Ali evidence, gaps, constraints, qualitative application decision, CV emphasis, and interview preparation topics.

### CV Tailoring Pack

Role/job-specific terminology and evidence mapping without modifying the master CV automatically.

### Interview Preparation Pack

Role/job-specific technical, practical, project-defense, and behavioral preparation derived from actual postings.

### Market Change Report

Compares equivalent windows and distinguishes real market change from source/search/sample change.

### Search Coverage and Data Quality Report

Explains what was searched, what was missed, source health, parser/translation/analysis coverage, duplicate handling, and confidence limits.

## 22. Export and integration interface

Career should not need to scrape JobHunter's HTML UI or reverse-engineer its SQLite schema.

JobHunter should eventually expose stable, versioned exports or a local read API for Career-facing artifacts.

Preferred characteristics:

- JSON for machine use;
- Markdown or similarly readable report for human review;
- stable schema/version identifier;
- snapshot/artifact ID;
- generated-at timestamp;
- source time window;
- exact source/job identifiers;
- evidence URLs/references;
- analysis/taxonomy versions;
- quality and uncertainty metadata;
- deterministic regeneration where practical.

The implementation may use CLI, local HTTP API, files, or another simple boundary. The important requirement is a documented, stable contract.

## 23. Review and correction support

Derived outputs need human correction without destroying history.

JobHunter should support:

- accept/reject/correct analysis claims;
- correction reason;
- original and corrected value;
- reviewer/timestamp;
- whether correction is local-only or should inform a deterministic mapping/taxonomy improvement;
- re-analysis under a new model/prompt/schema without deleting the old artifact;
- comparison between versions.

This is especially important before aggregate market conclusions rely heavily on model-derived data.

## 24. Privacy and security requirements

Career-facing integration must remain public-safe by default.

JobHunter should not expose through public Career artifacts:

- phone/address or other private contact details;
- private application notes;
- recruiter correspondence;
- compensation preferences;
- credentials/secrets;
- private personal profile data;
- confidential employer/application material.

If JobHunter later stores private Career inputs, public exports must explicitly sanitize them.

Source acquisition must remain bounded and policy-compliant. Career value never justifies bypassing authentication, CAPTCHA, rate limits, private data boundaries, or source restrictions.

## 25. Acceptance standard for Career use

A JobHunter feature is not useful to Career merely because it runs.

For a Career-facing output to influence a material decision, Career should be able to determine:

1. what sources and jobs produced it;
2. whether the sample is representative enough for the question;
3. which claims are source-explicit versus translated/inferred/normalized;
4. whether duplicates/reposts could inflate the result;
5. whether stale data or source failure matters;
6. what model/taxonomy/calculation version produced it;
7. what uncertainty or missing data remains;
8. whether Ali-specific evidence came from the Career authority rather than repository inference;
9. whether the proposed action follows from a repeated pattern rather than one posting;
10. whether a smaller Career change is sufficient.

## 26. Explicit non-goals and anti-patterns

JobHunter should not become:

- an unrestricted crawler;
- an automated mass-application bot;
- an automatic recruiter-messaging tool;
- a single opaque job-match percentage;
- a keyword-frequency curriculum generator;
- a system that treats every tool mention as equal demand;
- a system that interprets requested years as capability depth automatically;
- a system that infers Ali's capability from GitHub technology names;
- an authority that rewrites Career strategy without review;
- a system that hides source, translation, model, or taxonomy uncertainty;
- a source of false precision from small samples;
- a reason to add technologies artificially to UpgradePilot or another project;
- a substitute for actual applications and interview feedback once Career reaches that stage.

## 27. Priority order for future JobHunter implementation

Career need should guide implementation in this order unless JobHunter has a technical dependency requiring a different internal sequence.

### Highest Career value

1. trustworthy multi-source acquisition and representative sampling;
2. stable source identity, provenance, versions, lifecycle, deduplication, and repost handling;
3. evidence-backed responsibility and requirement extraction;
4. reviewed concept normalization/taxonomy;
5. role-family/archetype and market aggregate views;
6. data-quality, sample-bias, and uncertainty reporting;
7. stable Career-facing exports.

### Next Career value

8. Career capability snapshot import;
9. explainable requirement/responsibility-to-evidence mapping;
10. gap classification and blocker reasoning;
11. role/application prioritization;
12. CV Tailoring Packs;
13. Interview Preparation Packs;
14. Project Evidence Opportunity Maps;
15. learning-priority proposals.

### Later, after adequate longitudinal evidence

16. trend/change intelligence;
17. role-ladder inference;
18. skill adjacency/substitution graphs;
19. counterfactual gap analysis;
20. learning/evidence return analysis;
21. career-path adjacency and optionality analysis.

This is a Career-value priority, not a JobHunter implementation roadmap.

## 28. Success condition

JobHunter is successful for Career when it materially improves decisions such as:

> "SQL should move ahead of Kubernetes because it is repeatedly required across three realistic target role families, Ali currently lacks defensible SQL evidence, and a bounded relational-data responsibility could unlock both capability and application options."

or:

> "Do not add another framework to UpgradePilot; the sampled market asks for API design, testing, debugging, and SQL more often than the proposed technology, and those responsibilities can be demonstrated with less project scope."

or:

> "This vacancy is a reasonable stretch: the core Python/API responsibilities are supported, Docker is preferred rather than required, SQL is a material gap, and the degree requirement is not explicit. Tailor the CV toward UpgradePilot and prepare SQL/API questions rather than hiding the gap."

The desired output is not more data. It is **better, evidence-bounded Career judgment**.
