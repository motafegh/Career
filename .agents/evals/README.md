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
- `career-personal-work-planning`

Each skill keeps its own output and trigger evals under its skill directory. `career-skill-routing.json` tests cross-skill selection, legitimate composition, and cases where no Career skill should run.

## Integration acceptance questions

1. Does each direct operation have one clear primary skill?
2. Do mixed Career decisions use `career-review` as the orchestrator rather than causing every specialist to compete for primacy?
3. Do capability, market, external-claim, and personal-planning questions remain distinct when they share terms such as evidence, skill, project, Career, next, or plan?
4. Does `career-personal-work-planning` translate current Career/project truth into Ali-facing outcomes without becoming project-local technical planning?
5. Does `career-agent-retro` remain explicit/maintenance-oriented rather than self-invoking after ordinary tasks?
6. Do project-local implementation/teaching and simple canonical lookups correctly select no Career skill?
7. Does the skill set work without a dedicated `career-operation-router`?

## Static routing result

The combined review found and corrected material overlaps rather than hiding them behind a router:

1. `career-capability-assessment` and `career-claim-audit` initially overlapped on broad "demonstrated skill" wording.
2. specialist market/capability/claim procedures needed a clearer boundary when their evidence feeds a final material Career decision.
3. personal planning needed an explicit boundary from both `career-review` and project-local Planning/Design.

The integration branch now encodes these rules:

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

Ali-facing next session/day/week/month plan from current Career + project truth
→ career-personal-work-planning
   + preserve project-owned technical continuation
   + stop/conditionalize at unresolved Career/project gates

completed-agent execution retrospective
→ career-agent-retro

project implementation / project teaching / project technical planning / simple canonical lookup / plain job discovery
→ no Career skill
```

`career-review` links to sibling capability, market, and claim skills and loads them lazily only when their domain is material. `career-personal-work-planning` consumes current Career decisions and project continuation; it does not silently make a formal Career decision or redefine project execution.

### Static specification checks

The current six skill names and frontmatter use fields permitted by the published Agent Skills reference validator. Descriptions and compatibility text remain within the validator limits by static inspection, directory names match skill names, and each skill body remains below the Agent Skills recommendation of 500 lines.

The official `skills-ref` CLI was **not** executed in this environment because the local runtime could not reach external package/repository hosts. The validation claim above is therefore a source-backed static check against the published specification/reference validator, not a CLI execution result.

## Router admission rule

Do **not** create `career-operation-router` merely because multiple skills exist.

Admit a router only if clean-runtime integration evals show recurring missed routing, overlapping primaries, or unnecessary multi-skill loading that cannot be corrected proportionately through individual skill descriptions and `AGENTS.md` navigation.

**Current static conclusion:** a router is **not justified yet**. Known routing ambiguities were resolved proportionately through specialist descriptions, review composition, and the explicit personal-planning/project-planning boundary. Keep the router deferred until empirical evidence says otherwise.

## Evaluation status

The current repository work provides:

- static Agent Skills specification/metadata checks;
- governance-boundary desk checks;
- per-skill output eval fixtures;
- per-skill positive/negative trigger fixtures;
- a 28-case cross-skill routing matrix including no-skill cases;
- static cross-skill routing review and boundary refinement.

It does **not** yet provide an unbiased empirical trigger benchmark or with-skill/without-skill comparison. The current design conversation already contains the skill names and intended routing, and this environment does not expose a clean isolated skill-selection runner. Run trigger and output evals in clean, fresh skill-capable agent contexts before declaring the skills empirically validated.

## Activation boundary

Do not add these skills to `AGENTS.md`, merge them to `main`, or treat them as controlling Career procedures until empirical integration evaluation is complete enough for an activation decision and Ali authorizes activation.
