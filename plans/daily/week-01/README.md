# Deferred AegisLab Week 1 Daily Execution Index — Historical Only

> [!CAUTION]
> **This index and every linked daily file are deferred, superseded for active execution, and non-controlling. Do not open them as current instructions or execute their commands, branch actions, deliverables, or gates.**
>
> UpgradePilot is the formally selected primary 90-day flagship. [`../../../UpgradePilot.md`](../../../UpgradePilot.md) is the governing project charter. UpgradePilot implementation has not started, and no replacement UpgradePilot session or daily plan exists yet.
>
> The next authorized action is to create the **UpgradePilot capability and prerequisite specification**. The original AegisLab daily index below is preserved as historical planning evidence. Its linked files remain historical even if opened directly.

---

# Week 1 Daily Execution Index

**Historical status:** Deferred by the formal UpgradePilot selection decision; not an active daily route.  
**Preparation:** 2026-07-18 to 2026-07-19  
**Production week:** 2026-07-20 to 2026-07-26  
**Historical primary repository:** `motafegh/AegisLab`  
**Standard production requirement:** 4 focused hours Monday through Saturday  
**Historical weekly delivery:** namespace SSH closure plus Python Intake v0

## Authority

These files expanded the former AegisLab `plans/CURRENT_WEEK.md`. They are retained only as historical evidence and have no current execution authority.

Historical file order:

1. [Saturday preparation — 2026-07-18](2026-07-18.md)
2. [Sunday activation — 2026-07-19](2026-07-19.md)
3. [Monday — scenario truth and evidence acquisition](2026-07-20.md)
4. [Tuesday — fault diagnosis and namespace closure](2026-07-21.md)
5. [Wednesday — Python package and event model](2026-07-22.md)
6. [Thursday — OpenSSH log parser](2026-07-23.md)
7. [Friday — CLI and integration proof](2026-07-24.md)
8. [Saturday — owned modification and hard gate](2026-07-25.md)
9. [Sunday — evidence review and Week 2 activation](2026-07-26.md)

## Daily execution law

1. Open only the current date file and the referenced AegisLab documents.
2. Execute steps in order.
3. Do not skip a validation gate.
4. When a command produces unexpected output, stop the sequence and use the blocker protocol. Do not continue with guessed state.
5. Timeboxes are maximum budgets, not durations to fill.
6. When a deliverable finishes early and its proof passes, continue immediately to the next numbered deliverable in the same file.
7. Do not pull future-day work unless the current file explicitly authorizes it.
8. Technical evidence belongs in AegisLab. Execution summaries and hours belong in Career.
9. Never commit private keys, passwords, credentials, raw personal data, or temporary `/tmp` identity material.
10. Every technical claim must link to a command, output, test, fixture, file, or reproducible behavior.

## Required session messages

At the beginning:

```text
START DAY <program day>
Date: YYYY-MM-DD
Mode: Green | Yellow | Red
Sleep/function: <public-safe summary>
Available focused minutes:
Current deliverable:
Current AegisLab branch/commit:
```

At the end:

```text
SESSION END
Focused minutes:
Deliverables completed:
Evidence/commit:
Proof commands and results:
What Ali can explain:
AI assistance used:
Unresolved blocker:
Exact next deliverable:
```

## Branch and worktree rule

At the first technical session:

```bash
cd <local-aegislab-worktree>
git status --short
git branch --show-current
git rev-parse --short HEAD
```

- When the working tree contains unexplained changes, stop and classify them before editing.
- When the tree is clean and the current branch is `main`, create:

```bash
git switch -c week-01-namespace-python-intake
```

- When an already-active Week 1 branch exists, continue it rather than creating another branch.
- Do not mix Career planning changes into the AegisLab technical commit history.

## Week 1 final proof

The week passes only when:

```bash
python -m pytest -q
python -m ruff check src tests
python -m mypy src
python -m aegislab.cli parse tests/fixtures/sshd/success.log
python -m aegislab.cli parse tests/fixtures/sshd/unauthorized_key.log
```

and the namespace closure documents, truth records, fixtures, fault diagnosis, owned parser modification, and reduced-prompt explanation all exist and are defensible.