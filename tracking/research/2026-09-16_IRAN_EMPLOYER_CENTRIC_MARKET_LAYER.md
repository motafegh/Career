# Iran Market — Employer-Centric Intelligence Layer

**Date:** 2026-09-16  
**Status:** Current employer-level extension to the Iran-only E3 market lane; evidence artifact, not capability or live-state owner  
**Owner:** Career market-calibration evidence  
**Primary source in this pass:** Jobinja company pages + Jobinja Top-50 employer surface  
**Companions:** `2026-09-16_IRAN_MARKET_CURRENT_VACANCY_REFRESH.md`, `2026-09-16_IRAN_NATIVE_DETAIL_RESOLUTION_UPDATE.md`

## 1. Why this layer exists

The vacancy-led Iranian search is necessary but insufficient.

A title/keyword sweep can miss employers that:

- repeatedly hire the same relevant responsibility family under changing titles;
- maintain genuine internship / trainee / junior entry routes;
- hire support, implementation, QA, systems-analysis, data, AI and software roles side by side;
- have no ideal vacancy today but frequently open one;
- expose stronger evidence about hiring activity and résumé handling through their company pages than through one isolated advertisement.

The employer-centric question is therefore:

> Which Iranian employers show repeated, current, inspectable hiring behavior around Career-relevant technical responsibility families, and how should Career use that evidence without confusing company popularity with Ali-specific job fit?

This is **not** a universal ranking of Iranian employers and is **not** a claim about workplace quality.

---

## 2. Jobinja Top-50 — what the platform signal actually means

Jobinja maintains a `50 top companies` surface:

https://jobinja.ir/top50

Jobinja explicitly says the list is constructed from indicators observed over the **previous 90 days**.

The surface exposes, for each employer:

- an overall Jobinja score;
- `محبوبیت میان کارجویان` — popularity among jobseekers;
- `تعدد و تنوع فرصت‌های شغلی` — abundance/diversity of opportunities;
- `بررسی رزومه‌های دریافتی` — résumé-review activity;
- the current number of active vacancies shown by Jobinja.

These are useful platform signals, but they do **not** establish:

- that a company is objectively a better employer;
- that its engineering culture is strong;
- that it mentors juniors;
- that one of its current roles fits Ali;
- that a high active-job count means high technical hiring;
- that a high résumé-review score guarantees a response to Ali.

### Career rule

Use Jobinja Top-50 as an **employer-discovery and hiring-activity signal**, then inspect the company's actual current and historical job mix.

Do not use Top-50 rank as the application decision.

---

## 3. Employer-intelligence model

For Iranian Career decisions, inspect an employer across these dimensions:

| Dimension | Question |
|---|---|
| Platform activity | Is the company currently and repeatedly hiring? |
| Relevant-role density | How much of the hiring surface is actually technical/relevant rather than unrelated volume? |
| Responsibility-family recurrence | Do support / implementation / QA / Python / data / AI / systems roles recur over time? |
| Entry accessibility | Does the employer visibly use internship, trainee, junior, low-experience, or growth-under-mentorship routes? |
| Native responsibility quality | Do the descriptions expose real technical work rather than vague titles? |
| Access gates | Are degree, military service, experience, city, gender, prior-product/domain or other gates restrictive? |
| Employer responsiveness signal | Does Jobinja show relatively strong résumé-review activity? Use only as a weak platform-specific signal. |
| Technical/product context | Is there enough product/software/system responsibility to make the role valuable for the current Career direction? |
| Current Ali-fit opportunity | Is there a vacancy today whose responsibility and evidence boundary is defensible? |
| Watch value | Even without a fit today, is this employer worth revisiting because relevant roles recur? |

### Evidence hierarchy

```text
current native vacancy description
→ current company job page
→ recurring expired vacancy history
→ Top-50 / platform indicator
→ company self-description / culture language
```

A native job description overrides lightweight metadata or company marketing.

Expired jobs are **recurrence evidence only**. They are not current opportunities.

---

# 4. Current Jobinja technology-employer sample

The current Top-50 contains many technology employers. The following sample was inspected because their domain and/or live vacancy mix intersects with Career's current role bands.

Numbers below are the Jobinja surface observed in this research pass and may change continuously.

## 4.1 Didar CRM — high watch value for implementation / customer-technical responsibility

