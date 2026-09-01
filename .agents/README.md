# Career Agent Skills

Career uses six active repository Agent Skills under `.agents/skills/`. They are procedural aids and do not override `AGENTS.md` or the canonical Career truth owners.

| Skill | Primary responsibility |
|---|---|
| `career-capability-assessment` | Assess what Ali has actually demonstrated or owns at a bounded capability depth. |
| `career-market-calibration` | Interpret vacancy/sample evidence and what the market evidence can legitimately establish. |
| `career-claim-audit` | Audit CV, portfolio, application, interview, and other external claims against evidence. |
| `career-review` | Run material Career decisions such as readiness, strategy, allocation, workload, or project-role changes; compose specialist skills only when needed. |
| `career-agent-retro` | Reconstruct and improve completed agent execution, routing, context use, and governance friction. |
| `career-personal-work-planning` | Plan Ali's next session/day/week/month from Career priorities plus authoritative project continuation without taking over project-local technical planning. |

## Normal operation

Use the skill whose responsibility matches the **requested output**, not merely a keyword in the request.

- Read `AGENTS.md` first and preserve its authority order and Career/project boundary.
- Load skills on demand; do not read all six at the start of every task.
- When one skill clearly matches, read its `SKILL.md` before performing that procedure.
- Use one primary skill where possible. Load a sibling only when a material sub-question genuinely requires it.
- `career-review` is primary for final material Career decisions and may lazily compose capability, market, or claim procedures.
- `career-personal-work-planning` may read authoritative project continuation for context, but project repositories continue to own technical plans and execution.
- `career-agent-retro` is explicit retrospective/maintenance work, not an automatic post-task ceremony.
- If no skill matches, operate directly from the controlling Career authority rather than forcing a skill.

Project implementation, project teaching, project technical planning, simple canonical lookups, and plain vacancy discovery are valid **no Career skill** cases.

Skills guide procedure only. They do not own live state, capability truth, market truth, review decisions, project state, or other canonical records. A conflict between a skill and higher Career authority is resolved in favor of the higher authority and should be treated as a defect in the skill/governance layer.

Evaluation/support material lives under `.agents/evals/` and each skill's `evals/` directory. These are testing artifacts and are not normal operational context. The current routing matrix contains 28 cross-skill/no-skill cases.
