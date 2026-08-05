# 2026-08-18 Technical Capability Checkpoint

**Owner:** Ali Rajabi  
**Status:** Active Career assessment contract for the 2026-08-18 Day-30 review  
**Assessment date:** 2026-08-18  
**Career authority:** [`../CAREER_STATE.md`](../CAREER_STATE.md), [`CURRENT_CAREER_CYCLE.md`](CURRENT_CAREER_CYCLE.md)  
**Execution aid:** [`CURRENT_WEEK.md`](CURRENT_WEEK.md)  
**Technical truth owner:** `motafegh/UpgradePilot` source, tests, `MEMORY.md`, active plans, ADRs, and project-local evidence  
**UpgradePilot technical anchor used to define this checkpoint:** 2026-08-05 B2 / Step 7F state, including the live upstream-repository generality gap recorded at commit `d0d4e90642b2479d8a41eafe241fa0a5872b4be3`

## 1. Purpose

This file defines what Ali should be able to **understand, explain, read, reason about, test, modify, and diagnose by 2026-08-18** based on the actual UpgradePilot system and the current Career objective.

It exists for two uses:

1. **Now through 2026-08-17:** a concrete checkpoint for project-local learning and ownership work.
2. **On 2026-08-18:** the technical capability rubric used by Career during the Day-30 reassessment.

This is **not** an UpgradePilot implementation plan and must not control project sequencing. UpgradePilot owns how gaps are taught, practised, implemented, tested, and repaired. Career owns only the capability target, evidence standard, and later assessment.

The goal is not to master the entire repository. The goal is to convert the most employment-relevant current UpgradePilot responsibilities from scattered guided familiarity into one coherent, defensible technical model with bounded ownership evidence.

## 2. Target state on 2026-08-18

By the checkpoint, Career should be able to say approximately:

> Ali understands the current UpgradePilot B2 investigation system coherently, can read and reason about its central Python patterns, understands its evidence and trust architecture, can interpret representative tests, and has begun demonstrating bounded technical ownership rather than only immediate guided familiarity.

Expected depth is intentionally uneven:

- **Overall UpgradePilot architecture:** solid D2, with bounded signs approaching D3.
- **Evidence/trust reasoning:** strong D2.
- **Central Python source reading:** D2.
- **Python modification:** at least one genuine bounded D2→D3 candidate.
- **Testing:** D2 on representative project tests plus at least one ownership-bearing case.
- **Debugging:** D2 with real diagnostic evidence.
- **HTTP/API acquisition:** D2 conceptual/operational.
- **LLM integration/trust boundary:** D2 conceptual; independent implementation ownership not required.
- **PEP 440 / target-Python reasoning:** D1→D2 bounded understanding.
- **Git/GitHub ordinary operation:** working D2; advanced collaboration is not required.

No broad D3 or D4 claim is implied by meeting this checkpoint.

## 3. Depth labels used in this checkpoint

### Level A — Must own by the checkpoint

Ali should be able to:

- explain the responsibility without relying immediately on AI prose;
- identify approximately where it lives in the source tree;
- trace its major input → processing → output path;
- explain why the responsibility exists and what it does not prove;
- predict behavior for a representative changed case;
- read the central Python constructs involved;
- reason about the relevant tests;
- participate meaningfully in a bounded modification, test, or diagnosis with reduced prompting.

### Level B — Must understand operationally

Ali should be able to:

- explain purpose, inputs, outputs, boundaries, and major failure modes;
- recognize the implementation and use it safely;
- read the code with project-local AI assistance;
- understand why the chosen method exists.

Independent reproduction is not required.

### Level C — Exposure is sufficient for now

Ali should know what the concept/tool is and why UpgradePilot uses it. Deep internals, independent implementation, or broad transfer are deliberately deferred.

## 4. Frozen core versus moving frontier

UpgradePilot is moving rapidly. Career must therefore avoid an impossible target where every new commit becomes a new mastery requirement.

### Frozen core — must be coherent by 2026-08-18

The checkpoint covers the B2 investigation architecture established through the current Step-7 responsibility:

```text
public repository + PR number
→ validated PR identity
→ exact base/head identity + changed files
→ dependency-change analysis
→ DependencyVersionChange OR explicit problem

DependencyVersionChange
├── independent CI dependency-exercise branch
└── upstream branch
    → exact PyPI release
    → trusted upstream repository
    → complete release index
    → crossed-release selection
    → exact proposed-version tag/commit
    → exact changelog discovery/acquisition
    → authoritative crossed-release interval
    → deterministic source window
    → bounded local semantic candidate extraction
    → deterministic reconstruction/validation
    → grounded support-drop claim?
        ├── no  → target Python remains inactive / explicit unresolved state
        └── yes → exact-head pyproject.toml
                  → TargetPythonDeclaration
                  → target-Python relevance
```

For every major arrow Ali should be able to answer:

```text
What is the input?
What is the output?
Why is this step necessary?
What authority or trust does it establish?
What happens when it cannot establish that evidence?
What does the result NOT prove?
```

### Moving frontier — operational understanding is enough initially

For substantial responsibilities implemented only in the final 2–3 days before the checkpoint, Career initially requires only:

```text
What problem does it solve?
Where does it fit in the current system?
What does it consume?
What does it produce?
What are its stop/failure boundaries?
What does it not prove?
```

Those recent responsibilities may become later ownership targets without making the August-18 checkpoint move continuously.

## 5. Level-A system responsibilities

### 5.1 UpgradePilot product mission and bounded claim doctrine

Ali must be able to explain that UpgradePilot is evidence-backed dependency-update decision support, not an autonomous maintainer replacement.

Ali should distinguish:

```text
observation / acquired evidence
→ validation and identity
→ bounded interpretation
→ explicit uncertainty
→ bounded conclusion or suggestion
```

from unsupported guessing, compatibility claims, safety claims, or merge decisions.

Ali should understand why missing or conflicting evidence is preserved as an explicit state instead of being filled by inference.

### 5.2 Dependency-change evidence

Primary source areas:

```text
src/upgradepilot/dependency/analysis.py
src/upgradepilot/dependency/change.py
src/upgradepilot/dependency/requirements.py
src/upgradepilot/dependency/uv_lock.py
src/upgradepilot/dependency/versioning.py
```

Ali must understand the distinction among:

```text
source-file evidence
→ source-specific extracted version change
→ PR-wide trusted DependencyVersionChange
OR
→ DependencyChangeProblem
```

Required reasoning includes:

- why a changed dependency file is not automatically a trusted dependency change;
- why several changed packages cannot silently become one arbitrary package;
- why conflicting old→new transitions must stop rather than be reconciled by guess;
- why package-name normalization matters;
- why base/head revision and blob/source identity matter;
- why an expected unsupported or conflicting state is often a domain result rather than a program crash.

Ali does not need to memorize every `uv.lock` parsing branch.

### 5.3 Explicit evidence states and typed problem results

Ali must understand why UpgradePilot commonly represents states such as:

```text
available
unresolved
unsupported_source
source_unavailable
identity_mismatch
ambiguous_source
no_successful_ci
```

rather than collapsing domain truth to `True`/`False`.

Ali should be able to explain the practical meaning of result unions such as:

```python
DependencyVersionChange | DependencyChangeProblem
UpstreamRepositoryEvidence | UpstreamRepositoryProblem
TargetPythonDeclaration | TargetPythonDeclarationProblem
```

Expected inability to establish evidence should normally remain inspectable product information. Exceptions remain appropriate for programming errors, invalid internal contracts, or acquisition classes explicitly modeled as exceptional.

### 5.4 CI dependency-exercise reasoning

Primary source areas:

```text
src/upgradepilot/ci/dependency_exercise.py
src/upgradepilot/ci/workflow_commands.py
src/upgradepilot/github/actions.py
```

Ali must understand the current narrow question:

> Did at least one successful exact-head CI path consume the admitted dependency representation and exercise the changed package under the current deterministic rule?

Ali must distinguish:

```text
CI exists
CI succeeded
successful exact-head CI exists
workflow definition at exact head is available
admitted install path is actually consumed
the changed package is exercised
```

Current result classes should be understood conceptually:

```text
proven
no_successful_ci
unresolved
```

Ali must be able to explain why CI exercise does **not** establish complete coverage, compatibility, safety, or merge readiness.

Ali must also understand that the CI branch is currently independent from the upstream semantic branch: one branch does not erase or automatically gate the evidence of the other merely because they answer related questions.

### 5.5 Release intervals and crossed releases

Ali must understand why a change such as:

```text
2.6 → 2.8.4
```

requires reasoning across the full crossed interval rather than inspecting only `2.8.4`.

Required understanding:

- old version;
- proposed version;
- old-exclusive / proposed-inclusive crossed-release reasoning;
- release ordering;
- intermediate releases;
- why a support-boundary change can appear before the final proposed release;
- why exact version/source identity must remain attached to the evidence.

Deep packaging mathematics is not required.

### 5.6 Changelog discovery and deterministic source windows

Primary source areas:

```text
src/upgradepilot/github/changelog.py
src/upgradepilot/upstream/changelog.py
```

Ali must understand Step 7A conceptually:

```text
exact commit
→ bounded repository-tree inspection
→ admitted changelog basenames
→ exactly one candidate or explicit unresolved result
→ reacquire selected file at the same immutable commit
```

Ali must understand Step 7B conceptually:

```text
exact tagged changelog
+ trusted crossed-release interval
→ complete matching Markdown release sections
→ exact deterministic source window
```

Required terms/mechanisms:

- Markdown ATX headings (`#` through `######`);
- exact release-section selection;
- source ordering;
- original line IDs;
- original character offsets;
- complete section preservation;
- duplicate/missing/out-of-order section failure;
- bounded source-window size;
- unresolved on overflow rather than silent truncation;
- structural selection versus semantic interpretation.

### 5.7 Deterministic versus semantic responsibility

Ali must be able to classify the architecture into deterministic and semantic work.

Examples of deterministic work:

```text
identity validation
version interval selection
exact source acquisition
Markdown section selection
line/offset reconstruction
schema validation
candidate grounding
PEP-440-based target comparison
```

The bounded semantic task is approximately:

```text
Does this exact admitted release text explicitly state a current Python support drop?
```

Ali should understand why a probabilistic semantic model can be useful for this narrow interpretation without being granted authority over the surrounding evidence system.

### 5.8 LLM candidate extraction and trust boundary

Primary source areas:

```text
src/upgradepilot/upstream/support_drop_extractor.py
src/upgradepilot/upstream/support_drop.py
src/upgradepilot/upstream/claim.py
```

Ali must understand:

```text
trusted bounded source window
→ local LLM candidate extraction
→ UNTRUSTED candidate result
→ deterministic source reconstruction
→ deterministic claim validation
→ grounded claim / no relevant claim / unresolved
```

The model may select bounded candidate semantics such as:

```text
python_line
introduced_in_version
source_line_id
```

The model does **not** own:

```text
source authority
package/version identity
repository identity
exact quote text
exact offsets
target relevance
compatibility
safety
maintainer action
```

Ali must understand why model-produced prose or candidate data cannot become a trusted claim merely because it appears plausible.

### 5.9 Conditional target-Python activation

Primary source areas:

```text
src/upgradepilot/investigation.py
src/upgradepilot/target/python.py
src/upgradepilot/target/relevance.py
```

Ali must understand the rule:

```text
no grounded upstream support-drop claim
→ target pyproject.toml is not acquired for this responsibility
```

and:

```text
grounded upstream support-drop claim
→ target Python evidence becomes relevant
→ acquire exact-head pyproject.toml
→ interpret requires-python
→ evaluate bounded relevance
```

Ali must understand that this is not merely an optimization. It expresses an evidence-sequencing principle:

> Activate a later investigation when earlier evidence establishes a real question that makes it relevant.

### 5.10 Target Python declaration and bounded relevance

Primary source areas:

```text
src/upgradepilot/target/python.py
src/upgradepilot/target/python_specifier.py
src/upgradepilot/target/relevance.py
```

Ali must understand the basic TOML structure:

```toml
[project]
requires-python = ">=3.10"
```

Ali should distinguish:

```text
file unavailable
malformed TOML
[project] absent
requires-python absent
requires-python invalid
valid declaration
```

Ali must understand the bounded relevance question:

> Does the dropped Python X.Y line intersect any stable X.Y.Z release admitted by the target's declared `requires-python` range under the project's accepted method?

Ali must recognize basic PEP 440 operators used here:

```text
>=  >  <=  <  ==  !=  ~=
```

and the role of `packaging.specifiers.SpecifierSet` / `packaging.version.Version`.

Ali does not need to independently reproduce the candidate-version algorithm.

Most importantly, Ali must distinguish:

```text
outside_declared_python_range
```

from:

```text
compatible
safe
safe to merge
recommended action
```

Those are not equivalent claims.

### 5.11 Application orchestration versus domain logic versus CLI

Primary source areas:

```text
src/upgradepilot/investigation.py
src/upgradepilot/cli.py
```

Ali must understand the responsibility split:

```text
provider/acquisition modules
→ talk to external systems and return validated evidence

domain modules
→ answer bounded questions about that evidence

investigation.py
→ sequences/co-ordinates the evidence graph

cli.py
→ arguments, environment input, rendering, shell exit policy
```

Ali should be able to reason about where a new sequencing decision belongs and why `cli.py` should not become a duplicate orchestration layer.

### 5.12 Generality versus authority — current Step 7F live gap

The 2026-08-05 normal S001 run established PR/dependency/CI/PyPI evidence and then stopped at upstream repository resolution because Soup Sieve exposed its repository through:

```text
Homepage -> https://github.com/facelessuser/soupsieve
```

while the resolver previously admitted a narrower set of repository-association labels.

The correction admitted normalized `Homepage` candidates but preserved the stronger authority rule:

```text
admitted metadata candidate
+ canonical GitHub repository URL
+ usable exact-distribution PyPI provenance
+ one supported GitHub publisher repository
+ metadata/provenance repository agreement
→ UpstreamRepositoryEvidence
```

Ali must understand this distinction by the checkpoint:

> Broadening the accepted input spelling is not the same as weakening the trust boundary.

Ali should also understand why ambiguity remains explicit, for example two admitted labels pointing to different repositories.

### 5.13 Local HTTP inference and proxy diagnosis

Ali must understand the practical meaning of:

```text
127.0.0.1
loopback
port 12345
HTTP request
proxy
NO_PROXY
requests.Session
session.trust_env = False
timeout
HTTP status
```

Ali should be able to explain the recent failure family:

```text
intended local LM Studio request
→ ambient HTTP proxy inheritance
→ request did not follow the intended direct loopback transport
→ direct no-proxy control succeeded
→ product session now disables ambient environment inheritance
```

Deep TCP/IP mastery is not required, but Ali should understand why a request targeting `127.0.0.1` can still be affected by client proxy configuration.

## 6. Level-B responsibilities

### 6.1 GitHub and external API acquisition

Ali should understand operationally:

```text
HTTP request
→ status/response
→ JSON
→ validation
→ typed internal evidence
```

Required concepts:

- REST API;
- GET/request-response model;
- HTTP status;
- JSON;
- pagination;
- timeout;
- public/anonymous request;
- token/authorization context;
- SHA identity;
- exact revision;
- malformed response;
- acquisition failure.

Deep GitHub endpoint memorization is not required.

### 6.2 PyPI package identity and provenance

Primary source areas:

```text
src/upgradepilot/pypi/release.py
src/upgradepilot/pypi/provenance.py
src/upgradepilot/upstream/repository.py
```

Ali should understand the difference between:

```text
PyPI says package/version X exists
```

and:

```text
publisher/provenance evidence supports association with upstream repository Y
```

Ali does not need deep PyPI API/provenance internals.

### 6.3 URL parsing and normalization

Ali should recognize:

```python
urllib.parse.urlsplit(...)
```

and understand why canonical repository parsing rejects unsupported schemes, hosts, credentials, query/fragment data, ports, or unexpected path structures before treating a URL as a GitHub `owner/repository` identity.

Ali should understand normalization as converting multiple presentation spellings into a stable comparable form without changing authority.

### 6.4 Git tags, commits, and immutable source

Ali should understand:

```text
version
→ admitted tag spelling
→ resolved commit SHA
→ exact file at that immutable commit
```

and why the current bounded fallback tries only:

```text
<version>
v<version>
```

when the direct spelling is explicitly unavailable.

Deep Git object internals are deferred.

### 6.5 Structured LLM output

Ali should understand why UpgradePilot uses a strict structured JSON contract instead of trusting free-form model prose.

Required operational concepts:

```text
JSON object / array / string / boolean
strict schema
allowed/enumerated values
json.loads(...)
provider response parsing
malformed or incoherent result → unresolved
```

Ali does not need to memorize the full contract-v2 schema.

### 6.6 Dependency injection for testability

Ali should understand why central functions accept optional clients/evaluators such as:

```python
pull_client=None
actions_client=None
repository_client=None
package_client=None
support_drop_evaluator=None
```

and then use the supplied implementation or a real default.

Practical meaning:

> Production can use real external clients while tests can inject controlled doubles/mocks without changing the application orchestration.

Independent framework-level dependency-injection mastery is not required.

