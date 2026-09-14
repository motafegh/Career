# Iran / Persian Platform Acquisition and Market Research Report

**Date:** 2026-09-14  
**Status:** Comprehensive source-method + market-evidence report for E3; not a strategy, capability, salary-target, or application-readiness owner  
**Owner:** Career market-calibration evidence  
**Requested primary platforms:** Jobinja, JobVision, IranTalent, e-estekhdam  
**Extends:** [`2026-09-07_A3_IRAN_PERSIAN_EMPLOYMENT_MARKET_EXTENSION.md`](2026-09-07_A3_IRAN_PERSIAN_EMPLOYMENT_MARKET_EXTENSION.md)  
**Companion:** [`2026-09-14_E3_BROAD_RESPONSIBILITY_MARKET_RESEARCH_SYNTHESIS.md`](2026-09-14_E3_BROAD_RESPONSIBILITY_MARKET_RESEARCH_SYNTHESIS.md)

## 1. Purpose

This report answers two connected questions:

1. **How can Career reliably acquire current Iranian / Persian job evidence from the four requested platforms?**
2. **What does the current and recently verified Persian-market evidence say when searched by responsibility family rather than only by AI / Python job titles?**

The acquisition question matters because the four platforms expose materially different web surfaces. Treating them as interchangeable would create false negatives, stale evidence, or misleading market counts.

The market question is deliberately bilingual and responsibility-led.

Use both Persian and English terms because Iranian employers mix:

- Persian job titles;
- English titles;
- Persian descriptions containing English technology names;
- broad labels such as `کارشناس`, `تحلیلگر`, `استقرار`, `پشتیبان`, `سیستم‌ها و روش‌ها`, or `عملیات` that may hide technically relevant responsibilities.

---

## 2. Research principles

### 2.1 Original-source priority

Prefer evidence in this order:

```text
current direct employer / job-detail page
→ current platform listing / company hiring page
→ current category / filtered platform page
→ official platform report / taxonomy
→ current official feed / indexed mirror for discovery only
→ search-engine snippet only when stronger source is unavailable
```

A search-engine crawl date is not equivalent to a vacancy posting date.

### 2.2 Preserve Persian wording

Do not silently normalize Iranian terminology into English titles.

Examples:

```text
کارشناس استقرار
!= automatically "software engineer"

پشتیبان نرم افزار
!= automatically "help desk"

کارشناس سیستم‌ها و روش‌ها
!= automatically "business analyst"
```

Preserve the original title and description first; then add a normalized responsibility interpretation.

### 2.3 Responsibility over keyword

A keyword query answers:

> Which indexed/listed vacancies contain this term?

It does **not** answer:

> What percentage of the Iranian technical market belongs to this profession?

This is especially important for `هوش مصنوعی`, because the term appears in engineering, content, design, teaching, marketing and other non-engineering roles.

---

# 3. Platform acquisition analysis

## 3.1 Jobinja — strongest direct enumerability

### Current observed surface

Direct jobs page:

https://jobinja.ir/jobs

The page was directly readable and exposed:

- title / skill keyword search;
- job category;
- province;
- contract type;
- work-experience filter;
- salary filter;
- special features;
- server-rendered result cards;
- result age;
- company;
- city;
- contract type;
- pagination.

On the September 14 observation, the unfiltered page displayed **14,881 active opportunities**. This number is platform-wide and must not be interpreted as technical-market volume.

The current page also directly surfaced examples such as:

- `برنامه‌نویس Python`;
- `Technical Support`.

### Keyword query behavior

A direct Persian query for `هوش مصنوعی` was recoverable through the jobs page and displayed **328 active results** at the time of observation.

Direct query:

https://jobinja.ir/jobs?filters%5Bkeywords%5D%5B0%5D=%D9%87%D9%88%D8%B4+%D9%85%D8%B5%D9%86%D9%88%D8%B9%DB%8C

Current visible examples included:

- `کارشناس هوش مصنوعی (AI Specialist)`;
- `مهندس هوش مصنوعی گفتار (Speech AI Engineer)`;
- `متخصص هوش مصنوعی`;
- `مهندس هوش مصنوعی`;
- remote and part-time AI-labeled roles;
- non-engineering AI-labelled design / content / teaching roles.

### Critical interpretation rule

The `328` result count is **not** 328 AI-engineering jobs.

The query visibly mixes:

- AI engineering;
- AI specialist roles;
- teaching;
- AI-assisted design / content work;
- other keyword matches.

Therefore Jobinja counts are useful for enumeration and discovery, but every role-family conclusion requires detail-level classification.

### Jobinja filters useful for Career

Particularly useful filters include:

- `کارآموزی`;
- `دورکاری`;
- `کمتر از سه سال`;
- province;
- web/software;
- IT / DevOps / Server;
- support/customer operations;
- research / development;
- business / industrial categories.

### Recommended acquisition method

For each responsibility family:

1. search Persian title / responsibility synonyms;
2. search English synonyms separately;
3. filter to `کمتر از سه سال`, `کارآموزی`, and/or no-experience-limit where relevant;
4. enumerate result pages;
5. open detail pages where retrievable;
6. extract employer-explicit responsibilities and gates;
7. deduplicate same company/title/repost;
8. classify responsibility family only after inspection.

### Current evidence quality

**High for:** listing existence, count within the exact query, company/title/location/age/contract metadata, broad enumeration.  
**Medium for:** full responsibility analysis when detail pages are intermittently difficult to retrieve through automated web tooling.  
**Low for:** neutral prevalence inference from search counts.

Source: https://jobinja.ir/jobs

---

## 3.2 JobVision — rich taxonomy, weaker crawler extraction

### Current observed surface

Direct jobs page:

https://jobvision.ir/jobs

The page exposes a rich filter model including:

- title / company;
- job group;
- city;
- publication time;
- remote work;
- cooperation / employment type;
- internship;
- salary;
- work experience;
- seniority;
- benefits;
- industry;
- special conditions.

JobVision's own page explains that applicants can filter by experience and explicitly references internships / low-experience through higher-experience bands.

### Important crawler behavior

JobVision's `robots.txt` currently contains:

```text
disallow: *?*
```

and publishes a sitemap:

https://jobvision.ir/sitemap.xml

Source:

https://jobvision.ir/robots.txt

This means query-string result URLs should **not** be treated as a reliable general web-crawling surface.

In the text-only environment used for this research, the base jobs page exposed the filter taxonomy and explanatory content but did not reliably expose current result cards.

### Recommended acquisition method

Use JobVision through a hybrid route:

1. native JobVision filtering when interactive access is available;
2. sitemap / indexed detail pages for discovery;
3. direct vacancy pages when URLs are recoverable;
4. employer-authored text from the detail page as the evidence unit;
5. official JobVision feeds / social surfaces only as discovery support;
6. verify posting freshness before counting a job as current.

### What not to do

Do not conclude:

> JobVision has no matching jobs

because a text crawler returns an empty result surface.

That would be an acquisition failure, not market evidence.

### Current evidence quality

**High for:** platform taxonomy / filter semantics.  
**Potentially high for:** individual job detail when directly available.  
**Low for:** automated result-volume counting through public query URLs in this environment.

Source: https://jobvision.ir/jobs

---

## 3.3 IranTalent — strong structured taxonomy + current visible listings + salary context

### Current observed jobs surface

Direct jobs page:

https://www.irantalent.com/jobs

The page was directly readable and exposed **1,602 results** at the observation horizon.

Useful filters include:

- location;
- job group;
- publication time;
- industry;
- organizational level;
- education field;
- gender;
- employment type;
- workplace type;
- urgent hiring and other conditions.

### Especially useful Career job groups

IranTalent explicitly exposes groups including:

- `تحلیل داده / تحلیل بازار / تحلیل اقتصادی`;
- `داده، هوش تجاری و تحلیل`;
- `عملیات کسب‌وکار و بهبود فرایندها`;
- `فناوری اطلاعات / توسعه نرم‌افزار و برنامه نویسی`;
- `مدیریت استراتژیک / مشاوره مدیریت`;
- `مدیریت پروژه و برنامه`;
- `مهندسی - توسعه محصول/ تحقیق و توسعه`;
- `مهندسی - شبکه/ فناوری اطلاعات`;
- `مهندسی - کنترل کیفیت / بازرسی و نظارت`;
- `مهندسی - نصب / راه اندازی / اجرا`;
- `موفقیت مشتریان و عملیات پشتیبانی`;
- `هوش مصنوعی، یادگیری ماشین و اتوماسیون`.

This taxonomy itself validates a broader responsibility-based search universe.

### Seniority / organizational-level filters

IranTalent exposes:

- `کارآموز`;
- `کارمند / کارشناس`;
- `کارشناس ارشد / متخصص`;
- management levels.

### Education filter

Of particular methodological value, the education list includes:

- computer / IT fields;
- engineering fields;
- business / management fields;
- `سایر/تحصیلات دانشگاهی ندارد`.

This means education/access analysis can be treated as a distinct axis rather than assumed from title.

### Current visible role evidence

The September 14 root listing directly exposed same-day roles including:

- `مهندس پشتیبانی فنی ERP`;
- `کارشناس پشتیبانی عملکردی ERP در حوزه فناوری اطلاعات`;
- `مدیر سامانه برنامه‌ریزی منابع سازمانی`.

This is important current evidence that **ERP / technical support / functional support / enterprise-system responsibility is an active domestic role family**, not only a historical observation.

### Search / robots behavior

IranTalent's `robots.txt` disallows broad query-string and `/jobs-search/` crawling for general user-agents while permitting normal static pages and publishing a sitemap.

Source:

https://www.irantalent.com/robots.txt

Therefore a reliable acquisition process should prefer:

- the server-rendered root/category surface;
- direct job pages;
- indexed static pages;
- employer detail;

rather than depending on automated query-string enumeration.

### Salary / market-context layer

IranTalent's `Iran Salary` surface provides a useful **separate** market-context source.

Current 1405 examples observed:

#### Data Science / AI — expert level

- Tehran median requested net salary: approximately **50 million toman/month**;
- middle 50%: approximately **37–71 million toman**;
- the page explicitly discusses Python, SQL/data work, ML/evaluation, GenAI/LLMs, NLP/CV and deployment responsibility.

Source:

https://salary.irantalent.com/salary-report/data-science-ai-expert-salary/

#### Technical Support / Help Desk — expert level

- Tehran median requested net salary: approximately **39 million toman/month**;
- middle 50%: approximately **31–48 million toman**;
- the category explicitly includes software support and `کارشناس استقرار نرم افزار` alongside Help Desk / technical support.

Source:

https://salary.irantalent.com/salary-report/help-desk-technical-support-expert-salary/

### Salary-data caution

Salary reports answer compensation / category questions.

They do **not** establish:

- vacancy frequency;
- entry accessibility;
- demand growth for a title;
- Ali capability.

Keep compensation evidence separate from vacancy evidence.

### Current evidence quality

**High for:** taxonomy, filter structure, current root listings, salary/category context.  
**High when available for:** direct job pages.  
**Low for:** using salary-category volume as hiring-demand prevalence.

---

## 3.4 e-estekhdam — broad title/technology taxonomy + public/private market surface; freshness requires care

### Current / indexed search structure

Primary search surface:

https://www.e-estekhdam.com/search

The indexed/search-readable page exposes:

- geography;
- job title;
- technology;
- experience;
- education;
- gender;
- contract type;
- salary;
- industry;
- benefits;
- publication time;
- government / nationwide hiring alongside private hiring.

### Technology vocabulary

The platform exposes a large explicit technology vocabulary including:

- Python;
- Artificial Intelligence;
- Machine Learning;
- SQL;
- PostgreSQL;
- MySQL;
- SQLite;
- Django;
- Docker;
- Git;
- Linux;
- Power BI;
- TensorFlow;
- PyTorch;
- Kubernetes;
- many backend / frontend / infrastructure technologies.

