# A3 Extension — Iran / Persian Employment Market Calibration

**Date:** 2026-09-07  
**Status:** REVISED COMPREHENSIVE PASS — bounded current-market evidence complete for the Day-60 review horizon  
**Owner:** Career market-calibration evidence; not a strategy, capability, or application-readiness owner  
**Parent A3:** `2026-09-07_A3_CURRENT_EMPLOYMENT_MARKET_CALIBRATION.md`  
**Parent plan:** `../../plans/2026-09-07_DAY50_TO_DAY90_CAREER_REALITY_REASSESSMENT_AND_EXECUTION_PLAN.md`

## 1. Why this revision was necessary

The first Iran/Persian A3 extension was too keyword-led. Searching mainly for labels such as `هوش مصنوعی`, `AI`, or `Python` can badly distort the Iranian market picture because:

- AI keywords are used in both genuine engineering roles and non-engineering content/design/marketing roles;
- many roles relevant to an AI-era engineering career do **not** contain `AI` in the title;
- testing, systems analysis, implementation/support, SRE/DevOps, data engineering, backend integration, security and technical-support roles may build the exact verification/integration/operations responsibilities that remain valuable when implementation is increasingly AI-assisted;
- Iranian employers frequently use broad titles such as `کارشناس`, `تحلیلگر`, `پشتیبان`, `استقرار`, or English engineering titles whose real responsibility must be read from the description;
- one employer can expose several adjacent routes at once, making company-level sampling more informative than isolated keyword counts.

This revision therefore treats the Iranian market as a **role-architecture problem**, not an AI-keyword-count problem.

## 2. Market questions

This revision asks:

1. What technical responsibility families are actually visible in current/recent Persian-market hiring?
2. Which of those families provide plausible entry or early-career paths rather than only specialist/senior opportunities?
3. How often is AI embedded into backend, data, automation or product responsibilities rather than isolated in an `AI Engineer` title?
4. Which responsibilities repeatedly survive across the market even when AI tooling changes — programming, SQL/data, testing, debugging, systems analysis, operations, deployment, security, communication, business translation?
5. Does the Iranian market support Ali's anchored-hybrid hypothesis, or does it still screen mainly through one technical specialty?
6. Which entry-access filters matter locally: years of experience, degree, university pedigree, military-service status, gender, city/on-site requirements, or employer-specific constraints?
7. Which domestic roles could later become realistic Career bands for Ali if A4 shows sufficient evidence?

This file still does **not** decide Ali's capability, application readiness, salary target, geography priority or Career identity.

## 3. Sampling method

### 3.1 Primary requested platforms

- **Jobinja** — `https://jobinja.ir/`
- **JobVision** — `https://jobvision.ir/jobs`
- **IranTalent** — `https://www.irantalent.com/jobs`
- **e-estekhdam** — `https://www.e-estekhdam.com/`

### 3.2 Search architecture

Instead of only searching for technologies, the revised pass sampled responsibility families:

```text
A. software / backend / product engineering
B. data / BI / data engineering
C. QA / software testing / verification
D. DevOps / SRE / NOC / Linux / cloud operations
E. systems analysis / ERP / implementation / technical support
F. AI / ML / LLM / agents / automation
G. security / penetration testing / security operations adjacency
H. junior / internship / early-career routes
```

Searches used Persian and English title variants, current company hiring pages, platform categories, current daily feeds, related-job surfaces and direct descriptions where recoverable.

### 3.3 Freshness tiers

Use evidence proportionately:

- **Tier 1 — current / very fresh:** today through approximately 14 days;
- **Tier 2 — recent:** approximately 15–45 days;
- **Tier 3 — structural/supporting:** older current-ish or recently closed material useful for responsibility shape, not for current vacancy counts.

Do not infer current market frequency from Tier-3 examples.

### 3.4 Evidence-strength rule

```text
current full job description
→ responsibility + requirement + access-gate evidence

current employer/company jobs page
→ role-family / employer-demand evidence

current official platform feed/title
→ vacancy existence / taxonomy evidence only

salary report / category page
→ salary/category context only for its stated level

older/closed role
→ structural comparison only
```

### 3.5 Duplicate and selection control

- repeated Telegram/feed appearances of the same vacancy count as one vacancy;
- similar titles at the same employer are kept separate only when they represent distinct responsibility bands;
- keyword counts are not treated as market prevalence;
- the sample is targeted and convenience-based, not a statistically random Iranian labor-market survey;
- conclusions are therefore qualitative and bounded to the observed role architecture.