### 6.7 CLI and package basics

Ali should understand:

```toml
[project]
name = "upgradepilot"
requires-python = ">=3.12"

[project.scripts]
upgradepilot = "upgradepilot.cli:main"
```

and operationally recognize:

```python
argparse
os.getenv("GITHUB_TOKEN")
```

Ali should understand that the console-script entry point invokes `upgradepilot.cli.main` and that shell exit codes distinguish success/error classes.

Setuptools internals are deferred.

## 7. Python language and code-reading checkpoint

By 2026-08-18 Ali should comfortably read the following constructs when they appear in central UpgradePilot code.

### Required control flow and expressions

```python
def ...
return
if / elif / else
for
try / except
raise
assert
is / is not
in / not in
and / or / not
```

### Required collections

```python
list
tuple
dict
set
```

and ordinary comprehensions/generator expressions such as:

```python
[x for x in values]
{x for x in values}
tuple(x for x in values)
```

### Required built-ins / inspection helpers

```python
next(...)
any(...)
all(...)
len(...)
sorted(...)
isinstance(...)
type(...)
getattr(...)
```

### Required typing syntax

```python
str | None
Foo | Bar
tuple[Foo, ...]
list[Foo]
dict[str, object]
Sequence[Foo]
Callable[[A], B]
Literal["a", "b"]
```

Ali should understand the practical purpose of union types and narrowing with `isinstance(...)`.

### Required classes and dataclasses

Ali should recognize and explain approximately:

```python
class Foo:
    def __init__(...):
        ...

@dataclass(frozen=True, slots=True)
class Evidence:
    ...
```

Required understanding:

- class / instance;
- constructor / `__init__`;
- dataclass-generated record behavior;
- `frozen=True` as intentional immutability;
- `slots=True` as constrained attribute layout / avoidance of arbitrary new instance attributes at this level of depth.

### Required imports

Ali should be comfortable with ordinary and relative imports such as:

```python
from .target.python import ...
from ..github.repository import ...
```

### Required keyword-only arguments

Ali should understand the practical meaning of:

```python
def foo(value, *, client=None):
    ...
```

where parameters after `*` must be supplied by keyword.

### Recognize but do not master yet

```python
Protocol
field(init=False)
__all__
advanced generic typing
type-checker suppression comments
```

## 8. Testing checkpoint

By 2026-08-18 Ali should understand representative tests well enough to explain:

```text
setup
→ action
→ assertion
→ behavior protected
→ what would make the test fail
→ what the test does NOT prove
```

Required concepts from the current `unittest` style:

```python
unittest.TestCase
Mock
patch
return_value
assertEqual
assertIsNone
assertIsInstance
assert_called_once_with
assert_not_called
```

Ali should understand the practical distinction among:

```text
unit test
integration test
controlled end-to-end proof
live proof
regression suite
```

The Step-7F controlled proof is a key example:

```text
controlled external acquisition/model response
+ real source-window logic
+ real semantic adapter/reconstruction
+ real deterministic claim admission
+ real conditional target activation
```

Ali should understand why `assert_not_called()` before a grounded claim and `assert_called_once_with(..., "pyproject.toml")` after a grounded claim are architecture/orchestration proofs rather than testing trivia.

The checkpoint does not require understanding every test in the repository.

## 9. Exceptions versus explicit problem values

Ali should be able to distinguish:

### Programming/contract violation

Examples:

```python
raise TypeError(...)
raise ValueError(...)
```

when an internal API receives an invalid type/state combination.

### Expected product uncertainty or evidence failure

Examples conceptually:

```text
TargetPythonDeclarationProblem
DependencyChangeProblem
UpstreamRepositoryProblem
```

when a real external/evidence condition cannot establish the required fact.

Ali should be able to explain why not every expected evidence problem should become an exception.

## 10. Tools Ali should use comfortably

### Python/application execution

```bash
python
python -m upgradepilot ...
```

### Tests

Ali should know how to:

```text
run one relevant test file
run a focused test/case using the project's current runner
run the active regression suite when instructed
identify the first meaningful failure
separate a test failure from an external live-proof failure
```

### Git

Required ordinary commands/concepts:

```bash
git status
git diff
git log
git show
```

Ali should inspect what changed before/after meaningful AI-assisted work and understand the purpose of commits/diffs at a practical level.

### Local runtime / HTTP

Ali should recognize and safely use the current LM Studio local endpoint context and understand the proxy/environment issue described above.

