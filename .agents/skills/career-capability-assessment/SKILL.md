---
name: career-capability-assessment
description: >
  Assess whether evidence justifies a Career capability-depth, ownership, or demonstrated-skill conclusion for Ali on one bounded responsibility. Use when reassessing D-levels; deciding whether project, learning, source, test, modification, debugging, changed-case, delayed, or reduced-prompt evidence establishes capability; or deciding whether a responsibility or technology may be treated as demonstrated. Separate repository behavior, Ali's demonstrated actions, AI assistance, recency, confidence, and transfer limits. Do not use for ordinary project implementation, teaching, market research, or generic repository review.
compatibility: Designed for the motafegh/Career repository and agents that can read the repository authorities and the exact evidence being assessed.
---

# Career Capability Assessment

## Purpose

Perform a Career-level assessment of what Ali has actually demonstrated for one bounded professional or technical responsibility.

This skill defines the assessment procedure. It does **not** define Career capability levels, current capability state, or project truth. Those remain owned by the Career repository and the relevant project evidence.

The goal is calibrated judgment: resist unsupported promotion without suppressing legitimate ownership growth.

## Load only the authority and evidence you need

1. Follow `AGENTS.md` and the repository authority order.
2. Read `tracking/CAPABILITY_EVIDENCE_LEDGER.md` for the canonical depth model, assistance labels, evidence expectations, current record for the responsibility when one exists, and record format.
3. Read `CAREER_STATE.md` only when the assessment could change the live Career position, application readiness, current capability emphasis, or another state-owned conclusion.
4. Inspect the smallest sufficient underlying evidence. For project-derived evidence, use the relevant project repository's canonical source, tests, commits, outputs, working evidence, or registered Career handoff as needed; do not treat a Career summary as a substitute when the underlying evidence is material to the decision.
5. Do not load the whole Career or project repository by default. Expand context only when the current evidence cannot be interpreted safely without it.

If the evidence needed to decide is unavailable, record the proposition as unresolved or unassessed at the required scope. Absence of evidence is not evidence of inability.

## Assessment workflow

### 1. Define the responsibility precisely

Express the assessment target as a concrete responsibility with a practical boundary, not a broad technology label.

Prefer forms such as:

- modify and test one bounded Python parsing responsibility;
- diagnose one class of HTTP/environment failures;
- design and query a bounded relational-data model;
- review a pull request using a defined evidence set.

If the request asks for a broad conclusion such as "Python capability" or "ML ownership," decompose it into the material responsibilities actually evidenced. Do not average mixed responsibilities into one optimistic score.

### 2. Identify the decision being requested

Determine whether the task is to:

- establish a first assessment;
- reassess an existing record;
- decide whether new evidence changes the current depth;
- decide whether a capability/ownership claim is supportable;
- identify what remains unestablished.

Read the existing Career record when one exists before deciding what changed.

### 3. Separate the evidence streams

Keep these distinct:

- **Repository or product evidence:** what the system demonstrably does.
- **Ali evidence:** what Ali personally explained, predicted, selected, modified, tested, diagnosed, verified, reproduced, or challenged.
- **AI/human assistance:** what substantive explanation, implementation, test generation, diagnosis, decision structure, or correction was supplied.
- **Timing and conditions:** when the evidence occurred and whether it was immediate, delayed, changed-case, failure-based, repeated, or reduced-prompt.

Do not convert repository sophistication into Ali capability.

### 4. Judge evidence quality for the proposed depth

Use the canonical ledger requirements. Consider only dimensions that are meaningful for the responsibility and proposed depth, including where relevant:

- directness of Ali's performance;
- changed-case or variant evidence;
- ownership-bearing modification or test work;
- relevant failure diagnosis or repair;
- delayed reconstruction or recall;
- reduced-prompt performance;
- repeated or materially varied cases;
- recency and freshness;
- breadth of transfer.

These are evidence dimensions, **not a point system**. Never calculate a D-level mechanically from checked boxes.

### 5. Compare new evidence with the existing record

New evidence does not automatically replace prior evidence.

- Preserve stronger valid prior evidence when a new case is weaker.
- Let staleness reduce current confidence or narrow a present-tense claim when justified; do not erase historical evidence merely because it is old.
- A failure can strengthen diagnostic evidence or reveal a precise gap.
- A successful case can still be weak capability evidence when it was highly guided or merely repeated a supplied pattern.

### 6. Select the strongest defensible conclusion

Choose the highest depth that the canonical model and verified evidence actually support for the bounded responsibility.

Do not deliberately under-score merely because AI assistance existed. AI assistance changes the evidence interpretation and claim boundary; it does not by itself prove that no capability was demonstrated.

Do not promote beyond the evidence. In particular, do not infer ownership from exposure, project completion, repository size, successful commands, passing AI-generated tests, immediate repetition, reading-and-agreeing, or AI-generated implementation.

### 7. State confidence and transfer limits

Every material conclusion should make clear:

- how confident Career can be in the assessment;
- how current the evidence is;
- what neighboring responsibilities or unfamiliar contexts remain unproven;
- which stronger claim would overreach.

One bounded success is not unrestricted transfer.

### 8. Define the next evidence that could change the conclusion

When evidence is insufficient, state the **evidence class or acceptance condition** Career would need to reassess, not a project-local lesson or implementation sequence.

Good:

> Reassess after a materially changed case with limited prompting plus a relevant failure diagnosis.

Bad:

> Open `parser.py`, change function X, write test Y, then run command Z.

Career specifies what must become true and how it will know. The project/session owns how to produce legitimate evidence.

### 9. Update Career records only when authorized

Do not edit the capability ledger merely because project evidence exists.

A ledger change requires a Career review or explicit capability assessment that reaches a supported conclusion. If no material conclusion changed, preserve the existing record.

## Invalid shortcuts

Never use these shortcuts:

- project progress = Ali capability;
- documentation or explanation volume = ownership;
- test count or green CI = testing capability;
- AI-generated implementation = Ali implementation ownership;
- immediate correct repetition = independent transfer;
- one guided case = broad capability;
- AI assistance = automatically no capability;
- no observed evidence = proven inability;
- stale evidence = evidence never existed;
- technology exposure = technology mastery.

## Output

Keep ordinary conversational assessments proportional to the question.

For a formal or record-changing assessment, use the repository's canonical record format and include, when material:

- Responsibility
- Prior Career conclusion, if any
- New conclusion / depth
- Best evidence
- Assistance
- Last demonstrated / recency
- Confidence
- Transfer limit
- Claim permitted
- Claim prohibited
- Next reassessment or trigger

If evidence is insufficient to distinguish between two levels safely, say what is established, what remains unresolved, and what additional evidence would discriminate them. Do not invent precision.

## Final checks

Before finalizing, verify that:

- the assessment target is a bounded responsibility rather than a technology name;
- the canonical Career depth/evidence model was consulted;
- repository behavior, Ali evidence, and assistance were separated;
- the conclusion is the strongest supported one, neither inflated nor artificially suppressed;
- recency, confidence, and transfer limits are explicit where material;
- missing evidence was not converted into inability;
- no project-local learning or implementation plan was created;
- no live Career record was changed without a supported Career-level assessment;
- public Career records remain public-safe.