---

# 4. Platform-by-platform findings

## 4.1 Jobinja — strongest direct responsibility evidence in this pass

Jobinja is particularly useful because company pages and many detailed job descriptions are directly recoverable. The revised pass therefore used **company-led sampling** rather than broad keyword counts.

### Irancell Labs — one employer exposes the engineering stack

A recent active Irancell Labs page showed roles including:

- NOC Engineer — today;
- Senior Software Engineer — 14 days;
- Data Platform Technical Lead — 15 days;
- Operation Engineer — 20 days;
- QC Engineer — 20 days;
- Business Analyst — 40 days;
- Data Engineer — 41 days;
- DevOps Engineer — 50 days.

Its expired history additionally includes SRE, DevSecOps, backend, cloud infrastructure, big-data engineering, QA/software testing, platform engineering, data science and AI-management roles.

**Meaning:** a serious technology employer is not organized around one title such as `AI Engineer`. It needs a connected system of software, data, operations, quality, analysis, infrastructure and security responsibilities.

### Fanavaran — AI beside SRE, systems analysis and internship

A recent Fanavaran company page showed, in the same hiring surface:

- SRE;
- SRE Operations Engineer;
- AI Engineer;
- SysAdmin;
- C# programming internship;
- React;
- software systems analyst;
- full stack;
- DBA.

This is important because it exposes **entry, software, infrastructure, data and AI** lanes simultaneously.

#### Fanavaran AI Engineer — deep AI systems role, not junior

The detailed role requires 3–6 years and combines:

- GenAI;
- RAG;
- Chain/Agent systems;
- prompt engineering;
- instruction tuning/domain adaptation;
- LLM evaluation for hallucination, consistency, accuracy and latency;
- guardrails/error control;
- vLLM/Ollama/Docker deployment;
- cost and latency optimization;
- production monitoring;
- API/microservice/database integration;
- data-preprocessing pipelines.

This is strong evidence that Iranian AI engineering can already mean **full lifecycle AI systems engineering**, not only model experimentation or prompting.

It is equally strong evidence that serious AI-engineer titles may remain **experienced-role targets**, not an immediate beginner lane.

#### Fanavaran Software Systems Analyst — highly relevant non-AI hybrid role

The same employer's systems-analyst role requires 3–6 years and includes:

- customer requirement discovery;
- project/repository setup;
- root-cause analysis of reported bugs;
- proposing fixes;
- defining acceptance-test criteria;
- documentation;
- software lifecycle understanding;
- initial/basic testing;
- ERD/data-model understanding;
- Scrum, JSON, UML, BPMN;
- troubleshooting;
- systems thinking;
- cross-team communication.

This role is important to the Career review because many of these responsibilities map directly to the **human judgment/integration layer** identified in A2 even though the title contains neither AI nor Python.

### Wallex — conventional backend remains deep and cross-functional

A recent Python Backend Developer role at Wallex/WallGold is explicitly a 3–6-year role. It combines:

- Python + Django/Flask;
- REST APIs;
- scalable/secure backend design;
- relational databases/SQL;
- Redis/Celery/message brokers;
- observability;
- unit/integration tests;
- code review;
- Docker/Git/CI/CD;
- security and data integrity;
- distributed/microservice/event-driven concerns;
- cross-functional work with frontend, DevOps, product and QA.

**Meaning:** even where AI can generate much of this code, employers still organize responsibility around engineering ownership across APIs, data, reliability, testing and operations.

### ParsPack — technical support/operations as a real adjacent engineering lane

A recent Linux hosting support role is under three years in Jobinja metadata, though the description asks for at least two years of system-administration experience. It includes:

- ticket-based user support;
- log analysis and failure diagnosis;
- DNS/mail/CMS/backup/domain/SSL/database troubleshooting;
- Linux administration;
- web-server and database operation;
- virtualization/cloud familiarity;
- monitoring;
- Bash scripting;
- networking;
- time-sensitive problem resolution.

This is not a coding-heavy role, but it develops **diagnosis, systems thinking, production operations and user-facing technical responsibility** — capabilities that A2 treats as increasingly valuable in an AI-heavy engineering environment.

### Genuine Junior AI evidence exists — but can carry academic gates