### Job-title / responsibility vocabulary

The platform also exposes titles / families including:

- `تحلیلگر کسب و کار`;
- `کارشناس BI`;
- `تحلیلگر اطلاعات`;
- `Help Desk`;
- `پشتیبان نرم‌افزار`;
- `کارشناس تست نرم‌افزار`;
- network / security / database roles;
- ERP-related roles in category/search surfaces.

Current/indexed targeted pages exist for:

- `استخدام برنامه نویس پایتون`;
- `استخدام Help Desk`;
- `استخدام کارشناس ERP در تهران`.

Examples:

- https://www.e-estekhdam.com/search/%D8%A7%D8%B3%D8%AA%D8%AE%D8%AF%D8%A7%D9%85-%D8%A8%D8%B1%D9%86%D8%A7%D9%85%D9%87-%D9%86%D9%88%DB%8C%D8%B3-%D9%BE%D8%A7%DB%8C%D8%AA%D9%88%D9%86
- https://www.e-estekhdam.com/search/%D8%A7%D8%B3%D8%AA%D8%AE%D8%AF%D8%A7%D9%85-Help-Desk
- https://www.e-estekhdam.com/search/%D8%A7%D8%B3%D8%AA%D8%AE%D8%AF%D8%A7%D9%85-%DA%A9%D8%A7%D8%B1%D8%B4%D9%86%D8%A7%D8%B3-ERP-%D8%AF%D8%B1-%D8%AA%D9%87%D8%B1%D8%A7%D9%86

### Occupational guide surface

e-estekhdam maintains an occupational-guide surface:

https://www.e-estekhdam.com/positions

The indexed guide includes roles such as:

- database specialist;
- information-security specialist;
- systems-and-methods specialist;
- ERP specialist;
- product specialist;
- many other technical / business roles.

Example database page explicitly describes a path through junior DBA / database support toward database engineering and data engineering.

Source:

https://www.e-estekhdam.com/positions/%DA%A9%D8%A7%D8%B1%D8%B4%D9%86%D8%A7%D8%B3-%D9%BE%D8%A7%DB%8C%DA%AF%D8%A7%D9%87-%D8%AF%D8%A7%D8%AF%D9%87

### Market-report surface

The platform also publishes market reports:

https://www.e-estekhdam.com/reports

The page currently advertises a 1405 salary report plus historical labor-market reports.

### Important freshness limitation

Several indexed e-estekhdam search pages available through general web indexing were crawled months earlier.

Therefore:

- taxonomy / route existence may be current enough for search-design purposes;
- a vacancy on an older indexed page must **not** be counted as active without checking its actual posting/detail state;
- search-engine freshness must never substitute for employer/platform posting freshness.

### Recommended acquisition method

1. use the platform's title + technology taxonomy to build queries;
2. constrain publication time in native search where accessible;
3. prefer direct short-code / detail pages for vacancy evidence;
4. use occupational pages for structural responsibility interpretation only;
5. use reports for compensation / broad market context only;
6. verify active state independently when search-index age is stale.

### Current evidence quality

**High for:** taxonomy / search vocabulary / occupational architecture.  
**Medium for:** current vacancy discovery when native filters/detail pages are accessible.  
**Low for:** active-vacancy claims based only on stale indexed search pages.

---

# 4. Bilingual responsibility-search dictionary

The search dictionary should be organized by responsibility family, not merely technology.

## 4.1 Build / software

Persian:

```text
پایتون
برنامه نویس پایتون
توسعه دهنده
مهندس نرم افزار
بک اند
برنامه نویس بک اند
توسعه نرم افزار
```

English:

```text
Python
Python Developer
Software Engineer
Backend
Backend Developer
Application Engineer
Internal Tools
```

## 4.2 AI / applied AI

Persian:

```text
هوش مصنوعی
کارشناس هوش مصنوعی
مهندس هوش مصنوعی
یادگیری ماشین
پردازش زبان طبیعی
مدل زبانی
ایجنت هوش مصنوعی
هوش مصنوعی مولد
```

