---
name: career-agent-retro
description: >
  Reconstruct and audit how an AI assistant actually operated during a completed Career task or session. Use only when Ali explicitly asks for a retrospective, execution trace, governance/skill-use audit, context/tool-efficiency review, or analysis of what the agent really read, used, missed, or found ambiguous. Distinguish observed execution from inference, material guidance from incidental context, and agent error from governance, skill, stale-source, tool, or unavoidable-uncertainty causes. Recommend the smallest durable repair and the correct destination. Do not self-invoke after ordinary work, and do not modify repository files unless the current instruction separately authorizes changes.
compatibility: Designed for the motafegh/Career repository and agents with access to the relevant conversation/tool trace, session logs, or other execution evidence for the task being reviewed.
---

# Career Agent Retrospective

## Purpose

Analyze what an AI assistant **actually did** during a completed Career task and identify the smallest improvements that would make future agent work more accurate, discoverable, efficient, and governable.

This is not an idealized description of how the task should have been performed. It is an evidence-based execution retrospective.

Use this skill only on explicit request or during an explicitly authorized governance/skill-system audit. Default to analysis-only.

## Evidence sources

Use the strongest available execution evidence, such as:

- current conversation/tool history;
- agent session transcript or logs;
- repository reads/writes visible in tool traces;
- Git diff/commit history created during the reviewed task;
- skill invocation logs where the runtime exposes them;
- user corrections or steering during the task.

Do not reconstruct an exact trace from memory when logs are available.

If the runtime does not expose some information, label it as inferred or unknown rather than presenting it as observed fact.

Do not copy raw private transcripts, secrets, credentials, private paths, or sensitive user context into the public Career repository.

## Retrospective workflow

### 1. Fix the reviewed scope

Identify:

- the exact task/session being reviewed;
- whether the user wants only analysis or also authorized repairs;
- which repository and agent runtime were involved;
- the completion point of the task.

Do not silently include unrelated sessions.

### 2. Reconstruct the actual execution trace

Record, as evidence permits:

- instruction/governance/context files actually opened or read;
- approximate order of first use;
- skills/procedures actually selected or missed;
- external sources consulted;
- important tools/actions used;
- files actually modified;
- validations/checks actually run;
- user corrections that changed the path.

Separate **opened/read** from merely discovered, mentioned, or known to exist.

### 3. Label confidence and provenance

For each material trace statement, distinguish:

- **Observed** — directly supported by transcript/tool/log evidence;
- **Strongly inferred** — not directly logged but supported by clear execution evidence;
- **Uncertain/unknown** — evidence is insufficient.

Do not convert an expected workflow into an observed workflow.

### 4. Identify which guidance materially affected behavior

For each instruction/governance/skill source actually used, ask whether it changed:

- operation classification;
- authority/truth owner;
- scope boundary;
- evidence standard;
- file location;
- tool choice;
- validation method;
- write/no-write decision;
- stopping point;
- Career-to-project boundary.

Do not list every file as material merely because it was read.

### 5. Identify deliberate non-loading and unnecessary loading

Where evidence permits, note:

- relevant files deliberately not loaded because the task did not require them;
- files loaded speculatively but never used;
- oversized tool results whose contents did not affect the task;
- repeated reads caused by weak navigation or stale pointers.

A smaller context footprint is desirable only when correctness is preserved.

### 6. Classify friction before proposing a fix

Useful friction categories include:

- **Navigation/discovery** — the agent struggled to find the right owner or context.
- **Operation routing** — the agent misclassified the task or chose the wrong procedure/skill.
- **Authority ambiguity** — multiple files appeared to own the same truth or precedence was unclear.
- **Stale/duplicate truth** — mutable state was repeated and diverged.
- **Skill trigger/scope** — a skill failed to trigger, triggered too broadly, or overlapped another skill.
- **Missing procedure** — a recurring operation lacked a reliable skill/process.
- **Context bloat** — excessive material was loaded relative to the decision.
- **Tool economy** — unnecessary searches, reads, retries, or expensive operations occurred.
- **Missing automated check** — a deterministic check could have caught a repeatable mechanical error.
- **Privacy/safety boundary** — sensitive/public-safe handling was unclear or violated.
- **Tool/platform limitation** — the environment prevented the preferred workflow.
- **Unavoidable uncertainty** — no reasonable instruction or tool change would remove the ambiguity.