A recent Junior AI Engineer posting at Najm was explicitly entry-level and said extensive experience was not required. It expected candidates to start with small, defined tasks and grow alongside experienced teammates.

Responsibilities included:

- NLP;
- semantic search;
- LLMs;
- AI agents/chatbots;
- text-data work;
- training/evaluating/optimizing models;
- integration with software products;
- reading/applying papers.

However, the role also explicitly targeted students/graduates of top Iranian universities in computer/AI-related disciplines.

**Meaning:** true junior AI routes exist in Iran, but they may be gated by academic pedigree even when years-of-experience requirements are low.

### Early-professional data/business hybrid evidence

A Commercial Data Analyst posting at SnappShop is under three years in metadata and asks for about two years of analytics/BI experience. It combines:

- SQL mandatory;
- Python as a plus;
- KPIs/dashboards/automated reports;
- root-cause analysis;
- data quality;
- collaboration with data engineering/product;
- business/stakeholder translation.

This is another important non-AI title: it rewards a bounded hybrid of **data + business judgment + communication + technical analysis**.

### Jobinja calibration

Jobinja supports a broad conclusion:

> Iranian technical hiring is a connected responsibility system, not an AI-keyword market.

The strongest observed lanes include software/backend, data, QA/QC, SRE/operations, systems analysis, infrastructure/support and AI engineering. Entry opportunities exist, but the deepest AI/data/backend roles frequently remain experience-heavy.

---

## 4.2 JobVision — strongest current/fresh taxonomy signal

JobVision's public jobs page is dynamic and does not expose all current role descriptions reliably to the research tools. Its official current Telegram feed is therefore useful for **fresh vacancy/title evidence**, while descriptions should not be invented when the detail page is inaccessible.

### Current feed: AI embedded inside other engineering responsibilities

A very recent official feed simultaneously showed:

- penetration-testing/security specialist;
- **Data Engineer – Feature Store & AI Pipelines**;
- Senior Backend Developer – OMS Architect;
- **Backend Developer – OMS & AI Integration**.

This is a major improvement over an AI-keyword search. It shows that current Iranian employers are embedding AI directly into:

```text
data infrastructure
backend integration
production systems
```

rather than isolating all AI work in `AI Engineer` titles.

### Current SRE / DevOps / infrastructure demand

Recent JobVision feeds also show:

- Site Reliability Engineer (SRE);
- DevOps Engineer;
- infrastructure DevOps engineer;
- Senior SRE.

These roles establish ongoing demand for production reliability and operations responsibilities, even though they are not AI-labeled.

### Current software / Python demand

Recent feeds include:

- Python developer in quantitative/finance domain;
- backend Python/Django roles;
- full-stack roles;
- junior backend examples;
- Python/MQL programming internship.

The important signal is not one framework. It is that the conventional programming substrate still supplies entry and professional routes alongside AI-specific titles.

### Current QA / testing evidence

Recent JobVision feed evidence includes QA Engineer roles. This matters because testing is one of the strongest recurring responsibilities in the international A3 and one of the A2 high-value human layers.

### Current data / BI evidence

Recent feeds include:

- Data Engineer;
- Data Engineer – Feature Store & AI Pipelines;
- Power BI specialist;
- senior data-analysis roles.

### JobVision calibration

The current JobVision surface supports this interpretation:

> AI is becoming an **adjacency embedded in software/data systems**, while QA, SRE/DevOps, backend, data and security remain distinct hiring lanes.

It also supports keeping entry pathways broader than `Junior AI Engineer`: internships, junior backend and other adjacent roles can provide meaningful technical-entry routes.

---

## 4.3 IranTalent — strongest structured category/seniority context

IranTalent is useful not only for individual jobs but because its market architecture exposes how employers and candidates are categorized.

Its current jobs page includes categories such as:

- cybersecurity / information security;
- data analysis / market analysis / economic analysis;
- IT/software/programming;
- business operations/process improvement;
- project management;
- product management;
- network/IT engineering;
- installation/implementation;
- AI/ML/automation.

It also exposes seniority filters including intern, employee/expert, senior expert, middle management and executive, plus education filters including a no-university-education option.

**Meaning:** the market itself recognizes a broad technical/implementation architecture rather than one narrow AI lane.

### Current/recent roles that a keyword-only pass would miss

Recent IranTalent surfaces included titles such as:

- IT ERP Technical Support Engineer;
- IT ERP Functional Support Engineer;
- software-development roles;
- Python Developer;
- AI-related product/management/development roles.

ERP/support/implementation responsibilities are particularly relevant to Ali's later role-family review because they can combine:

```text
technical systems
+ business process understanding
+ user/stakeholder interaction
+ troubleshooting
+ implementation ownership
```

without demanding a pure research/algorithmic identity.

### Junior Python market context

IranTalent's 1405 Junior Python/Django report gives a useful responsibility checklist rather than only salary data. It explicitly tells junior candidates to evaluate whether a job involves:

- real Python/Django backend work;
- API development;
- database/query writing;
- tests;
- Git/code review;
- senior/tech-lead mentorship.

At the sampled moment, the page showed no exact active match for its selected junior category and surfaced nearby roles instead. That is important negative evidence: a broad salary category does **not** imply abundant live junior vacancies at every moment.

### AI/Data salary category context

IranTalent's 1405 `کارشناس` Data Science / AI category reports a Tehran median requested net salary of roughly **50 million toman/month**, with a middle 50% around **37–71 million toman**. The category covers titles including AI Engineer, ML Engineer, Data Scientist, NLP and Computer Vision roles.

For comparison, the Junior Python/Django category reports a Tehran median requested net salary around **36 million toman/month**, middle 50% about **27–44 million**.

These figures must **not** be used to claim a simple AI salary premium because the seniority categories differ (`کارشناس` versus explicit Junior).

### IranTalent calibration

IranTalent strengthens two conclusions:

1. AI/data is a real professional category with meaningful compensation and role diversity.
2. The domestic technical market also contains implementation/support/process/software roles that may be more accessible or more aligned with an anchored-hybrid first-job strategy than chasing an AI title alone.

---

## 4.4 e-estekhdam — broad private + formal-enterprise route evidence

e-estekhdam differs from the other platforms because it exposes both private-company hiring and more formal institutional/bank recruitment channels.

### Current/recent software-test evidence

Recent official feed evidence includes:

- software-test specialist roles;
- software/hardware test technician roles;
- companies hiring software-testing specialists alongside Java/.NET/Oracle developers.

This strengthens the case that **verification/testing is itself a real employment lane**, not merely a supporting activity inside development.

### Systems analysis / implementation / support

Recent e-estekhdam evidence includes:

- software/system analyst;
- business analyst;
- software support;
- systems/methods specialist;
- software deployment/implementation specialist.

One multi-province software-company advertisement included `تحلیلگر سیستم` and said initial training would be provided after selection. Another current/recent large company hiring surface included analyst, Linux admin, software test, Java, .NET and CRM responsibilities together.

These roles are strategically important because they can reward:

- requirement analysis;
- business-process understanding;
- troubleshooting;
- acceptance/validation;
- implementation/support;
- technical communication.

### AI evidence

Recent/current official feed evidence also includes experienced AI-specialist hiring, including roles responsible for designing/developing/deploying AI models and integrating them into products/services.

The existence of AI roles does not remove the broader software/analysis/support structure around them.

### Formal institutional hiring can impose much harder gates

Recent 1405 formal bank/enterprise recruitment evidence shows technology roles such as:

- programmer;
- IT security;
- systems analyst;
- BI;
- support;
- DevOps;
- database/Oracle.

But some of these routes impose hard filters such as:

- bachelor's/master's degree;
- GPA thresholds;
- approved-university criteria;
- locality/residency requirements;
- other formal recruitment conditions.

This is a materially different access model from a startup/company role that may accept portfolio evidence.

### e-estekhdam calibration

Iran is not one homogeneous hiring channel. Career should distinguish at least:

```text
private/startup/product-company hiring
vs
large enterprise/vendor hiring
vs
formal bank/institutional recruitment
```

because their entry gates can differ more than their technical stack.

---

# 5. Responsibility-family map

## 5.1 Software / backend / product engineering

### Current/recent evidence

Visible examples include:

- Python backend;
- Python/Django;
- full stack;
- Java/.NET/C#;
- backend + AI integration;
- quantitative Python;
- software engineer;
- software/product engineering.

### Recurrent responsibility shape

Where descriptions are available, roles tend to combine:

- APIs;
- databases;
- tests;
- Git/code review;
- security/reliability;
- deployment/operations collaboration;
- problem solving/debugging.

### Career meaning