English:

```text
AI
Artificial Intelligence
AI Engineer
AI Specialist
Machine Learning
ML Engineer
Generative AI
LLM
NLP
AI Agent
Agentic AI
RAG
```

## 4.3 Implementation / integration / ERP

Persian:

```text
استقرار
کارشناس استقرار
پیاده سازی
راه اندازی
یکپارچه سازی
پشتیبانی نرم افزار
پشتیبانی سیستم
ERP
کارشناس ERP
پشتیبانی ERP
تحلیلگر سیستم
```

English:

```text
Implementation
Technical Implementation
Software Implementation
Integration
Integration Engineer
ERP
ERP Support
Functional Support
Technical Consultant
Systems Analyst
Application Support
```

## 4.4 Automation / process

Persian:

```text
اتوماسیون
هوشمندسازی
اتوماسیون فرایند
بهبود فرایند
سیستم ها و روش ها
تحول دیجیتال
RPA
BPMS
```

English:

```text
Automation
AI Automation
Workflow Automation
Process Automation
RPA
Business Automation
Process Improvement
Digital Transformation
```

## 4.5 Data / BI / analysis

Persian:

```text
تحلیل داده
تحلیلگر داده
مهندس داده
هوش تجاری
کارشناس BI
تحلیلگر کسب و کار
تحلیلگر اطلاعات
پایگاه داده
SQL
```

English:

```text
Data Analyst
Data Engineer
BI
Business Intelligence
Business Analyst
Database
SQL
Analytics
Reporting
```

## 4.6 Quality / evaluation / testing

Persian:

```text
تست نرم افزار
کارشناس تست
کنترل کیفیت نرم افزار
تضمین کیفیت
QA
QC
تست اتوماسیون
```

English:

```text
QA
Quality Engineer
Software Tester
Test Engineer
Test Automation
Quality Analyst
AI Evaluation
AI Quality
```

## 4.7 Support / diagnosis / operations

Persian:

```text
پشتیبانی فنی
پشتیبانی نرم افزار
پشتیبان سیستم
Help Desk
عملیات فنی
کارشناس عملیات
NOC
عیب یابی
```

English:

```text
Technical Support
Software Support
Product Support
Help Desk
Technical Operations
Operations Engineer
Application Support
NOC
Troubleshooting
```

## 4.8 Entry / transition terms

Persian:

```text
کارآموز
کارآموزی
بدون سابقه
کمتر از سه سال
کارشناس
جذب تازه کار
```

English:

```text
Junior
Entry Level
Associate
Graduate
Trainee
Intern
Internship
0-2 years
1-3 years
```

Do not require one of these labels when experience/responsibility evidence itself clearly indicates an entry/transition role.

---

# 5. Current + preserved Iranian role-family evidence

## 5.1 Direct AI roles exist, but `AI` keyword volume is noisy

Current Jobinja `هوش مصنوعی` results show a substantial volume of keyword matches and several same-day/recent engineering roles.

But the same result set includes content/design/teaching and other AI-use roles.

Conclusion:

> Use AI keyword search for discovery; never use its raw count as AI-engineering prevalence.

## 5.2 ERP / implementation / support is an active technical-responsibility family

Current IranTalent root evidence directly exposes same-day ERP technical-support and ERP functional-support roles.

IranTalent's 1405 technical-support category also explicitly includes `کارشناس استقرار نرم افزار` as part of the broader support/implementation family.

This strengthens the September 7 finding that domestic implementation/support roles deserve serious Career examination rather than being treated as nontechnical by title.

## 5.3 The Iranian market is a connected system of responsibilities

The September 7 direct Jobinja/employer pass found active/recent evidence across:

- software/backend;
- data engineering / analytics;
- QA/QC/testing;
- SRE/operations;
- systems analysis;
- infrastructure/support;
- AI engineering;
- security adjacency.

Examples preserved in the prior report include Irancell Labs, Fanavaran, Wallex, ParsPack, Najm and SnappShop.

