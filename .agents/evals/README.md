# Career Agent Skills Integration Evals

**Status:** First-generation integration evaluation scaffold; not yet activated on `main`.

## Purpose

Evaluate whether the first Career Agent Skills coexist with clear routing before adding repository-wide activation instructions or a router skill.

Current candidates:

- `career-capability-assessment`
- `career-market-calibration`
- `career-claim-audit`
- `career-review`
- `career-agent-retro`

Each skill keeps its own output and trigger evals under its skill directory. `career-skill-routing.json` tests cross-skill selection, legitimate composition, and cases where no Career skill should run.

## Integration acceptance questions

1. Does each direct operation have one clear primary skill?
2. Do mixed Career decisions use `career-review` as the orchestrator rather than causing every specialist to compete for primacy?
3. Do capability, market, and external-claim questions remain distinct when they share terms such as evidence, skill, project, or Career?
4. Does `career-agent-retro` remain explicit/maintenance-oriented rather than self-invoking after ordinary tasks?
5. Do project-local implementation/teaching and simple canonical lookups correctly select no Career skill?
6. Does the skill set work without a dedicated `career-operation-router`?

## Router admission rule

Do **not** create `career-operation-router` merely because multiple skills exist.

Admit a router only if clean-runtime integration evals show recurring missed routing, overlapping primaries, or unnecessary multi-skill loading that cannot be corrected proportionately through individual skill descriptions and `AGENTS.md` navigation.

## Evaluation status

The current repository work provides:

- static Agent Skills specification/metadata checks;
- governance-boundary desk checks;
- per-skill output eval fixtures;
- per-skill positive/negative trigger fixtures;
- this cross-skill routing matrix.

It does **not** yet provide an unbiased empirical trigger benchmark. The current design conversation already contains the skill names and intended routing, and this environment does not expose a clean isolated skill-selection runner. Run trigger and with-skill/without-skill evals in clean, fresh agent contexts before declaring the skills empirically validated.

## Activation boundary

Do not add these skills to `AGENTS.md`, merge them to `main`, or treat them as controlling Career procedures until integration review is complete and the user authorizes activation.
