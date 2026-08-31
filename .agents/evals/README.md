# Career Agent Skills Integration Evals

**Status:** First-generation integration evaluation scaffold; static routing review passed after boundary refinements; not yet activated on `main`.

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

## Static routing result

The first combined review found one material overlap and one orchestration ambiguity:

1. `career-capability-assessment` and `career-claim-audit` both initially described "demonstrated skill" questions broadly enough that an external CV claim could plausibly make both compete for primacy.
2. specialist market/capability/claim procedures needed a clearer boundary when their evidence feeds a final material Career decision.

The integration branch now encodes these rules directly in the skill descriptions and evals:

```text
direct capability-depth / ownership question
→ career-capability-assessment

market sample / vacancy evidence-strength question
→ career-market-calibration

CV / portfolio / application / interview / external wording claim
→ career-claim-audit

final material Career state / strategy / readiness / project-role decision
→ career-review as primary
   + load only the specialist procedures actually needed

completed-agent execution retrospective
→ career-agent-retro

project implementation / project teaching / simple canonical lookup / plain job discovery
→ no Career skill
```

`career-review` now links to its sibling capability, market, and claim skills and loads them lazily only when their domain is material.

### Static specification checks

The current five skill names and frontmatter use fields permitted by the published Agent Skills reference validator. Each description remains below the 1,024-character validator limit, compatibility text remains below 500 characters, directory names match skill names, and each skill body remains below the Agent Skills recommendation of 500 lines.

The official `skills-ref` CLI was **not** executed in this environment because the local runtime could not reach external package/repository hosts. The validation claim above is therefore a source-backed static check against the published specification/reference validator, not a CLI execution result.

## Router admission rule

Do **not** create `career-operation-router` merely because multiple skills exist.

Admit a router only if clean-runtime integration evals show recurring missed routing, overlapping primaries, or unnecessary multi-skill loading that cannot be corrected proportionately through individual skill descriptions and `AGENTS.md` navigation.

**Current static conclusion:** a router is **not justified yet**. The known routing ambiguity was resolved proportionately through specialist descriptions and lazy review composition. Keep the router deferred until empirical evidence says otherwise.

## Evaluation status

The current repository work provides:

- static Agent Skills specification/metadata checks;
- governance-boundary desk checks;
- per-skill output eval fixtures;
- per-skill positive/negative trigger fixtures;
- a 20-case cross-skill routing matrix including no-skill cases;
- static cross-skill routing review and boundary refinement.

It does **not** yet provide an unbiased empirical trigger benchmark or with-skill/without-skill comparison. The current design conversation already contains the skill names and intended routing, and this environment does not expose a clean isolated skill-selection runner. Run trigger and output evals in clean, fresh skill-capable agent contexts before declaring the skills empirically validated.

## Activation boundary

Do not add these skills to `AGENTS.md`, merge them to `main`, or treat them as controlling Career procedures until empirical integration evaluation is complete enough for an activation decision and the user authorizes activation.