A programming/software substrate remains important even in the AI-heavy market. What appears weaker is **manual implementation speed as the sole differentiator**, not software understanding itself.

---

## 5.2 Data / BI / data engineering

### Current/recent evidence

- Data Engineer;
- Feature Store & AI Pipelines;
- data platform;
- Commercial/Business Data Analyst;
- Power BI;
- data science + AI.

### Recurrent responsibility shape

- SQL;
- data modeling;
- data quality;
- pipelines;
- dashboards/analytics;
- root-cause analysis;
- business translation;
- in deeper engineering roles: Spark/Kafka/Airflow/OLAP/storage/monitoring.

### Career meaning

SQL/data remains a major cross-role capability. Data engineering itself often skews more experienced, while analyst/data-business roles may offer somewhat earlier entry points.

---

## 5.3 QA / testing / verification

### Current/recent evidence

- QA Engineer;
- QC Engineer;
- software test specialist;
- software/hardware test technician;
- historical/current automation-test patterns.

### Recurrent responsibility shape

- test execution;
- quality verification;
- regression/acceptance thinking;
- defect reporting;
- troubleshooting;
- collaboration with development/product teams.

### Career meaning

This lane is strategically more important in the AI era than a keyword-only search would reveal. Strong AI agents can increase output volume, which increases the value of people who can determine whether the output is correct, safe and acceptable.

QA/test roles should therefore remain part of A7's role-family consideration, even if they are not the preferred long-term identity.

---

## 5.4 DevOps / SRE / NOC / Linux / cloud operations

### Current/recent evidence

- SRE;
- SRE Operations Engineer;
- DevOps Engineer;
- infrastructure DevOps;
- NOC Engineer;
- Linux support;
- Operation Engineer;
- SysAdmin.

### Recurrent responsibility shape

- monitoring;
- incident/failure response;
- logs;
- infrastructure/service reliability;
- Linux/networking;
- deployment;
- troubleshooting;
- production operations.

### Career meaning

These roles often require deeper infrastructure experience than Ali currently has, but they strongly validate A2's thesis that **diagnosis, observability and operational responsibility** remain durable human-value layers.

Cloud/Kubernetes should not automatically become a new learning track; these are evidence about responsibility value first.

---

## 5.5 Systems analysis / ERP / implementation / support

This was one of the most important findings missed by the first Iran pass.

### Current/recent evidence

- software systems analyst;
- business analyst;
- systems/methods specialist;
- ERP Technical Support Engineer;
- ERP Functional Support Engineer;
- deployment/implementation specialist;
- software support;
- Linux/hosting support.

### Responsibility shape

Where descriptions are available, these roles can involve:

- requirements discovery;
- business-process understanding;
- system/process modeling;
- root-cause debugging;
- acceptance-test criteria;
- documentation;
- user/customer interaction;
- implementation/deployment;
- troubleshooting;
- data-model understanding;
- communication between business and technical teams.

### Career meaning

This is potentially a **high-value role family for later Career review** because Ali has prior management/sales/purchasing/operational experience that may eventually support business-process translation, while his technical transition can supply software/data/AI understanding.

This does **not** mean Ali is qualified today. It means the market contains a bridge between his prior professional history and his technical direction that a pure `Junior Python`/`AI Engineer` search would miss.

---

## 5.6 AI / ML / LLM / agents / automation

### Current/recent evidence

Visible titles/responsibilities include:

- AI Engineer;
- Junior AI Engineer;
- Data Science + AI;
- LLM-related engineering;
- AI/agent specialist;
- AI automation/deployment;
- AI software development;
- Feature Store & AI Pipelines;
- Backend + AI Integration.

### Responsibility shape

The deeper roles combine:

- model/LLM work;
- RAG/agents;
- evaluation;
- guardrails;
- deployment;
- latency/cost;
- production monitoring;
- APIs/microservices;
- databases;
- data pipelines;
- software engineering quality.

### Career meaning

The domestic market supports **applied AI systems engineering**, but many serious roles are not junior. The strongest entry hypothesis remains:

> credible software/data/testing substrate + AI/agent project evidence + ability to learn/grow under stronger engineers.

---

## 5.7 Security / penetration testing / secure engineering adjacency

Current JobVision evidence includes penetration-testing/security roles, while larger technology employers expose DevSecOps/security-team history and information-security categories.

### Career meaning

