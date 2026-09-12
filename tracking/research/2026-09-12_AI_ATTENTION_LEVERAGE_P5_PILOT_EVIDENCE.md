# AI Attention Leverage — P5 Pilot Evidence

**Date opened:** 2026-09-12  
**Owner:** Ali Rajabi / Career  
**Status:** ACTIVE supporting evidence — reconcile into the main report at P5 closure  
**Parent report:** `2026-09-12_AI_ATTENTION_LEVERAGE_AND_LOW_ENERGY_PRODUCTIVITY_REPORT.md`  
**Purpose:** Preserve real P5 pilot evidence without creating a second live Career-state owner.

---

## PILOT-1 — On-demand Current-State Re-entry Pack

### Real trigger/input

Use the current UpgradePilot state after the CI static↔runtime correlation slice reached E-phase orientation.

Evidence consulted:

- UpgradePilot `MEMORY.md`;
- active `working-memory/2026-09-12_ci-static-runtime-correlation-bridge.md`;
- `src/upgradepilot/ci/workflow_runtime_correlation.py`;
- `tests/test_workflow_runtime_correlation.py`.

### Ali setup burden

`LOW`

The trigger can be expressed as simply as:

> Re-orient me to current UpgradePilot work from the canonical current owners; keep it compact and do not take over project planning.

### AI work performed

Recovered current responsibility, current implementation/proof, one representative source/test flow, stronger-claim exclusions, current E questions, and deferred scope.

### Compact re-entry packet produced

**Current responsibility**

UpgradePilot is no longer building the first CI static↔runtime bridge. A/B/C/D are complete. The current responsibility is **E — decide which remaining evidence gap actually matters next before authorizing another implementation slice**.

**What materially changed**

- added deterministic static↔runtime workflow/job/step correlation for a deliberately bounded ordinary named-workflow class;
- introduced the stronger dependency-CI state `supported_runtime_correlated`;
- preserved `supported_not_correlated` as a conservative fallback when static consumption + successful CI exist but safe step correlation cannot be established;
- full deterministic suite is green at **549 tests**;
- maintainer-action synthesis remains abstention-only; no targeted-check/merge/investigate/block/defer permission was added.

**One current engineering flow**

```text
exact static workflow definition
+
exact workflow run / exact-attempt jobs / runtime step summaries
↓
workflow_runtime_correlation
↓
static job/step identity ↔ runtime job/step identity
↓
dependency-CI interpretation
↓
supported_runtime_correlated OR conservative weaker/unresolved state
```

The correlation layer establishes **identity/relationship**, not dependency installation, exact version, wheel selection, compatibility, proposal safety, or maintainer action.

**Representative safety boundary**

Positive correlation currently requires literal unique names, exact static/runtime job-name-set agreement, ordered unique runtime step numbers, one runtime match per static step, and preserved step order. Matrix/strategy, reusable workflows, dynamic/missing names, ambiguity, or mismatched sets stay unresolved rather than guessed.

**Proof / non-proof**

Proven:

- bounded static job↔runtime job correlation;
- bounded static user-step↔runtime-step correlation;
- stronger runtime-correlated dependency-CI classification;
- focused/nearest/full deterministic regressions green.

Not proven:

- exact installed dependency version;
- selected/downloaded wheel;
- wheel compatibility;
- behavioral compatibility;
- complete CI coverage;
- proposal safety;
- any non-abstention maintainer action.

**What not to broaden into now**

Do not automatically add:

- matrix/reusable/dynamic-name support;
- job-log parsing;
- exact wheel/version semantics;
- targeted-check permission;
- other maintainer actions;
- CLI/report redesign.

E must first identify which missing proposition is actually decision-relevant.

**Four ownership/retrieval questions**

1. Why is `supported_runtime_correlated` stronger than `supported_not_correlated`, and what still remains unproven?
2. Why can a matrix workflow make the *correlation layer* unresolved without forcing the whole dependency-CI result to lose already-earned static/support evidence?
3. Why are display names acceptable matching anchors only together with the surrounding uniqueness/set/order constraints?
4. Before requesting job logs or broader workflow support, what exact missing proposition would those new data/capabilities need to establish?

### Ali review/use burden

Expected `LOW` for orientation; actual user-use benefit still needs Ali's real use/feedback in a later UpgradePilot return.

### Material errors/noise observed

None found during generation. The packet remained consistent with the canonical current state and representative source/test evidence.

### Attention/re-entry benefit

`PROVISIONALLY HIGH`

The packet compresses several large owners/source/test surfaces into one current responsibility and preserves exact links back to canonical truth without storing another live-state copy.

### Ownership effect

`NEUTRAL-TO-STRENGTHENING`

It does not answer E for Ali. It prepares the current model and questions Ali must still reason through.

### Disposition

`CONTINUE / LIKELY ADOPT SHAPE`

Important correction:

> If the last meaningful touchpoint cannot be established confidently, do **not** invent a "what changed since last time" delta. Fall back to a **current-state-only re-entry pack** and say the delta horizon is unknown.

---

## PILOT-4 — Bounded Background Research Scout, second real trial

### Exact question

What evidence supports a compact delegation/return-package contract for unattended or review-later AI work, and what should it *not* claim?

### Evidence inspected

Current official guidance and research, including:

- GitHub Copilot coding-agent best practices;
- GitHub Copilot agent review guidance;
- OpenAI's 2026 Codex safety/operating-boundary guidance;
- Schmalbach (2026), *Software Delegation Contracts: Measuring Reviewability in AI Coding-Agent Work*.

### Findings