### Repository navigation

Ali should increasingly locate behavior by responsibility/package rather than treating the repository as an undifferentiated set of files.

## 11. Source familiarity tiers

### Tier 1 — know best by 2026-08-18

Ali should be able to navigate and explain central behavior in:

```text
src/upgradepilot/investigation.py
src/upgradepilot/dependency/change.py
src/upgradepilot/ci/dependency_exercise.py
src/upgradepilot/upstream/repository.py
src/upgradepilot/upstream/support_drop.py
src/upgradepilot/upstream/support_drop_extractor.py
src/upgradepilot/target/python.py
src/upgradepilot/target/relevance.py
src/upgradepilot/cli.py
```

This does not mean line-by-line memorization.

### Tier 2 — understand owner/responsibility and important behavior

```text
src/upgradepilot/dependency/analysis.py
src/upgradepilot/dependency/requirements.py
src/upgradepilot/dependency/uv_lock.py
src/upgradepilot/dependency/versioning.py

src/upgradepilot/github/api.py
src/upgradepilot/github/pull_request.py
src/upgradepilot/github/actions.py
src/upgradepilot/github/repository.py
src/upgradepilot/github/tag.py
src/upgradepilot/github/changelog.py

src/upgradepilot/pypi/release.py
src/upgradepilot/pypi/provenance.py

src/upgradepilot/upstream/interval.py
src/upgradepilot/upstream/interval_evidence.py
src/upgradepilot/upstream/changelog.py
src/upgradepilot/upstream/claim.py

src/upgradepilot/target/python_specifier.py
```

### Level C / deferred source depth

No checkpoint requirement exists to master every helper, every provider edge case, every experiment/tool, every test, or every historical module.

## 12. Required ownership evidence before the checkpoint

Knowledge alone is insufficient. Career should seek at least these evidence classes from real UpgradePilot work.

### 12.1 One meaningful modification

A real current responsibility where Ali can explain:

```text
requirement/problem
→ his prediction or technical model
→ modification he performed or materially directed
→ changed behavior
→ how the result was verified
→ what assistance AI supplied
```

AI may write substantial code; ownership depends on Ali understanding and materially controlling the bounded change.

### 12.2 One meaningful test responsibility

Ali should be able to take a representative relevant test and explain:

```text
setup
→ action
→ assertion
→ invariant/behavior protected
→ changed case
→ failure meaning
→ limitation of the proof
```

Preferably Ali materially alters or adds one case when the real project naturally requires it.

### 12.3 Real debugging/diagnosis evidence

At least one defensible case should show:

```text
symptom
→ Ali's initial localization/hypothesis
→ discriminating evidence
→ corrected model if needed
→ repair
→ verification
```

The existing proxy incident counts as meaningful bounded evidence. A second natural case is desirable if real work produces one; do not manufacture a fake failure simply to satisfy this file.

### 12.4 One delayed reconstruction

After at least roughly a day away from the immediate explanation, Ali should reconstruct the current system from memory before reopening project-local teaching material.

Career should compare retained structure with the actual current architecture and record both accurate understanding and gaps.

### 12.5 One challenge or independent prediction

Prefer at least one case where Ali:

- challenges an AI assumption/design/debugging direction;
- predicts the behavior/test consequence before implementation;
- identifies a likely failure boundary before AI provides the answer.

Correctness is useful but not mandatory; the evidence goal is Ali making his own technical model explicit and revising it from evidence.

## 13. Questions the 2026-08-18 assessment should be able to ask

The assessment should sample, not mechanically administer all questions. Ali should be able to answer most of the central questions coherently without first reading an AI-generated answer.

### Product and evidence doctrine

1. What exactly does UpgradePilot currently do?
2. What does it explicitly not decide?
3. What does “evidence-backed” mean in this project?
4. Why are unavailable/conflicting states recorded rather than guessed through?

### Dependency change

5. What is a `DependencyVersionChange`?
6. Why is a changed dependency file not automatically trusted dependency identity?
7. Why normalize package names?
8. Why preserve exact base/head/source identity?
9. What should happen if two admitted sources establish conflicting transitions?

### CI

10. Why is “GitHub Actions passed” insufficient?
11. What does “dependency exercise proven” mean under the current rule?
12. Why must the workflow evidence correspond to the exact PR head?
13. What is the difference between a successful job and a proven dependency-exercise path?
14. Why is CI independent from upstream semantic investigation?
15. What does unresolved CI mean, and what does it not mean?