This earlier evidence remains useful as a responsibility-shape baseline; the September 14 pass does not treat every earlier vacancy as still active.

## 5.4 Serious AI-engineering jobs can be lifecycle-heavy

The preserved Fanavaran AI Engineer example included:

- RAG / agents / prompt engineering;
- LLM evaluation;
- guardrails;
- deployment;
- latency / cost optimization;
- monitoring;
- API/microservice/database integration;
- data preprocessing.

It was also an experienced role.

Conclusion:

> Iranian `AI Engineer` can mean full application / deployment / evaluation ownership, not only model usage. The title must not be assumed to be entry level.

## 5.5 Systems analysis / process roles contain durable AI-era responsibilities

The preserved Fanavaran systems-analysis example included:

- customer requirement discovery;
- root-cause investigation;
- fix proposals;
- acceptance-test criteria;
- ERD/data-model understanding;
- troubleshooting;
- software lifecycle reasoning;
- cross-team communication.

This is exactly why `تحلیلگر سیستم`, `کارشناس سیستم‌ها و روش‌ها`, implementation and process families belong in the search universe even without `AI` in the title.

## 5.6 Technical support can range from shallow ticket handling to strong diagnostic work

The preserved ParsPack evidence included Linux, logs, DNS, mail, SSL, databases, backups, web servers, monitoring, Bash and networking.

IranTalent's current technical-support taxonomy likewise warns that software support and deployment responsibilities vary materially by organization.

Conclusion:

Support roles should be classified by **actual diagnostic/system responsibility**, not by title.

## 5.7 Junior AI routes exist but may contain academic/access gates

The September 7 Iranian sample found genuine junior AI evidence such as Najm, where limited experience was acceptable but academic/university-profile expectations were strong.

Conclusion:

Entry-level existence and personal accessibility are separate questions.

## 5.8 Data / BI / business-analysis roles strongly reinforce SQL + business translation

The prior SnappShop sample combined:

- SQL;
- Python as a plus;
- KPI/dashboard work;
- automated reporting;
- root-cause analysis;
- data quality;
- collaboration with product/data-engineering stakeholders.

IranTalent's current taxonomy separately exposes data analysis, BI/analytics and business-process groups.

Conclusion:

The Iranian market supports a hybrid data/business lane, but SQL remains a strong substrate for that family.

---

# 6. Platform-specific extraction matrix

| Platform | Current listing visibility | Filter richness | Detail evidence | Automated query reliability | Best Career use |
|---|---|---|---|---|---|
| Jobinja | High | High | Medium–High when detail retrieves | High for known query shape; detail can intermittently fail in tooling | Broad enumeration + fresh title/company metadata + targeted detail analysis |
| JobVision | Low/Medium in text crawler | Very High | High when direct detail available | Low through query-string crawling; robots disallow query params | Native filtered search + sitemap/detail discovery + vacancy-level analysis |
| IranTalent | High | Very High | High | Medium; root/static strong, query crawling restricted | Taxonomy + current listings + detail + salary/category context |
| e-estekhdam | Medium / route-dependent | Very High | Medium–High when current detail page available | Medium; indexed search pages can be stale | Broad Persian title/technology discovery + current detail verification + market reports |

---

# 7. Recommended Iranian acquisition protocol

## Phase 1 — define search frame

For each research batch specify:

- responsibility families;
- entry / transition band;
- geography;
- publication freshness target;
- source platforms;
- whether the goal is vacancy discovery, recurrence analysis, salary context or Ali-specific fit.

## Phase 2 — bilingual discovery

Run both:

```text
Persian responsibility terms
+
English responsibility terms
```

Do not rely on translation equivalence. Search both independently because employers use mixed vocabulary.

## Phase 3 — entry/access filtering

Where platforms support it, inspect:

- internship;
- less than three years;
- employee/expert level;
- work mode;
- city;
- education field;
- gender-specific constraints;
- military-service constraints;
- salary only when useful;
- publication time.

## Phase 4 — vacancy-level extraction

For every retained job record:

```text
platform
source URL
observed date
posting date / age
company
original Persian/English title
location
work mode
employment type
experience requirement
education requirement
other access gate
employer-explicit responsibilities
employer-explicit required skills
preferred skills
technical stack
business/process responsibility
testing/diagnosis responsibility
normalized responsibility families
salary if stated
active / closed / uncertain
```

## Phase 5 — source-layer separation

Label every field as one of:

```text
EMPLOYER_EXPLICIT
PLATFORM_METADATA
CAREER_NORMALIZATION
CAREER_INFERENCE
```

Never present `CAREER_INFERENCE` as employer wording.

## Phase 6 — duplicate control

Deduplicate by:

- company;
- normalized title;
- location;
- description / responsibility overlap;
- original employer link where present.

Cross-posting on two platforms counts as one employer vacancy, not two market observations.

## Phase 7 — freshness control

Suggested evidence tiers:

```text
T1 CURRENT
0–14 days

T2 RECENT
15–45 days

T3 STRUCTURAL
older / closed / uncertain current state
```

T3 can support responsibility-shape analysis but not current vacancy-volume claims.

## Phase 8 — interpretation

Aggregate by:

- responsibility family;
- recurring substrate;
- access gates;
- entry depth;
- stakeholder/business responsibility;
- degree of diagnosis/testing/ownership;

Do **not** aggregate only by technology keyword.

---

# 8. Iranian normalized responsibility families

The current evidence supports keeping at least these families in future domestic scans:

1. **Python / software / backend engineering**
2. **AI / ML / LLM application engineering**
3. **Data / BI / analytics**
4. **Implementation / ERP / integration / functional support**
5. **Software / technical / product support**
6. **QA / software testing / quality engineering**
7. **Systems analysis / business analysis / systems-and-methods**
8. **Automation / process improvement / BPMS / RPA**
9. **Operations / SRE / NOC / infrastructure support**
10. **Security / secure operations adjacency**
11. **Technical consulting / solutions / customer-facing implementation**
12. **Trainee / internship / early-career routes**

A vacancy may belong to more than one family.

---

# 9. What the four-platform evidence currently supports

### Supported

- Iranian technical hiring is broader than AI/Python titles.
- Python, data, SQL, support, testing, systems analysis, ERP/implementation and operations are all visible in the platform taxonomies and/or current/recent vacancy evidence.
- AI-labeled demand exists, but raw AI keyword counts materially overinclude non-engineering work.
- ERP/implementation/software-support is a current domestic responsibility family and deserves separate analysis.
- Persian + English bilingual search is necessary.
- Entry routes exist across several families, but experience, degree/pedigree, gender, local/on-site and other gates can dominate accessibility.
- Employer responsibility text is more valuable than title alone.
- IranTalent and e-estekhdam salary/report surfaces can add compensation/context evidence but should not be mixed with vacancy-prevalence claims.

### Not supported

- A precise Iranian market share for AI jobs from the observed search counts.
- A claim that JobVision has no jobs when crawler result cards are unavailable.
- Treating stale e-estekhdam indexed pages as current openings.
- Treating every `هوش مصنوعی` Jobinja result as engineering.
- Treating `پشتیبانی` as automatically low-skill or `استقرار` as automatically software engineering.
- Treating a title's English translation as the responsibility truth.

---

# 10. Current source register

## Jobinja

- Jobs/search surface: https://jobinja.ir/jobs
- Current `هوش مصنوعی` query: https://jobinja.ir/jobs?filters%5Bkeywords%5D%5B0%5D=%D9%87%D9%88%D8%B4+%D9%85%D8%B5%D9%86%D9%88%D8%B9%DB%8C

## JobVision

- Jobs/search surface: https://jobvision.ir/jobs
- Robots / sitemap declaration: https://jobvision.ir/robots.txt
- Sitemap: https://jobvision.ir/sitemap.xml

## IranTalent