**Jobinja Top-50:** #23, overall 8.4  
**Observed indicators:** popularity 10 / opportunity diversity 6 / résumé review 9  
**Observed active vacancies:** 18

Current company-page roles include:

- `Technical Customer Success Specialist`;
- `Customer Success Analyst`;
- `کارشناس استقرار نرم‌افزار`;
- Data Analyst;
- Machine Learning Engineer;
- other customer/product roles.

Historical company-page evidence additionally shows repeated:

- software implementation + support;
- QA;
- software training;
- technical/customer-success responsibilities.

### Important native-detail correction

The current `Technical Customer Success Specialist` role is **not automatically junior-friendly**. Its detailed responsibility text asks for serious software-development depth, APIs/webhooks/authentication/integration, debugging/log/database reasoning and Python/Node/SQL-style technical work, despite permissive-looking metadata.

This is a strong example of the rule:

> **native responsibility depth beats title and metadata.**

### Career use

- **Employer watch:** HIGH.
- **Current software-implementation vacancy:** worth native-detail resolution.
- **Technical Customer Success vacancy:** benchmark / likely too deep unless the current native requirements fit unexpectedly.
- **Why monitor:** implementation/support/customer-technical families visibly recur.

Source: https://jobinja.ir/companies/didar-crm/jobs

---

## 4.2 Asiatech — high family signal, but current ERP support is experience-gated

**Jobinja Top-50:** #11, overall 8.7  
**Observed indicators:** popularity 10 / opportunity diversity 7 / résumé review 10  
**Observed active vacancies:** 23

Current technical mix includes:

- IT / network quality control;
- DevOps;
- systems and methods;
- management systems;
- `کارشناس پشتیبانی نرم افزار (ERP)`;
- `کارشناس استقرار نرم‌افزار (ERP)`;
- SOC;
- PHP.

This is excellent evidence that one employer can expose multiple Career-relevant responsibility families simultaneously.

### Current ERP Support native JD

The current ERP-support description explicitly requires:

- **3–6 years experience**;
- daily enterprise-software user support;
- reported-error analysis;
- initial testing of changes/fixes;
- ticket registration and follow-through;
- user education/documentation;
- SLA responsibility;
- Rahkaran familiarity;
- SQL Server;
- BPMN;
- bachelor's degree;
- military-service completion/permanent exemption.

### Career use

- **Employer watch:** HIGH for market intelligence.
- **Current ERP Support:** responsibility shape is excellent, but experience/access requirements make it a benchmark rather than an immediate first-batch application from current Career evidence.
- **Current ERP Deployment:** resolve separately only if its native gates are materially lighter.
- **Why monitor:** ERP/support/quality/systems families are live and broad.

Source: https://jobinja.ir/companies/asiatech/jobs

---

## 4.3 Parmis IT — strong QA / support / implementation watch employer

**Jobinja Top-50:** #25, overall 8.4  
**Observed indicators:** popularity 10 / opportunity diversity 6 / résumé review 9  
**Observed active vacancies:** 12

Current/recent company-page roles include:

- Help Desk;
- `کارشناس تست نرم‌افزار مالی`;
- C#/.NET test automation;
- full-stack development;
- `کارشناس پشتیبانی و استقرار نرم‌افزار`;
- financial/management-software implementation.

This employer is particularly useful because the product domain naturally creates:

```text
software product
+ customer/business process
+ testing
+ deployment/implementation
+ support
```

### Career use

- **Employer watch:** HIGH.
- **Current financial-software test role:** high-value native-JD resolution candidate for the conditional QA lane.
- **Support/implementation roles:** recurrent; monitor for lighter experience gates.
- **Current Help Desk:** separate network/IT support from application/product support; do not merge them simply because both say support.

Source: https://jobinja.ir/companies/parmis-it/jobs

---

## 4.4 Mahak Software Group — strong current software-support recurrence

**Jobinja Top-50:** #29, overall 8.3  
**Observed indicators:** popularity 8 / opportunity diversity 7 / résumé review 10  
**Observed active vacancies:** 17

Current roles include:

- `کارشناس پشتیبان نرم‌افزار` — Tehran, posted about 2 days before the observed page;
- `کارشناس پشتیبانی فنی نرم‌افزار` — Mashhad, about 5 days;
- another software-support role in Mashhad;
- after-sales internship;
- PHP development;
- AI team lead.