Security remains a real adjacent market, but A3 does not justify broadening Ali into a separate security-specialist route before A4/A7. The stronger immediate use is as a **cross-cutting engineering responsibility**: permissions, security boundaries, secure APIs/data, infrastructure and trustworthy AI behavior.

---

# 6. Entry-access map

A better Iran analysis must distinguish role existence from **entry accessibility**.

## 6.1 Tier E0 — genuine internship / first-step routes

Observed examples include:

- programming internship;
- Python/MQL internship;
- C# programming internship;
- historical/recent AI internship/junior roles;
- support/implementation internships in some enterprise-company hiring surfaces.

These are the clearest low-experience routes, but can still impose student/university/background conditions.

## 6.2 Tier E1 — junior / early professional

Observed examples include:

- Junior AI Engineer;
- junior backend;
- early data/business analyst;
- technical support/Linux support;
- some QA/testing roles;
- implementation/support roles.

Typical access pattern can still include:

- 0–2 years or roughly <3 years;
- relevant degree;
- top-university preference for some AI roles;
- 1–2 years practical experience despite a relatively junior title;
- military-service status or age/gender filters in some ads.

## 6.3 Tier E2 — professional specialist

Many visible roles labeled simply `کارشناس`, `AI Engineer`, `Data Engineer`, `Systems Analyst`, backend or SRE actually ask for approximately 2–6 years and meaningful ownership.

This appears to be a large part of the serious technical market.

## 6.4 Tier E3 — senior/lead

Senior backend, senior data, technical leads, architecture, senior SRE and advanced AI/ML roles remain clearly separate.

### Entry conclusion

Iran has real entry routes, but:

> **title modernity does not imply junior accessibility.**

A current `AI Engineer` may be a 3–6-year lifecycle role, while a less fashionable `support`, `QA`, `systems`, or internship title may provide the more realistic first professional engineering entry.

---

# 7. Access and eligibility filters specific to the Iran sample

## Experience

Experience requirements vary from none to 5+ years. They must be checked per vacancy rather than inferred from title.

## Degree and academic pedigree

- many conventional and enterprise roles require bachelor's degrees;
- some AI roles explicitly prefer/require students or graduates of top Iranian universities;
- IranTalent's platform taxonomy itself allows filtering for no university education, showing that the whole market is not degree-gated;
- formal bank/institutional recruitment can impose especially strict degree/university/GPA conditions.

## Military service

Some private listings explicitly require completed/permanent exemption; others mark it unimportant. Knowledge-based-company routes may offer alternative-service opportunities for eligible candidates.

## Gender / age

Some Iranian postings still explicitly specify gender or age ranges. Treat these as vacancy-specific access filters, not Career capability evidence.

## Geography and work mode

- Tehran remains heavily represented;
- current technical roles also appear outside Tehran and in multi-province hiring;
- remote roles exist, including technical support and some software work;
- local work mode may reduce international visa barriers but can introduce commute/location constraints.

---

# 8. AI integration is broader than AI titles

The strongest revised finding is:

```text
AI is not merely creating new job titles.
It is being inserted into existing engineering responsibilities.
```

Current examples include:

- **Data Engineer – Feature Store & AI Pipelines**;
- **Backend Developer – OMS & AI Integration**;
- AI Engineer with APIs/microservices/databases/deployment/monitoring;
- software + AI-development titles;
- AI automation/deployment roles.

This is highly relevant to Ali's hypothesis. It suggests that the valuable profile is less likely to be:

> "I know one AI framework"

and more likely to be:

> "I can operate a real software/data system and integrate/evaluate AI responsibly inside it."

---

# 9. Specialization vs hybrid breadth — Iran result

The revised Iranian evidence supports a more precise version of the anchored-hybrid model.

## What the market appears to reward

```text
one primary responsibility anchor
+ adjacent systems/data/operations understanding
+ AI leverage where relevant
+ verification/troubleshooting
+ communication/business context
```

Examples:

- backend anchor + AI integration;
- data-engineering anchor + AI pipelines;
- AI anchor + software/deployment/monitoring;
- systems-analysis anchor + bugs/tests/data models/customer requirements;
- support/operations anchor + logs/Linux/networking/databases.

## What the evidence does not support

- being a shallow generalist with no defendable anchor;
- learning many unrelated technologies because AI makes them easier;
- replacing programming/data/system fundamentals with prompting;
- assuming a broad AI title removes the need for depth.