- Jobs/search surface: https://www.irantalent.com/jobs
- Robots / sitemap declaration: https://www.irantalent.com/robots.txt
- Salary reports index: https://salary.irantalent.com/salary-reports/
- 1405 Data Science / AI expert report: https://salary.irantalent.com/salary-report/data-science-ai-expert-salary/
- 1405 Technical Support / Help Desk expert report: https://salary.irantalent.com/salary-report/help-desk-technical-support-expert-salary/
- 1405 annual salary report: https://salary.irantalent.com/annual-salary-report/iran-talent-salary-report-1405/

## e-estekhdam

- Search: https://www.e-estekhdam.com/search
- Occupational guides: https://www.e-estekhdam.com/positions
- Market reports: https://www.e-estekhdam.com/reports
- Python search route: https://www.e-estekhdam.com/search/%D8%A7%D8%B3%D8%AA%D8%AE%D8%AF%D8%A7%D9%85-%D8%A8%D8%B1%D9%86%D8%A7%D9%85%D9%87-%D9%86%D9%88%DB%8C%D8%B3-%D9%BE%D8%A7%DB%8C%D8%AA%D9%88%D9%86
- Help Desk search route: https://www.e-estekhdam.com/search/%D8%A7%D8%B3%D8%AA%D8%AE%D8%AF%D8%A7%D9%85-Help-Desk
- ERP Tehran search route: https://www.e-estekhdam.com/search/%D8%A7%D8%B3%D8%AA%D8%AE%D8%AF%D8%A7%D9%85-%DA%A9%D8%A7%D8%B1%D8%B4%D9%86%D8%A7%D8%B3-ERP-%D8%AF%D8%B1-%D8%AA%D9%87%D8%B1%D8%A7%D9%86

## Previous Career baseline

- `2026-09-07_A3_IRAN_PERSIAN_EMPLOYMENT_MARKET_EXTENSION.md`

---

# 11. Recommended next research batch

The next high-value Iranian pass should not simply collect more AI jobs.

It should build a **responsibility-diverse fresh vacancy set**, ideally across all four platforms, with deliberately separate strata such as:

```text
A. junior / low-experience software / Python
B. AI / LLM / automation
C. data / BI / SQL
D. ERP / implementation / systems integration
E. technical / software / product support
F. QA / testing / evaluation
G. systems / process / business analysis
H. operations / SRE / NOC
```

Within each stratum, prioritize T1/T2 current postings and record hard access gates.

The goal should be enough distinct employers to answer recurrence questions, not a huge raw corpus.

A reasonable next evidence package would be approximately:

- 5–10 distinct current jobs per high-priority family where the market supplies them;
- fewer when the family is genuinely sparse;
- explicit `NO SUFFICIENT CURRENT SAMPLE` rather than backfilling with stale posts.

That dataset can then be compared against Ali's current capability evidence in the E3 readiness review.

---

# 12. Final judgment

The four requested Persian platforms are usable, but only with source-specific acquisition methods.

The most reliable combined method is:

```text
Jobinja
→ direct fresh enumeration / query discovery

JobVision
→ native filters + sitemap/detail discovery; do not rely on query crawling

IranTalent
→ structured taxonomy + current visible listings + direct details + separate salary context

e-estekhdam
→ broad Persian title/technology discovery + detail verification + occupational / market-report support, with strict freshness controls
```

The Iranian market should be researched using a bilingual responsibility map rather than a narrow `AI / Python` title list.

The strongest emerging domestic opportunity space is not only "AI Engineer." It includes the connected frontier of:

```text
software / Python
+ data / SQL / BI
+ AI / automation
+ implementation / ERP / integration
+ support / diagnosis
+ QA / testing
+ systems / process analysis
+ operations
+ technical consulting / solutions
```

This source model is now strong enough to support a systematic fresh Iranian vacancy sweep and later Ali-specific E3 comparison without confusing crawler limitations, title conventions, keyword noise or stale indexing with market truth.

## 13. No-change statement

This report does **not** by itself change:

- Career working identity;
- geography priority;
- capability D-levels;
- E2 status;
- application-readiness status;
- salary target;
- UpgradePilot allocation;
- exact Career next action.

Those require the appropriate Career review and canonical owner update.