# Career Agent Skills Empirical Evaluation Protocol

**Status:** Candidate-system empirical test protocol; not activation evidence by itself.

## Goal

Evaluate the six candidate Career Agent Skills in clean, fresh skill-capable sessions without exposing the expected routing/output labels to the worker agent.

Candidates:

- `career-capability-assessment`
- `career-market-calibration`
- `career-claim-audit`
- `career-review`
- `career-agent-retro`
- `career-personal-work-planning`

## Blindness rule

The worker agent must not read:

- any `evals/evals.json` file;
- any `evals/eval_queries.json` file;
- `.agents/evals/career-skill-routing.json`;
- prior empirical results;
- this protocol's grading section before completing the run.

The controller/grader may read those files after the worker response is recorded.

Use a fresh conversation/session for each independent run where practical. Do not prime the worker with skill names, expected labels, or earlier answers.

## A. Trigger evaluation

For each skill:

1. Controller selects one query from that skill's `evals/eval_queries.json` without showing `should_trigger`.
2. Start a fresh skill-capable session with the Career branch checked out and normal repository skill discovery enabled.
3. Send only the query.
4. Record:
   - whether the candidate skill was automatically loaded/materially applied;
   - any competing Career skills loaded;
   - whether the response respected project/Career boundaries;
   - token/time data if the runtime exposes it.
5. Repeat each query 3 times when practical.

Suggested default acceptance:

- positive query trigger rate > 0.5;
- negative query trigger rate < 0.5;
- no recurring competing-primary collision.

Do not optimize descriptions from one anomalous run. Refine only when repeated misses/collisions show a pattern.

## B. Cross-skill routing evaluation

Use `.agents/evals/career-skill-routing.json` as the hidden answer key.

For each case:

1. Send only the `query` to a fresh worker session.
2. Record the primary Career skill actually used, any secondary skills, or no Career skill.
3. Grade after the response against:
   - `primary_skill`;
   - `allowed_secondary_skills`;
   - `must_not_use`.
4. Treat `primary_skill: null` as a real expected outcome; do not reward loading a Career skill merely because one exists.

A failure is material when the wrong primary changes authority, scope, evidence standard, or action boundary—not merely because an optional secondary procedure was omitted.

## C. Output-quality evaluation

For each skill's `evals/evals.json` case:

### With-skill run

1. Start a clean session with the candidate skills available.
2. Send only the `prompt`.
3. Save the complete response and observed skill provenance/activation if available.

### Baseline run

1. Start a separate clean session from the same Career repository state with the target candidate skill unavailable/disabled if the client supports it.
2. Send the same `prompt`.
3. Save the response.

If the client cannot selectively disable one skill, use the closest honest baseline available and record the limitation. Do not claim a controlled with/without comparison when one was not actually run.

### Grade after both outputs exist

Compare against the hidden `expected_output` and inspect concrete assertions such as:

- correct authority/source owner used;
- Career/project boundary preserved;
- no unsupported capability/market/claim/state inference;
- required stop/gate behavior present;
- no invented implementation steps or evidence;
- concise enough to be useful;
- no unnecessary sibling-skill loading.

Add/refine assertions only after observing real outputs; do not overfit the rubric before seeing failures.

## D. Personal-work-planning specific checks

For `career-personal-work-planning`, verify especially:

- technical project continuation is read through from the project's canonical live owner rather than recreated by Career;
- session/day plans stay outcome-focused and compact;
- reduced capacity causes scope reduction, not schedule compression;
- unresolved Career/project gates conditionalize farther planning;
- missing capability evidence is not manufactured through fake failures or artificial project work;
- direct state lookup, formal Career review, project planning/design, and project teaching remain non-triggers.

## E. Result record

For each run record at least:

```text
case_id
run_number
fresh_session: yes/no
query_or_prompt
skills_loaded
primary_skill_observed
secondary_skills_observed
response_saved
trigger_or_routing_verdict
output_quality_verdict
material_failure_reason
runtime/token notes if available
```

Keep raw worker outputs outside the worker's future context until grading is complete.

## F. Decision rule after empirical runs

After enough clean runs:

```text
repeated clean pass
→ keep description/procedure unchanged

repeated trigger miss or collision
→ refine the smallest relevant skill description/boundary

correct routing but weak output
→ refine procedure/eval assertions, not trigger description by default

recurring no-skill/skill ambiguity across several candidates
→ reconsider whether a router is justified

single anomalous failure
→ record; do not add governance/process automatically
```

Do not activate on `main` until empirical evidence is sufficient, material failures are resolved or explicitly accepted, and Ali authorizes activation.