### Best interpretation

Ali's original intuition is **partly validated**:

> broader integration capability is becoming useful.

But the domestic market still appears to hire through a recognizable anchor:

> backend, data, AI, QA, systems/implementation, or infrastructure.

Therefore the more resilient model remains:

> **anchored hybrid, not generic generalist.**

---

# 10. Iran vs UAE/Europe — important contrasts

## Shared technical direction

Across the international and Iranian samples, the stable responsibility pattern is similar:

```text
software/programming substrate
+ APIs/integration
+ data/database competence
+ testing/debugging/evaluation
+ operations/reliability awareness
+ AI/LLM/agent capability where relevant
+ communication/problem translation
```

## Iran-specific advantages

Potentially fewer barriers around:

- foreign work authorization;
- visa sponsorship;
- UAE-national graduate restrictions;
- country-specific European residency requirements.

There are also explicit internship/junior routes and domestic product companies where Persian business/domain understanding can matter.

## Iran-specific constraints

- many serious technical roles still ask for 2–5+ years;
- Tehran concentration;
- some gender/age/military-service filters;
- some AI roles strongly prefer academic pedigree;
- formal institutional routes may be more credential-heavy than startup/private-company hiring;
- compensation, currency, team quality and mentorship require vacancy-specific review.

### Cross-market implication

The major difference may be **access architecture**, not the engineering direction itself.

---

# 11. Salary context — keep separate from role-fit

IranTalent 1405 data provides useful but non-equivalent benchmarks:

### Junior Python/Django — Tehran

- median requested net: approximately **36M toman/month**;
- middle 50%: approximately **27–44M**.

### Data Science / AI — `کارشناس` — Tehran

- median requested net: approximately **50M toman/month**;
- middle 50%: approximately **37–71M**.

These should **not** be used to claim that AI pays a fixed premium because they compare different level labels.

For a first role, Career should prioritize:

1. actual responsibility;
2. technical mentorship/code review;
3. opportunity to build transferable evidence;
4. team/product quality;
5. access feasibility;
6. then compensation relative to matched market level.

---

# 12. Revised Iran/Persian role-family implications for later A7 review

These are market hypotheses only. A4 must compare Ali's evidence before any role family is activated.

## High strategic relevance

### 1. Applied AI / AI Application / AI Integration Engineer

Why:
- real domestic AI/LLM/agent demand;
- AI increasingly embedded in backend/data systems;
- matches the A2 direction.

Caution:
- serious roles often require experience;
- entry AI can be academic-pedigree gated.

### 2. Technical Implementation / Systems / AI Solutions / Automation

Why:
- systems analysis, implementation/support, ERP, automation and cross-team roles are visible;
- combines technical systems with business/process translation;
- may eventually leverage Ali's prior business/operational experience better than a narrow coding-only narrative.

Caution:
- many systems-analysis roles still ask for 2–3+ years;
- exact junior/trainee accessibility must be sampled vacancy by vacancy.

### 3. Python Backend / Data-Adjacent Engineering

Why:
- strong conventional substrate;
- APIs/DB/tests/Git/reliability are portable into AI application roles.

Caution:
- many visible product-company backend roles are mid/senior.

### 4. Data / Analytics / Data Engineering

Why:
- SQL/data quality/business interpretation recur strongly;
- AI pipelines increasingly connect to this lane.

Caution:
- deep data engineering often requires production experience;
- analyst roles can be earlier-entry but may require SQL/business experience.

## Worth keeping as adjacent entry bands

### QA / Software Testing / Test Automation

Potentially useful because it develops verification, failure analysis and engineering collaboration — exactly the scarce layer identified in A2.

### Technical Support / Linux / Implementation Support

Potentially useful when the role provides real technical diagnosis, logs, systems, networking/databases and mentorship rather than call-center-only support.

### Systems / Business Analyst with technical responsibilities

Potentially valuable bridge for Ali's prior professional experience if the role genuinely includes software/data/process responsibility.

## More conditional

### Pure ML / research-heavy AI

Exists domestically, but many roles require deeper math/ML/research background or academic pedigree. It should not automatically become the first-entry priority.

### SRE/DevOps/Cloud infrastructure

Strong market value but usually a deeper operational responsibility. Better treated as an adjacent literacy layer unless A4/A7 reveals a realistic entry route.

---

# 13. What this revised study changes from the first Iran pass