### 7. Diagnose the root cause

Do not assume every agent mistake proves the governance is defective.

Classify each important finding as primarily:

- agent execution error;
- governance/instruction ambiguity;
- weak navigation/pointer design;
- skill design or trigger defect;
- stale/duplicated source content;
- missing deterministic validation;
- tool/runtime limitation;
- user scope change or interruption;
- unavoidable uncertainty.

A finding may have secondary causes, but identify the primary one before proposing changes.

### 8. Choose the correct repair destination

Possible outcomes include:

- **No change** — existing guidance was clear; the agent simply failed to follow it once.
- **Canonical source repair** — the underlying truth is stale, duplicated, or unclear.
- **AGENTS/navigation refinement** — the right source exists but is hard to discover or route to.
- **Skill refinement** — a repeatable procedure or trigger is weak.
- **New skill proposal** — a recurring, high-value operation lacks reusable procedure.
- **Automated check/script** — a deterministic mechanical failure can be caught cheaply.
- **Tooling change** — tool output/access makes correct operation unnecessarily difficult.
- **Process/eval change** — representative tests are missing for agent behavior.

Do not add more text to `AGENTS.md` merely because an agent made a mistake. Prefer the smallest destination that addresses the root cause.

### 9. Prioritize by impact, recurrence, and confidence

Prioritize findings that are:

- likely to recur;
- materially harmful when they recur;
- supported by clear evidence;
- fixable with a proportionate change.

Do not turn one unusual session artifact into a large governance redesign.

### 10. Keep analysis separate from repair

Default retrospective behavior is analysis-only.

If Ali asks for the retrospective only, do not edit files, create branches, or implement fixes.

If Ali explicitly authorizes repairs in the same instruction, first identify the findings and repair targets, then make only the authorized changes under normal Career governance.

## High-value retrospective questions

When relevant, answer questions such as:

- Which repository files did the agent actually read, and in what approximate order?
- Which instructions materially changed a decision?
- How was the operation type/skill selected?
- What relevant context was intentionally not loaded?
- Where did routing, duplication, ambiguity, or stale state cause friction?
- Did the agent read too much or too little?
- Did tool choice or output size waste effort?
- Was there a deterministic mistake that should become a check?
- Did the user have to correct a recurring agent behavior?
- Does the finding justify a new/refined skill, or would that be overfitting?

## Invalid shortcuts

Never use these shortcuts:

- ideal workflow = actual workflow;
- file mentioned = file read;
- one agent mistake = governance defect;
- more instructions = better governance;
- more files loaded = safer reasoning;
- repeated context = stronger authority;
- tool failure = agent reasoning failure;
- user correction = proof the original instructions were missing;
- every lesson = repository change.

## Output

Keep the retrospective concise enough to act on.

A useful structure is:

### Actual trace

| Order | Source/action | Evidence confidence | Material effect |
|---|---|---|---|

### Findings

| Finding | Category | Primary root cause | Impact/recurrence | Recommended destination |
|---|---|---|---|---|

### Missed or unnecessary context

State only meaningful omissions or excess reads.

### Recommended changes

List the smallest prioritized changes. Include **no change** where that is the correct conclusion.

If the user asks for confidence separation, label statements explicitly as observed, strongly inferred, or uncertain.

## Final checks

Before finalizing, verify that:

- the reviewed task/session boundary is explicit;
- actual execution is separated from ideal procedure;
- claims about reads/tools/skills are grounded in available trace evidence;
- material versus incidental guidance is distinguished;
- root cause is diagnosed before repair destination;
- agent error is not automatically converted into more governance;
- context/tool efficiency is considered without sacrificing correctness;
- no repository changes were made unless explicitly authorized;
- no sensitive transcript material is copied into public Career records.