The company describes its core business as producing and supporting financial and management software. Historical listings show repeated software-support/customer/software roles.

### Career use

- **Employer watch:** HIGH.
- **Tehran software-support vacancy:** promote into native-detail resolution because it is current and directly inside Career's technical-product/software-support band.
- **Mashhad technical-support vacancy:** relevant if geography is feasible; native duties still required.
- **After-sales internship:** do not assume technical value until duties are inspected.

Source: https://jobinja.ir/companies/mahak-software-group/jobs

---

## 4.5 Fanavaran — strong technical employer signal + explicit internship lane

**Jobinja Top-50:** #9, overall 8.9  
**Observed indicators:** popularity 9 / opportunity diversity 8 / résumé review 10  
**Observed active vacancies:** 15

Current technical roles include:

- SRE;
- SRE Operations Engineer;
- AI Engineer;
- SysAdmin;
- `کارآموز برنامه نویسی C#`;
- React;
- software systems analyst;
- other software roles.

The current C# internship is important even though C# is not Career's anchor language. It demonstrates that this employer has a **real technical entry lane** rather than only senior/specialist hiring.

### Career use

- **Employer watch:** HIGH.
- **Current C# internship:** not an automatic application; do not chase a new stack merely because the employer has an entry opening.
- **Market signal:** strong evidence that structured technical entry exists inside a mature software organization.
- **Future relevance:** high if Python/data/QA/analysis/implementation entry roles appear.

Source: https://jobinja.ir/companies/fanavaran-5/jobs

---

## 4.6 System Group / Hamkaran System — recurring implementation/ERP watch employer

**Jobinja Top-50:** #42, overall about 8.1 in the observed Top-50 surface.

Current inspected roles skew toward deeper AI/software responsibilities such as ML/NLP and other specialist work.

Historical/current-market evidence outside a single current page repeatedly exposes:

- ERP implementation;
- support;
- web-service/application support;
- enterprise-system responsibility.

The current Iran vacancy sequence already contains a Fara Samaneh / Hamkaran-System-associated `کارشناس استقرار و پشتیبانی نرم افزار ERP` candidate.

### Career use

- **Employer/ecosystem watch:** HIGH for the implementation/ERP responsibility family.
- **Current direct Jobinja fit:** not established from this pass.
- **Why monitor:** enterprise-software implementation/support is one of the strongest Iran-specific role families discovered for Ali's business/process + technical transition shape.

---

## 4.7 Mobinhost — adjacent infrastructure/support watch

**Jobinja Top-50:** #34, overall about 8.3.

Current/recent roles include:

- datacenter installation;
- hosting support;
- senior system administration;
- other hosting/infrastructure work.

Historical evidence also shows recurring hosting/technical-support and internship-like activity.

### Career use

- **Employer watch:** MEDIUM-HIGH as an adjacent systems/technical-support route.
- **Current fit:** requires role-specific inspection because hosting support can quickly become Linux/network/operations-depth heavy.
- **Do not infer:** generic technical support fit from the title alone.

---

## 4.8 ParsPack — infrastructure/support benchmark and watch

**Jobinja Top-50:** #36, overall about 8.2.

Current observed openings skew away from Ali's first application band, while historical pages include Linux-hosting support and related infrastructure responsibilities.

### Career use

- **Employer watch:** MEDIUM for support/operations opportunities.
- **Capability benchmark:** useful for Linux/network/diagnosis responsibility.
- **Not current first target** unless a lower-experience support/operations role appears.

---

## 4.9 Mohaymen — strong engineering/security market signal

**Jobinja Top-50:** #30, overall about 8.3.

Current roles observed include:

- SRE;
- Data Analyst;
- SOC Tier-1/Tier-2.

### Career use

- **Market/capability benchmark:** HIGH.
- **Immediate application watch:** CONDITIONAL.
- This employer is valuable for tracking what Iranian security/platform/data employers demand, but current roles can require operational depth beyond Career's strongest evidence.

---

## 4.10 Digikala — large-product/data benchmark

**Jobinja Top-50:** #21, overall 8.4  
**Observed active vacancies:** 30.

Current evidence includes a data-analyst responsibility; historical evidence spans data, backend, QA, operations and other mature-product responsibilities.

