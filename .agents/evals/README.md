# Career Agent Skills Integration Evals

**Status:** Active first-generation Career Agent Skills support/evaluation material on `main`.

## Active skills

- `career-capability-assessment`
- `career-market-calibration`
- `career-claim-audit`
- `career-review`
- `career-agent-retro`
- `career-personal-work-planning`

Each skill keeps its own output and trigger eval fixtures under its skill directory. `career-skill-routing.json` preserves the current **29-case** cross-skill routing expectations, including valid no-skill outcomes.

## Routing summary

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

substantive audit of canonical Career governance / strategy / planning / portfolio / capability / market content
→ no Career skill by default
   + inspect the relevant canonical owners directly
   + use a specific specialist only when a real sub-question requires it

project implementation / project teaching / project technical planning / simple canonical lookup / plain job discovery
→ no Career skill
```

## Validation status

The current material includes static Agent Skills metadata/specification checks, governance-boundary review, per-skill output fixtures, positive/negative trigger fixtures, and the **29-case** cross-skill routing matrix.

The routing matrix now explicitly distinguishes a substantive canonical-content governance audit from a completed-agent execution retrospective, preventing `career-agent-retro` from being selected merely because the word “governance audit” appears.

A clean blind empirical benchmark was intentionally **not made an activation gate** after Ali explicitly chose to activate and merge the current skill set on 2026-09-01. Do not describe the skills as empirically benchmarked unless such testing is actually performed later.

## Router decision

Do not add `career-operation-router` merely because multiple skills exist. The current routing ambiguities are handled through skill descriptions, review composition, explicit no-skill cases, and the personal-planning/project-planning boundary. Reconsider a router only if real usage shows repeated routing failures that cannot be fixed proportionately in the existing surfaces.