The first extension mainly established that Iran has AI/LLM/agent demand.

The revised study establishes something more useful:

1. **Iran has multiple technical entry and progression lanes, not one AI market.**
2. **AI is increasingly embedded inside backend and data responsibilities.**
3. **QA/testing, systems analysis, implementation/support and operations are strategically relevant AI-era roles even without AI in the title.**
4. **Serious AI/data/backend roles often remain mid-level despite modern titles.**
5. **Genuine junior AI exists, but can have academic-pedigree gates.**
6. **A less fashionable adjacent role may sometimes be a better first technical entry than chasing an `AI Engineer` title.**
7. **Iran supports anchored-hybrid breadth, but still hires through recognizable responsibility anchors.**
8. **Technical fit and entry-access fit must remain separate, just as in the UAE/Europe sample.**

---

# 14. What this evidence does NOT justify

Do not infer that:

- Iran has an easy junior-AI market;
- any role mentioning AI is engineering work;
- current AI demand makes conventional software/data/testing obsolete;
- QA/support/systems roles are automatically good Career moves — role quality matters;
- Ali is currently qualified for any sampled role;
- a 3–6-year role becomes an entry target because AI assistance exists;
- formal bank/institution hiring rules apply to private startups, or vice versa;
- the salary figures represent guaranteed offers;
- Iran should replace UAE/Europe as Career priority before A4/A7.

---

# 15. Evidence register

## Jobinja

- Irancell Labs active jobs: `https://jobinja.ir/companies/irancell-labs-1/jobs`
- Wallex active jobs: `https://jobinja.ir/companies/wallex/jobs`
- Wallex Python Backend Developer: current/recent direct Jobinja role inspected during this pass.
- Fanavaran active jobs: `https://jobinja.ir/companies/fanavaran-5/jobs`
- Fanavaran AI Engineer: current/recent detailed role inspected during this pass.
- Fanavaran Software Systems Analyst: current/recent detailed role inspected during this pass.
- ParsPack active jobs: `https://jobinja.ir/companies/parvasystem/jobs`
- ParsPack Linux hosting support: current/recent detailed role inspected during this pass.
- Najm Junior AI Engineer: recent detailed role, used as Tier-2/3 entry-pattern evidence rather than current-volume evidence.
- SnappShop Commercial Data Analyst: recent detailed role, used as early-professional data/business evidence.
- Irancell Labs Data Engineer: recent detailed description used to show title/seniority mismatch and deep data responsibilities.

## JobVision

- Current official JobVision Telegram feed: `https://t.me/s/jobvision`
- Current observed titles included penetration testing/security, `Data Engineer – Feature Store & AI Pipelines`, `Backend Developer – OMS & AI Integration`, SRE, DevOps, Python and other engineering roles.
- Direct JobVision job detail pages were not consistently accessible to this research path; title-only observations are therefore not used to infer unshown requirements.

## IranTalent / IranSalary

- Current jobs: `https://www.irantalent.com/jobs`
- Junior Python/Django salary report: `https://salary.irantalent.com/salary-report/python-django-etc-junior-salary/`
- Data Science / AI expert salary report: `https://salary.irantalent.com/salary-report/data-science-ai-expert-salary/`
- Salary-report index: `https://salary.irantalent.com/salary-reports/`

## e-estekhdam

- Main site: `https://www.e-estekhdam.com/`
- Official Telegram feed used for current/recent discovery: `https://t.me/s/eestekhdam_com`
- Current/recent examples inspected included software testing, software/system analysis, implementation/support, Linux/admin/development and AI-specialist hiring.

---

# 16. Combined A3 handoff after the revised Iran study

The combined international + Iran/Persian market evidence now supports a stronger, more precise proposition:

```text
The labor market is not moving from specialists to generic generalists.

It is increasingly rewarding engineers who have
one credible technical anchor
+ adjacent integration breadth
+ strong verification/debugging responsibility
+ AI leverage where useful.
```

For Iran specifically, the possible entry surface is broader than `Junior AI Engineer` and may include:

```text
junior/intern software
QA/testing
technical implementation/support
systems/business analysis with real technical responsibility
backend/data roles
applied-AI integration
```

A4 must now answer which of these Ali can actually defend today and which represent the smallest high-value evidence gaps.

**Next:** A4 — Ali capability/evidence reality against A2 ownership standards and the expanded A3 market map.