### PyPI / upstream repository

16. What does exact PyPI package/version evidence establish?
17. What does PyPI package existence not establish?
18. How does UpgradePilot currently establish a trusted upstream repository?
19. Explain the Step-7F `Homepage` failure.
20. Why did accepting `Homepage` not weaken the trust model?
21. What happens when admitted metadata candidates disagree about the repository?

### Release interval / exact source

22. Why inspect all crossed releases instead of only the proposed version?
23. Why resolve a proposed version tag to a commit?
24. Why acquire source at an exact commit?
25. What does Step 7A do?
26. What does Step 7B do?
27. What is a deterministic source window?
28. Why preserve original line IDs and character offsets?
29. Why does oversized or structurally incomplete source become unresolved instead of silently truncated?

### LLM boundary

30. What is the LLM allowed to produce?
31. What is it not trusted to establish?
32. Why are candidates different from grounded claims?
33. What turns a candidate into a grounded support-drop claim?
34. Why is the model's own reproduced quote not trusted as source authority?
35. What should happen when HTTP/JSON/schema/model output is malformed or unavailable?

### Target Python

36. Why does target `pyproject.toml` remain inactive without a grounded upstream claim?
37. What does `[project].requires-python` mean?
38. What does `>=3.10` mean at the current depth?
39. What is PEP 440 used for here?
40. Why is `outside_declared_python_range` not equivalent to “safe to merge”?

### Architecture

41. What belongs in provider/acquisition code?
42. What belongs in a domain module?
43. What belongs in `investigation.py`?
44. What belongs in `cli.py`?
45. If a new evidence-sequencing decision is introduced, why is `cli.py` usually the wrong owner?

### Python/code reading

46. What is a dataclass and why are many evidence records frozen?
47. What does `Foo | Bar` mean?
48. What does `str | None` mean?
49. Why use `Literal[...]` for state vocabularies?
50. Why is `isinstance(...)` used frequently after a union result?
51. What does the `*` in a function signature do for following parameters?
52. Why use tuples/sets/comprehensions in evidence comparison?
53. What is the difference between returning a problem object and raising an exception here?

### Testing

54. What is a mock?
55. What does `patch()` do in the current test style?
56. Why inject clients/evaluators into `investigate_public_pull_request()`?
57. What does `assert_not_called()` prove in the Step-7F activation test?
58. What does `assert_called_once_with(..., "pyproject.toml")` prove?
59. What is the difference between a unit test, integration test, controlled end-to-end proof, live proof, and regression suite?
60. Why are controlled tests not a substitute for the selected live proof?

### Runtime/debugging

61. Reconstruct the proxy-contamination incident.
62. What does `session.trust_env = False` change?
63. Why can a loopback request still be affected by proxy configuration?
64. If a normal run stops at upstream repository resolution, which later work should not execute?
65. If semantic extraction returns no grounded claim, what target acquisition should not occur?
66. If CI is unresolved but upstream evidence succeeds, what can and cannot be concluded?

### Ownership

67. Show one meaningful current project change you personally understood and materially directed or modified.
68. Explain one representative test you understand, including what it does not prove.
69. Describe one real failure where your first hypothesis/localization mattered.
70. Describe one AI proposal/debugging direction/assumption you challenged.
71. Identify one important current UpgradePilot responsibility you still do not own.
72. Explain how you distinguish AI-generated project capability from your own technical capability.

## 14. Assessment method on 2026-08-18

Career should not score this as a trivia exam.

Use a mixed assessment:

```text
reduced-context explanation
+ source reading
+ changed-case prediction
+ representative test reasoning
+ modification evidence
+ debugging evidence
+ explicit uncertainty/non-claim
```

### Strong checkpoint result

A strong result would include:

- coherent reconstruction of the frozen core with only minor corrections;
- strong explanation of evidence/trust/claim boundaries;
- comfortable reading of central Python constructs;
- correct reasoning about representative source/test behavior;
- at least one bounded modification ownership candidate;
- meaningful test responsibility;
- real debugging evidence;
- ability to identify non-owned areas honestly;
- roughly 80% or more of sampled central questions answered coherently, with emphasis on “why,” not memorized vocabulary.

### Satisfactory checkpoint result

A satisfactory result would include:

- coherent high-level flow with some implementation/detail gaps;
- correct major evidence boundaries;
- D2-level reading/reasoning in central files;
- at least some ownership-bearing modification/test/diagnosis evidence;
- gaps clearly identified and routed back to UpgradePilot.

### Partial checkpoint result

A partial result would include meaningful project exposure and some correct understanding but show one or more material problems:

- system explanation still collapses without immediate AI support;
- recent implementation significantly outruns retained architecture understanding;
- tests remain mostly opaque;
- no meaningful modification/diagnosis evidence exists;
- Python constructs in central files remain too unfamiliar for effective source reasoning.

A partial result does not automatically require a strategy reset. Career should identify the smallest blockers and reassessment trigger.

### Unsupported stronger claim

Career must not promote broad D3/D4 merely because:

- UpgradePilot progressed rapidly;
- many tests pass;
- AI generated sophisticated code;
- Ali can repeat an immediate explanation;
- Ali ran commands successfully;
- the repository has many modules/commits.

Stronger claims require reduced-prompt, changed-case, modification, testing, and/or diagnosis evidence.

## 15. Evidence record to accumulate before the review

Do not create separate bureaucracy for every item. The project-local AI can preserve material evidence where UpgradePilot already records it, while Ali's daily Career note remains lightweight.

Before the review, Career should be able to recover approximately:

```text
Current UpgradePilot stage/gate:
Material responsibilities advanced since 2026-08-05:
Delayed reconstruction evidence:
Meaningful modification evidence:
Meaningful test evidence:
Debugging/diagnosis evidence:
Challenge/prediction evidence:
Most important still-unowned responsibility:
Current source-reading confidence:
Current workload/focused-time evidence:
AI assistance level for each ownership claim:
```

Evidence may come from UpgradePilot source/tests/working-memory, Career notes, commit history, and Ali's reduced-context explanation.

## 16. Deliberate learning time expectation

This checkpoint does not require a detached course.

Expected deliberate learning/consolidation effort from 2026-08-06 through 2026-08-17 is approximately **8–12 focused hours**, embedded inside the already planned UpgradePilot work rather than added as a separate curriculum.

The intended daily pattern remains approximately:

```text
Block A → make the current system more coherent
Block B → learn + build on the highest-value current responsibility
Block C → allow faster AI-assisted implementation while preserving one ownership action
```

UpgradePilot owns the exact teaching sequence and source/test exercise used to close a gap.

## 17. Explicitly deferred from this checkpoint

Do not spend the next period trying to achieve any of the following merely for the August-18 assessment:

- memorizing every class, state string, module, or test;
- understanding every `uv.lock` parser branch;
- mastering all GitHub endpoints;
- mastering Git internals;
- deep TCP/IP/networking;
- the full PEP 440 specification;
- setuptools/build-system internals;
- advanced regex;
- transformer/LLM internals;
- LM Studio internals;
- reproducing the strict JSON schema from memory;
- understanding all 300+ product tests;
- independently rewriting UpgradePilot from scratch;
- independently redesigning the complete architecture;
- advanced typing mechanisms that are not blocking current source comprehension.

The checkpoint is intentionally selective.

## 18. Relationship to market readiness

Meeting this checkpoint does not by itself make Ali application-ready and failing one subsection does not automatically prevent applications.

The 2026-08-18 Career review must combine this technical evidence with:

```text
workload/sustainability
portfolio/GitHub presentation
representative current market evidence
role-family/geography constraints
CV/positioning
application-readiness decision
```

This file answers only the technical capability/ownership portion of that decision.

## 19. Use before 2026-08-18

During UpgradePilot sessions, use this file as a **gap-selection reference**, not as a second project plan.

Correct use:

```text
Career checkpoint says CI exact-head reasoning is Level A
→ current UpgradePilot session reveals that gap
→ UpgradePilot teaching/implementation process closes it using real source/tests
→ material ownership evidence is preserved
```

Incorrect use:

```text
Career file says CI is Level A
→ Career invents a detached CI course or implementation exercise
```

The project remains the learning environment.

## 20. Change control

Keep this checkpoint substantially stable through 2026-08-18 so the assessment target does not move every time UpgradePilot commits new work.

Change it before the review only if:

- UpgradePilot undergoes a material architecture/responsibility change that makes part of the frozen core obsolete;
- Career changes the Day-30 capability objective;
- Ali explicitly changes the assessment goal.

Ordinary project progress should update UpgradePilot, not this Career checkpoint.