### Career use

- **Market benchmark:** HIGH.
- **Application watch:** role-specific rather than company-wide.
- Data-heavy opportunities remain gated where SQL/relational expectations exceed current evidence.

---

## 4.11 Bime Bazar — high platform activity does not equal high current fit

**Jobinja Top-50:** #1, overall 9.7  
**Observed indicators:** popularity 10 / opportunity diversity 10 / résumé review 9  
**Observed active vacancies:** 52.

This is the clearest demonstration that company-level volume must be normalized by **relevant-role density**.

The employer has substantial hiring activity, but the current technical roles inspected are largely more experienced backend/data/IT responsibilities rather than obvious entry-transition roles for Ali.

### Career use

- **Market signal:** HIGH.
- **Immediate Ali-fit signal:** LOW/role-specific from the current sample.
- Do not prioritize solely because the company is #1 or has 52 openings.

---

## 4.12 Snapp ecosystem — high hiring volume, current fit must remain vacancy-specific

Top-50 contains multiple Snapp-family employers including:

- Snappfood;
- Snapp Pay;
- Snapp Group;
- Snappbox;
- Snapp Market.

These companies show large-scale Iranian digital-product hiring and are useful market benchmarks.

However, the inspected current pages do not justify assuming a current junior technical fit merely from employer scale or brand.

### Career use

- **Market signal / mature-product benchmark:** HIGH.
- **Watch:** yes, especially for support/QA/data/implementation/junior software openings.
- **Application decision:** vacancy-specific only.

---

## 4.13 PART AI — specialist AI benchmark

**Jobinja Top-50:** #44, overall around 8.0.

As a specialized AI organization, PART is useful for observing current Iranian AI responsibility depth and terminology.

### Career use

- **AI-market benchmark:** HIGH.
- **Immediate application priority:** only if a genuinely junior/trainee/implementation/evaluation responsibility appears whose native depth fits.
- Do not turn specialist AI employer visibility into pressure to claim ML/AI ownership that Career has not established.

---

## 4.14 AbrNOC / Payam Pardaz — cloud/security signals

The observed Top-50 also includes employers such as:

- AbrNOC — cloud / infrastructure context;
- Payam Pardaz — security/software context.

These are useful for the long-term adjacent cloud/security direction.

### Career use

- **market/capability benchmark:** useful;
- **current application watch:** role-specific;
- do not deepen these domains solely because the companies are visible in Top-50.

---

# 5. Employer classes for Career use

These classes describe **how Career should use current evidence**. They are not employer-quality rankings.

## Class A — application-watch employers

Revisit frequently because they expose current or recurring roles close to Ali's approved calibration bands:

- **Didar CRM** — implementation / technical-customer / data/product responsibilities;
- **Asiatech** — ERP support/deployment, quality, systems; current roles may be experience-gated;
- **Parmis IT** — QA/testing, support, deployment/implementation;
- **Mahak Software Group** — software support / technical support + entry-adjacent activity;
- **Fanavaran** — broad engineering stack + explicit technical internship lane;
- **System Group / Hamkaran ecosystem** — enterprise-software implementation/support;
- **Mobinhost** — technical support / hosting / systems adjacency.

A company remains Class A even when today's exact vacancy is not suitable, because relevant role families recur.

## Class B — mature engineering / capability benchmarks

Use to understand what deeper Iranian technical responsibility looks like and to detect future junior openings:

- Digikala;
- Bime Bazar;
- Snapp ecosystem;
- Mohaymen;
- ParsPack;
- Dotin and similar mature financial/software employers when their current roles are inspected.

## Class C — specialist market-signal employers

Use mainly to monitor domain-specific responsibility evolution:

- PART AI — AI;
- AbrNOC — cloud/infrastructure;
- Payam Pardaz — security;
- other high-specialization employers discovered in subsequent company sweeps.

Do not infer application fit from the class itself.

---

# 6. Changes to the active Iran candidate-resolution queue

The employer-centric pass adds **new candidates for native-detail resolution**; it does not displace Viuna/Avisa without stronger vacancy evidence.

### Preserve the current first two

1. **Viuna — Technical Software Support** — remains highest-information current candidate.
2. **Avisa — Python/Django Internship** — remains strongest explicit Python entry route.

### Add to the next resolution group

