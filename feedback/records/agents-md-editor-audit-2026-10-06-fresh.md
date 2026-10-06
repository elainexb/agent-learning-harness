# Independent AGENTS.md audit — 2026-10-06

## Run boundary

Asia/Shanghai. The user requested a fresh assessment using agents-md-editor, current official guidance, grilling for consequential uncertainty when necessary, and the skill's output contract. AGENTS.md must not be modified; show a patch only for CHANGE.

No persistent memory file or previous audit record was read for this run. Existing conversation history could not be physically erased through the available tools; previous verdicts and candidate recommendations were excluded from this assessment's inputs. This separate record is necessary to preserve the independent run's evidence without importing earlier conclusions. It is the record for this run only.

Mode: AUDIT. Scope: effective instructions for the current directory, principally `/Users/xuebai/.codex/AGENTS.md`. This is an instruction-content assessment, not an automatic-discovery, cross-project, or runtime-performance certification.

Acceptance: discover current applicable standards; normalize their target behaviors; attempt a counterexample for every evaluated target; separate coverage from materiality; preserve user requirements; resolve or surface consequential decisions; rescan; report the required fields and actual verification limits. The explicit request authorizes this research. No application implementation, skill installation, governance migration, or recurring automation is authorized by it.

## Current Standard

REQUIRED denotes documented mechanisms or structural requirements. RECOMMENDED denotes official advice, including conditional model/workflow advice. INFERRED denotes an explicitly bounded interpretation. None implies that every source must be copied into AGENTS.md.