1. **Well-scoped task definitions matter.** GitHub explicitly recommends a clear problem, complete acceptance criteria, and enough repository/change scope to make the task reviewable.
2. **Research/plan before mutation is often useful.** Current cloud-agent guidance supports repository research and planning before opening a PR or committing to a change.
3. **Agent output still needs normal review.** GitHub states agent PRs/reviews can be wrong and should receive ordinary human review.
4. **Explicit delegation contracts mainly improve reviewability, not necessarily correctness.** The 2026 controlled pilot found evidence sufficiency/reviewer clarity improved under explicit return-package requirements while objective task correctness did not materially improve; this came with additional token/wall-clock cost.
5. **Risk/authority boundaries should be explicit.** OpenAI's Codex deployment guidance emphasizes bounded access, explicit higher-risk approvals, and auditability/telemetry.

### Practical implication for this program

A repeatable `REVIEW_LATER` delegation contract should normally recover only:

```text
TASK / QUESTION
→ exact responsibility and desired output

INPUT / AUTHORITY BOUNDARY
→ what sources/context the AI may rely on

ACCEPTANCE / STOP CONDITION
→ what would make the returned work useful and where to stop

RETURN PACKAGE
→ findings/output
→ evidence/source anchors
→ material limitations/unknowns
→ changed files/actions when applicable
→ what Ali/owner must review or decide
```

Do **not** require this ceremony for tiny obvious background-safe transformations. Its value is highest when reviewability is otherwise the bottleneck.

### Ali setup burden

`LOW`

### Ali review/use burden

`LOW-MEDIUM`

The result is compact enough to guide workflow design without requiring Ali to read the full source set.

### Material errors/noise

No material contradiction found across the selected sources. The research study is treated as supporting evidence rather than universal proof.

### Attention benefit

`HIGH`

The scout converts a multi-source search into one bounded design conclusion while leaving the adoption decision open.

### Ownership effect

`STRENGTHENING`

The output clarifies what Ali still owns: acceptance, review, and consequential decision.

### Disposition

`PROVISIONAL ADOPT`

Likely future persistence: reusable cross-workflow delegation/return-package procedure, but only after the remaining pilots show the same contract generalizes beyond research.

---

## PILOT-5 — Independent Challenge Pass on the AI-leverage program

### Real artifact challenged

- `plans/2026-09-12_AI_ATTENTION_LEVERAGE_AND_LOW_ENERGY_PRODUCTIVITY_ADOPTION_PLAN.md`;
- `tracking/research/2026-09-12_AI_ATTENTION_LEVERAGE_AND_LOW_ENERGY_PRODUCTIVITY_REPORT.md` through P4.

### Challenge boundary

Return at most three material findings. Prefer `NO MATERIAL FINDING` over speculative critique.

### Finding 1 — Re-entry delta must fail closed when the prior touchpoint is uncertain

**Severity:** Medium  
**Confidence:** High

A "delta since Ali last worked here" is only trustworthy when the last meaningful touchpoint can be recovered from conversation/project evidence. Otherwise the AI can create a plausible but false change narrative.

**Smallest repair direction:** make current-state orientation the default invariant; include a delta only when its baseline is explicit/recoverable.

### Finding 2 — Derived learning formats can recreate artifact/maintenance bloat

**Severity:** Medium  
**Confidence:** High

The proposed learning bundle can easily become:

```text
canonical learning artifact
+ fast-relearn file
+ Notebook source pack
+ audio
+ video
+ flashcards
+ quiz
+ term map
```

That would violate the same proportionality principles this program is trying to enforce.

**Smallest repair direction:** preserve one grounded canonical learning artifact where project-local governance justifies it; generate derivative formats **on demand** and do not persist them all by default.

### Finding 3 — Durable Career governance/Skills must be tool-agnostic

**Severity:** Medium  
**Confidence:** High

The research report necessarily discusses current products such as ChatGPT Work, Codex, GitHub Copilot and Gemini Notebook. These product capabilities change quickly.

**Smallest repair direction:** if a durable Skill/governance rule is later adopted, define stable capability classes such as:

```text
research agent
repository/coding agent
scheduled/conditional automation
source-grounded learning transformer
```

and keep named-product selection in replaceable tool guidance or current workflow examples, not the durable Career contract.

### No-change conclusions from the challenge pass

No material defect found in:

- the four attention classes;
- the prohibition on capability inference from AI output;
- the rule that rest remains valid;
- the rejection of token-utilization quotas;
- the Career↔project authority boundary;
- the requirement to test workflows before creating Skills/governance.

### Ali setup burden

`VERY LOW`

### Ali review/use burden

`LOW`

Three findings are bounded and directly actionable.

### Attention/quality benefit

`MEDIUM-HIGH`

The challenge pass found three issues worth carrying into P6/P7 without opening a second broad audit.

### Ownership effect

`STRENGTHENING`

The pass supplies pressure/counterevidence; Ali/Career still decides adoption.

### Disposition

`PROVISIONAL ADOPT WITH STRICT OUTPUT CAP`

A future challenge procedure should default to at most three material findings and explicitly support `NO MATERIAL FINDING`.

---

## P5 state after first execution batch

| Pilot | Current evidence |
|---|---|
| PILOT-1 Re-entry pack | generated successfully from live UpgradePilot truth; actual Ali-use benefit still needs later confirmation |
| PILOT-2 Learning bundle v2 | waiting for a natural project-local learning-artifact trigger |
| PILOT-3 Low-energy audio + retrieval | waiting for grounded source material + a genuine low-energy use period |
| PILOT-4 Research scout | two positive real trials; provisional adopt |
| PILOT-5 Independent challenge | one positive real trial with three useful findings; provisional adopt with output cap |

Do not call P5 complete yet. PILOT-2/PILOT-3 require natural real use, and PILOT-1 still benefits from Ali's actual re-entry experience before final persistence decisions.