- **Mahak — `کارشناس پشتیبان نرم‌افزار` (Tehran, very fresh)** — new high-value company-page candidate; resolve JD/access.
- **Mahak — `کارشناس پشتیبانی فنی نرم‌افزار` (Mashhad)** — inspect if geography is feasible.
- **Parmis — `کارشناس تست نرم‌افزار مالی`** — strong conditional QA candidate; recover native requirements.
- **Didar — `کارشناس استقرار نرم‌افزار`** — strong family/current listing; recover native JD before fit decision.

### Keep as employer/family benchmarks unless lighter gates emerge

- Asiatech ERP Support — current JD requires 3–6 years + bachelor's + military-service completion/exemption + Rahkaran/SQL/BPMN familiarity;
- Didar Technical Customer Success — title is attractive but detailed technical depth is much stronger than a normal junior support role;
- Fanavaran C# internship — validates entry lane, but do not change Career stack simply to chase one internship;
- infrastructure/cloud/security specialist roles — role-specific only.

---

# 7. New Iran acquisition architecture

From this point, Iran market work should use **two simultaneous discovery lanes**.

## Lane 1 — vacancy-first

Continue the existing four-platform process:

```text
Jobinja + JobVision + IranTalent + e-estekhdam
→ Persian + English responsibility terms
→ current/open verification
→ native duties
→ access
→ fit
→ application decision
```

## Lane 2 — employer-watch

Maintain a small employer set and periodically inspect:

1. current company-page vacancies;
2. newly opened relevant roles;
3. current role-family mix;
4. internship/junior routes;
5. expired history only for recurrence;
6. changes in active-job count / Jobinja Top-50 signals as secondary context;
7. employer-native career pages where stronger than Jobinja.

### Promotion rule

A company-watch finding becomes an active candidate only when a **specific current vacancy** survives the ordinary current/open + native-duty + access + evidence-fit sequence.

No company gets an automatic application because it is popular or in Top-50.

---

# 8. What this adds to Career decision quality

The employer-centric layer improves decisions in five ways.

### 8.1 It prevents title-search blind spots

A software company may repeatedly hire implementation/support/QA work without the exact keywords used in the broad sweep.

### 8.2 It distinguishes opportunity volume from relevant opportunity

Fifty active vacancies can be less useful than five recurring implementation/support roles.

### 8.3 It reveals recurring responsibility families

Repeated implementation/support/QA roles across months are stronger market-shape evidence than one isolated vacancy.

### 8.4 It surfaces real entry behavior

An employer that actually posts internships or junior roles gives stronger entry-access evidence than generic culture claims about learning.

### 8.5 It creates a better watch strategy

Career no longer has to rediscover every employer from scratch on every search pass.

---

# 9. Limits

- Jobinja Top-50 is a platform-specific ranking, not a neutral survey of all Iranian companies.
- Company self-descriptions are employer marketing and receive low evidentiary weight.
- Current active-job counts change frequently.
- Some Jobinja detail pages are intermittently inaccessible through automated tooling.
- Expired roles establish recurrence only.
- The current employer sample intentionally emphasizes technology employers and therefore does not estimate the prevalence of these responsibilities in the whole Iranian labor market.
- JobVision, IranTalent and e-estekhdam do not expose an identical Top-50 company mechanism; employer-centric analysis on those platforms should use company/category/native-career surfaces rather than forcing a false equivalent metric.
- This market evidence changes no Ali capability D-level.

---

# 10. Current Career implication

The current Iran-only strategy becomes:

```text
VACANCY-FIRST CURRENT SEARCH
+
EMPLOYER-WATCH SEARCH
+
NATIVE JD / ACCESS VERIFICATION
+
ALI EVIDENCE BOUNDARY
→ bounded application decisions
```

The new company layer supports the existing role-band decision rather than changing it.

The most important newly reinforced Iranian responsibility families remain:

- technical software/product support;
- implementation / deployment / ERP;
- QA/testing;
- structured junior/intern software entry;
- later, role-specific data/AI/security/cloud routes when current depth/access fit.

The next employer-driven native-detail checks should prioritize **Mahak software support, Parmis financial-software testing and Didar software implementation** alongside the already-active Viuna/Avisa/Carbon sequence.

Do not broaden into indiscriminate company applications. Use the watchlist to discover better vacancies earlier.