| ID | Guidance | Source | Strength | Applicability and relationship |
|---|---|---|---|---|
| S1 | Codex home guidance and overrides, project discovery, merge precedence, nonempty-file selection, and configured size limits determine applicable instructions. | [AGENTS.md documentation](https://learn.chatgpt.com/docs/agent-configuration/agents-md) | REQUIRED | Establishes this audit's target. Default cumulative limit is 32 KiB; a file below it is not thereby well designed. |
| S2 | Confirm effective instructions in a new run after adoption. | [AGENTS.md documentation](https://learn.chatgpt.com/docs/agent-configuration/agents-md) | RECOMMENDED | Complements S1; conditional on an applied change. |
| S3 | Put personal defaults globally, project rules near their code, and rich repeatable workflows in skills or supporting resources. | [Customization](https://learn.chatgpt.com/docs/customization/overview) | RECOMMENDED | Separates the global target from installation documentation and project-specific commands. |
| S4 | Use practical, accurate guidance; prefer focused rules grounded in recurring friction; make goals, constraints, completion, and verification clear. | [Best practices](https://learn.chatgpt.com/guides/best-practices) | RECOMMENDED | Supports both restraint in adding rules and explicit acceptance. |
| S5 | Reassess instruction necessity, use task-relevant context, and review boundaries that create excessive reading, testing, approval pauses, or premature stopping. | [Instruction maintenance, 2026-09-11](https://developers.openai.com/blog/rethinking-skills-and-prompts-for-gpt-6-astra) | RECOMMENDED | Model-sensitive advice, related to S3/S4; does not automatically override explicit user process requirements. |
| S6 | Follow through on authorized work; respect explicit user instructions over skill guidelines; identify skill-caused pauses; use relevant tests and justified retesting. | [Current model prompting](https://developers.openai.com/api/docs/guides/latest-model) | RECOMMENDED | Applies to effective host guidance as well as the file. The source calls for evaluation on the chosen model/workload. |
| S7 | Skills require name/description, use progressive disclosure, and currently use `.agents/skills` for repository discovery. | [Build skills](https://learn.chatgpt.com/docs/build-skills) | REQUIRED | Structural/discovery mechanisms; explicit manual loading does not verify automatic discovery. |
| S8 | Give skills focused triggers, inputs, outputs, decisions, resource references, and representative positive/negative requests. | [Build skills — Plugins](https://developers.openai.com/plugins/build/skills) | RECOMMENDED | Complements S7 and the editor's workflow/contract; not an instruction to rewrite skills in this audit. |
| S9 | Support behavioral claims with actual runs, traces, artifacts, and negative controls; package validity is insufficient. | [Skill evaluations, 2026-01-22](https://developers.openai.com/blog/eval-skills) | RECOMMENDED | Defines the limit of static counterexample analysis and validator results. |
| S10 | Sandbox and approval policies control real execution. | [Agent approvals & security](https://learn.chatgpt.com/docs/agent-approvals-security) | REQUIRED | Separate from written workflow approval. No policy configuration change is needed. |
| S11 | Bound delegated work, respect explicit user/project/skill triggers, and account for token/coordination costs. | [Subagents](https://learn.chatgpt.com/docs/agent-configuration/subagents) | RECOMMENDED | Relevant if an unresolved grilling decision needs delegated fact-finding; no such decision emerged here. |
| S12 | In a long implementation run, follow the accepted plan, keep diffs scoped, and verify milestones. | [Long-horizon experiment, 2026-02-23](https://developers.openai.com/blog/run-long-horizon-tasks-with-codex) | RECOMMENDED | A scoped experimental workflow, not a universal rule forbidding the user from changing the plan or requesting optional improvements. |

### Discovery and saturation

The Standard Frontier began with AGENTS discovery, instruction maintenance, and customization. Adjacent discovery added practical prompting/completion, skill metadata/loading and priority, model-sensitive autonomy/testing, eval evidence, execution controls, subagent triggers, and scoped long-running implementation. Relevant official HTML bodies were opened and read.

Follow-up searches covered scope/correctness/minimal changes, instruction conflicts, maintenance, and validation. They returned already-covered guidance plus API/SDK repair loops, Goals, plugin submission, showcase examples, and older prompting recipes. Those specialized implementation surfaces do not establish additional requirements for this global-file audit. Scoped long-horizon guidance was separately examined instead of turning its example runbook into universal policy. The current Build skills reference governs local discovery recommendations; the older eval tutorial's installation example does not supersede it.

No material new applicable standard remained after these follow-ups and the final rescan. This is coverage saturation over the inspected official source frontier and available repository evidence, not absolute completeness.

## Effective instructions and actual materials

- CODEX_HOME: unset. Default target directory: `/Users/xuebai/.codex`.
- Global AGENTS.md exists; global override is absent.
- Current directory AGENTS.md and override are absent.
- `git rev-parse --show-toplevel`: exit 128, no Git root. The documented project discovery check therefore applies only to cwd.
- Focused user-config inspection found no project_doc_max_bytes or project_doc_fallback_filenames entries. Managed/client settings were not exhaustively audited; the global rules are also explicitly present in the current user-supplied instructions.
- Actual file: 6,935 bytes, 20 rules, SHA-256 `a1acc7690963c37f21c908421975c8b42b5a668acf5fa8a45777c4a2dfee1e42`.
- Read current editor SKILL.md, output contract, installed grilling SKILL.md, README, INSTALL, TREE, router snippet, and editor starter eval definitions. Prior records were excluded. The router snippet is an unapplied proposal, not a discovered AGENTS.md.
- Effective host instructions already address user/skill priority, persistence within authorization, proportional verification, permission enforcement, and delegation triggers. These are not assumed to be portable to every other host.

## Gap

### Normalization, counterexample attempts, coverage, and materiality

Behavior strength below describes the target behavior rather than the source's authority. An example here is a static logical challenge to the actual instruction text, not a real agent execution or an observed project failure.

| Target | Scope / trigger; expected behavior; strength; exception | Counterexample attempt and evidence | Coverage | Materiality / disposition |
|---|---|---|---|---|
| T1: Applicable guidance (S1) | Start in this cwd; use the applicable file/override chain; REQUIRED; configured names/limits may vary. | Treat the router snippet as an automatically loaded AGENTS file. It has a different name and was not configured as a fallback; the inspected chain and explicit prompt identify the global rules. No compliant counterexample found for this assessed chain. | COVERED | No AGENTS content gap. Runtime discovery elsewhere remains untested. |
| T2: Reload validation (S2) | After adoption; check a new run's instruction chain; DEFAULT; no applied change means no reload required. | Claim new-session loading without a new session. Actual adoption trigger is absent, and this report makes no such claim. | COVERED, conditional | No change needed in this no-edit run. |
| T3: Layer placement (S3) | Durable personal versus codebase rules; keep each at the relevant layer; DEFAULT; personal workflow gates may be global. | Add package-specific app commands globally. Current file contains personal governance and a reusable skill-validation command, not an invented application command. | COVERED | No missing project command or repo-file requirement follows for this global target. |
| T4: Concision/progressive disclosure (S3–S5) | Always-loaded guidance; keep the main file focused and move rich procedures when useful; DEFAULT; indispensable persistent constraints may remain. | A trivial task still receives the detailed comparison and reuse requirements at lines 16–27, even though line 38 permits risk-scaled execution. That demonstrates always-loaded detail; risk scaling does not remove its input size. | PARTIAL | Input overhead exists, but this run does not establish unnecessary clauses, measured behavior degradation, or a minimal relocation that preserves discovery and all constraints. No material change is justified merely by size. NO_CHANGE; no claim of optimal concision. |
| T5: Relevant reading (S5) | Inspect material needed for the task; DEFAULT; more context is appropriate for actual dependencies. | Read architecture/database/deployment manuals for every typo. Line 10 requires relevant context; line 38 scales research and reuses prior valid work. Such an unconditional reading requirement is absent and would not follow from the file. | COVERED | No demonstrated behavioral delta. |
| T6: Goal and finish line (S4) | Before consequential work; define outcome, scope, constraints, acceptance, and verification; REQUIRED under user policy; only applicable stages for other tasks. | Finish after a first artifact without checking agreed criteria. Lines 10, 18, 24, 33, 37 require criteria, evidence, and acceptance; the attempt violates them. | COVERED | No compliant counterexample found. |
| T7: Planning and task applicability (S4/S5) | Difficult/ambiguous work; plan before coding; DEFAULT in official advice, stricter user gates apply; valid prior design may be reused. | Select a framework first or code before approved design. Lines 6, 20, 24 prohibit it. Force a new full project process on an explanation: line 38 limits nonimplementation tasks to applicable stages. | COVERED | Preserving current user gates is supported; no new policy needed. |
| T8: Authorized continuation (S6) | Work within explicit authorization; continue independent work and routine checks; DEFAULT; consequential unresolved choices and execution controls still govern. | Ask again for routine retesting already authorized. Line 32 prohibits repeated approval/grilling; lines 12/38 preserve independent progress and settled decisions. | COVERED | No compliant counterexample for repeated routine approvals. Different user gates are intentional constraints. |
| T9: User/skill priority and pause disclosure (S6/S8) | A skill conflicts with explicit task instructions or causes a pause; honor the user and explain the exact skill cause; REQUIRED in the effective host; cannot bypass higher-priority controls. | Apply the editor's last step despite no-edit, or pause without identifying the responsible skill. Both violate the effective host and current user request. | COVERED | No new global duplication required; portability to a different host is unverified. |
| T10: Appropriate verification (S6/S9) | Validate agreed outcomes; use meaningful normal/boundary/negative checks; DEFAULT plus explicit user requirements; enlarge checks for justified concerns. | Treat one successful exit as proof of general correctness. Lines 18, 19, 33 explicitly reject that. Run irrelevant repeated suites: host verification rules and line 38's risk scaling do not justify it. | COVERED | Static reasoning is reported separately from runtime evidence. |
| T11: Skills and discovery (S7/S8) | Invoke this editor explicitly; read its full instructions/contract and available dependencies; REQUIRED; automatic discovery uses separate mechanisms. | Use only its name, omit its contract, or infer grilling availability. Actual full reads and dependency inspection supply evidence against that attempted failure for this run. | COVERED for explicit invocation | README/INSTALL use `.codex/skills`, differing from current `.agents/skills` documentation. Automatic discovery and legacy compatibility are untested. This is an installation-document issue, not a missing global AGENTS behavior. |
| T12: Execution boundary (S10) | Run tools under sandbox/approval policies; REQUIRED; written authorization cannot override enforcement. | Use an AGENTS approval as permission to bypass the sandbox. The effective permissions instructions forbid it; nothing in the global file requests bypass. | COVERED | No configuration or global policy change needed. |
| T13: Delegation (S11) | Delegate on applicable user/project/skill triggers with bounded ownership; DEFAULT; available host controls still apply. | Spawn unsolicited agents simply because an official example recommends parallelism. The effective host requires an applicable trigger. Grilling's delegated fact-finding applies if a question needs discoverable facts; no unresolved interview frontier occurred. | COVERED | No need to create agents or alter the file. |
| T14: Scoped implementation (S4/S12) | Execute an accepted plan; keep changes within its scope; REQUIRED in the user's current policy; approved changes can revise that scope. | Quietly make an unrelated change outside agreed scope while satisfying line 31. This fails: line 31 requires evidence, a revised design, and approval first. An approved new scope is a permitted change to the contract, not the same counterexample. | COVERED for this normalized target | No unapproved-scope gap demonstrated. This does not entail every possible stricter scope policy. |
| T15: Maintenance/evidence (S4/S5/S9) | Review relevant guidance during this audit and preserve attributable evidence; DEFAULT; ongoing scheduling needs its own request. | Declare that today's audit guarantees future compliance, or that textual starter cases prove behavior. Current report avoids these claims; lines 19/33/37 require evidence-state separation. | COVERED for this run | No automation or runtime certification follows from the task. |

### Additional scope hypothesis: analyzed, not adopted as a target

Hypothesis H1: an agent may propose a scope expansion only when the original task cannot be completed correctly without it. This is a stronger proposal policy than requiring approval before executing a scope change.

Concrete static counterexample: the agent completes the agreed task correctly, identifies an optional improvement, explains its cost and alternatives, and asks whether the user wants it as additional work. It performs no extra changes without approval. That can satisfy the existing rules, including lines 12, 26, and 31, while violating H1's restriction on proposals.

Thus H1 is not behaviorally entailed by current approval rules; if assessed as a hypothetical target, coverage would be PARTIAL. Its delta could materially affect which recommendations an agent can make. However, no provided Candidate Learning and no inspected current authoritative source establishes that stronger universal restriction as the desired policy for this run. S12 describes keeping executed diffs inside an accepted plan, not restricting every optional recommendation. H1 therefore fails the target-provenance gate for a material gap. It is not used to justify CHANGE and is not declared semantically equivalent to existing rules.

### Gap Frontier dispositions

- T4: NO_CHANGE; partial concision coverage preserved, material benefit and a necessary minimum change are unestablished.
- T11 installation-document difference: NO_CHANGE for AGENTS.md; explicit invocation works, automatic discovery is a separately unverified property.
- H1: excluded from the material Gap Frontier because its desired-policy provenance is absent; no inferred user policy or candidate learning is created.
- Remaining applicable targets: no demonstrated material unaddressed behavioral delta. No unresolved material gap requires an AGENTS patch.

## Candidate Learning

NONE. Provenance: NONE. No Candidate Learning was provided in this fresh request or produced by feedback-learning for this run. Audit-generated ideas remain hypotheses; they are not promoted to user requirements.

## Decision

NO_CHANGE.

Reason: the current-source targets have no demonstrated material AGENTS.md gap warranting a minimum patch. Partial coverage and unverified properties are retained above. NO_CHANGE does not assert perfect instruction quality, equivalence with every stronger proposed policy, or verified runtime behavior.

## Proposed Change

NONE. No AGENTS.md patch is emitted or applied.

### Grilling and Adapt

The installed grilling SKILL.md was actually loaded and its availability announced. No interview round was entered. Counterexample analysis resolves semantic differences; the explicit current user rules resolve approval boundaries; no applicable material target leaves a consequential repository policy choice that must be guessed. In particular, H1 is not a valid policy requirement simply because an auditor can imagine it.

Adaptation applies guidance at its actual level and trigger: preserve intentional user governance; use effective host priority/permission rules; keep repository installation issues separate; qualify model-related advice and runtime claims. No new governance choice was adopted.

## Validation

| Check | Result | Basis and limit |
|---|---|---|
| Standard alignment | PASS | The decision distinguishes authority, applicability, coverage, and materiality. T4 remains PARTIAL; this PASS is not a claim that every recommendation is maximally satisfied. |
| Behavioral preservation | PASS | No AGENTS rule was changed; all 20 rules retain the initial file identity. |
| Conflict check | PASS | No applicable override found; no-edit governs Apply; existing explicit user approvals are retained. |
| Regression check | PASS | Static counterexample review and unchanged-file verification only. No runtime improvement or cross-project generality is claimed. |

Source traceability, learning provenance, normalization, per-target counterexample attempts, partial-coverage handling, materiality, and both rescans were checked. The final instruction rescan repeated the target/trigger/exception analysis against the unchanged rules and found no new material gap. The Standard rescan found no new applicable dimension from those analyses. Both frontiers can close for this bounded audit.

Normal/boundary/negative checks include: completing already-authorized work; continuing independent work around unavailable evidence; preserving approval for genuine scope changes; refusing to treat no-edit as Apply authorization; not mistaking related wording for entailment; not mistaking an absent sentence for a missing behavior; not treating an audit hypothesis as a supplied learning; and not treating validator success as a behavioral test. These are logical checks of actual materials, not synthetic agent runs.

Actual commands and results:

- Read-only Python file/config inspection: exit 0. Established target, absence of overrides, initial digest, and focused project_doc settings.
- `git rev-parse --show-toplevel`: exit 128, no Git repository.
- Read `/Users/xuebai/.local/bin/codex-skill-validate`: exit 0. It selects the dedicated validator virtual environment's Python and official quick_validate.py.
- `codex-skill-validate skills/agents-md-editor`: exit 0, `Skill is valid!`. This establishes package structure only.
- Numbered AGENTS read and read-only identity calculation: exit 0. 6,935 bytes, 20 rules, same digest.
- Final read-only Python verification: exit 0. `FINAL_AGENTS_UNCHANGED: PASS`, `CURRENT_SKILL_UNCHANGED: PASS`, `OUTPUT_CONTRACT_READBACK: PASS`, 15 target coverage records, `MINIMAL_PATCH: NONE`. The AGENTS digest matched this run's captured baseline.

Initial AGENTS SHA-256: `a1acc7690963c37f21c908421975c8b42b5a668acf5fa8a45777c4a2dfee1e42`.

Editor SKILL.md SHA-256: `15bd0ad475b43ef7f3ece4d5d98a83ff07fe321e64226918e367ac7fe73415a7`.

Output contract SHA-256: `a407526a8cbabb346ef5539cd796e9bab4cdd1f3a4b1774dd9066af335186045`.

Grilling SKILL.md SHA-256: `fa5c1e5ee76b1c8f1ae56101f52c9e239de75d5c578adc61227b92d10b7e52ef`.

Limits: no fresh-session loader experiment, automatic skill-discovery test, runtime scenario suite, measured token/cost comparison, cross-project trial, or ongoing compliance guarantee. User acceptance remains separate.

## Evidence

Only S1–S12 official sources and the current materials listed above support this verdict. Relevant AGENTS clauses are lines 5–6, 10–12, 16–27, 31–33, and 37–39. The current skill's provenance, normalization, counterexample, materiality, rescan, and output requirements governed the audit. All repository evidence was collected in this run; no previous verdict was an input.

The only intended filesystem change is this independent audit record. AGENTS.md, skills, installation documentation, configuration, and persistent memory remain unchanged.
