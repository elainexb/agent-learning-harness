# AGENTS.md Editor — current guidance recheck

Date: 2026-10-06, Asia/Shanghai. Mode: AUDIT. Decision: CHANGE, proposal only.

This run follows the local agents-md-editor SKILL.md and references/output-contract.md. The user explicitly authorized a current-guidance audit and prohibited modifying AGENTS.md. Acceptance: establish current applicable standards, assess the effective instruction system, preserve user requirements, resolve consequential uncertainty, recommend only a supported minimal repair, validate statically, and rescan. No adoption, installation, application implementation, or behavior certification is authorized.

The existing placement preference and patch were reused after current verification. This is a recheck, not a history-free independent experiment. Memory supplied governance context; current target content, sources, and the actual prior user message were checked directly. Previous reports' claims of compliance were not treated as runtime evidence.

## Current Standard

REQUIRED describes documented loading mechanisms. RECOMMENDED describes official advice. INFERRED describes this audit's interpretation, not an OpenAI requirement to adopt a particular layout.

| Guidance | Source | Strength |
|---|---|---|
| Global guidance, overrides, project discovery, merge order, fallback configuration and size limits determine the file instruction chain. Without a project root, only the current directory is searched for project instructions. | [Custom instructions](https://learn.chatgpt.com/docs/agent-configuration/agents-md) | REQUIRED — mechanism |
| Keep personal defaults global and project rules close to their scope; rich reusable workflows can use skills and progressive disclosure. | [Customization](https://learn.chatgpt.com/docs/customization/overview) | RECOMMENDED |
| Keep guidance practical, state goals and completion, and reference task-specific Markdown for detailed planning/review/architecture procedures. | [Best practices](https://learn.chatgpt.com/guides/best-practices) | RECOMMENDED |
| Revisit permanent instructions; read relevant documents, calibrate tests, and review approval boundaries and premature stopping. The September 11 article includes model-specific advice, so it does not justify deleting explicit user governance. | [Instruction maintenance](https://developers.openai.com/blog/rethinking-skills-and-prompts-for-gpt-6-astra) | RECOMMENDED |
| Make explicit user instructions take precedence over skill guidelines; identify the skill and instruction responsible for a pause. | [Instruction following](https://developers.openai.com/api/docs/guides/latest-model#instruction-following) | RECOMMENDED; supported by current host instructions |
| Current repository skill discovery uses .agents/skills; metadata discovery, full instructions and supporting resources are distinct loading stages. | [Build skills](https://learn.chatgpt.com/docs/build-skills) | REQUIRED — documented discovery mechanism |
| Evaluate behavior using actual traces/artifacts and checks; define outcomes before judging improvement. | [Skill evaluations](https://developers.openai.com/blog/eval-skills) | RECOMMENDED |
| Moving Sections 3/4 verbatim into a mandatory conditional reference is a suitable minimal adaptation here. | Source recommendations above plus verified prior user preference | INFERRED |

All source pages were opened in this run. Follow-up searches revisited AGENTS hierarchy, maintenance, completion, instruction conflict and verification; they added no new material target dimension. This is bounded coverage of the current personal-global audit, not proof that no further guidance or failure mode exists. Markdown endpoint retrieval failed; ordinary HTML pages and relevant sections were successfully read.

## Gap

The target `/Users/xuebai/.codex/AGENTS.md` contains 20 rules and 6,935 bytes. Sections 3/4 contain nine detailed research/architecture rules, 3,118 bytes. They enter context even for tasks where those procedures do not apply. Section 6 already scales execution by task and risk, so the gap is placement of detailed context, not absence of task applicability.

A simple translation can follow every current rule while carrying the research/architecture procedures. This is a structural counterexample. It does not demonstrate excess billing, latency, or an observed behavior failure.

The prior consequential tradeoff was whether to retain always-visible detail or require conditional loading with another file/read step. The actual user-message history was checked: after a beginner explanation of both options and their unverified runtime benefits, the user answered “可以，我同意你的建议” at 2026-10-06T03:30:15.320Z. That confirms the placement recommendation only. It authorizes neither application of this patch nor acceptance of its effectiveness.

The installed grilling procedure was read. Its frontier is empty for this recheck: target, no-edit restriction, requirement preservation and placement choice are settled. No material new evidence changes that choice. Accordingly, no repeated interview or subagent fact-finding round is necessary.

### Material dimension rescan

| Dimension | Current evidence and counterexample/limit | Conclusion |
|---|---|---|
| Target and discovery | No Git project, no cwd AGENTS/override, no global override; CODEX_HOME and project-doc settings unset. User-injected rules match global content. | Current target supported; fresh-session automatic discovery unverified. |
| Size/truncation | 6,935 bytes is below the documented default 32 KiB cap. | No measured size-limit defect; being under the cap does not prove good design. |
| Personal/project scope | Rules are personal cross-project working agreements. | Retain global gates; project commands should not be invented here. |
| Goal/examples/completion | Sections 1/2/5 specify real materials, scope, acceptance, full-scale evidence and user acceptance. | Static coverage; representative execution unverified. |
| Context placement | All nine procedure rules always present; translation counterexample above. | Supported MOVE repair. |
| Relevant reading and proportionality | Sections 2/5/6 preserve applicable stages, prior evidence and risk scaling. | Static coverage; excessive reading/research in actual small tasks unverified. |
| Decision and approval boundaries | Consequential unresolved choices trigger grilling; routine execution reuses valid approvals. | Preserve explicit gates; actual excess approval frequency unverified. |
| User/skill conflicts | Host instructions prioritize user instructions and require disclosure of skill-caused pauses. | Covered in this effective session; standalone portability of that host rule unverified. |
| Persistence and authorized scope | Complete-work/evidence rules coexist with explicit scope and acceptance gates. | No supported reason to remove those gates; actual premature stopping unverified. |
| Validation and evidence honesty | Original rules distinguish documented/source/local/accepted evidence and normal/boundary/negative cases. | Static coverage; wording does not certify effectiveness. |
| Maintenance and instruction adoption | One canonical fact source, risk scaling and no application authority from rule edits remain explicit. | Static coverage; current request prohibits adoption. |
| Skill integration | Editor manually read from visible skills/ and passed structural validation. README/INSTALL still recommend .codex/skills; SKILL.md does not link its existing output-contract reference. | Package integration issues surfaced; automatic discovery and contract loading unverified. Separate from this global-file patch. |

The audit does not conclude that every other dimension fully complies. Conclusions are separated into supported content/configuration, bounded static coverage, package integration issues, and unavailable runtime evidence.

## Candidate Learning

NONE. No supplied Candidate Learning; a prior user placement preference is not fabricated feedback learning.

## Decision

CHANGE — recommend MOVE, without applying it.

The decision rests on current layering guidance, the measured placement delta, a verified user tradeoff, and static preservation. It does not rely on unmeasured runtime benefits.

## Proposed Change

- Target: `/Users/xuebai/.codex/AGENTS.md` and proposed `/Users/xuebai/.codex/references/research-and-architecture.md`.
- Current state: all 20 original rules live in the global file.
- Proposed state: retain 11 original core rules plus a mandatory router globally; move nine rules in Sections 3/4 byte-for-byte into one reference.
- Rationale: conditional access to detailed procedures while preserving research, architecture, implementation, approval and evidence obligations.
- Minimal complete patch: [Existing verified two-file MOVE patch](/Users/xuebai/Downloads/agent-learning-harness-v0.1-visible/feedback/records/agents-md-editor-2026-10-06-proposed-move.patch). Includes the new reference; applying only the router would leave a missing dependency.

Compared alternatives: NO_CHANGE keeps direct visibility and one-file maintenance but retains irrelevant startup detail; DELETE or paraphrase adds unnecessary preservation risk; a new Skill adds discovery/installation/metadata work; a plain mandatory reference is sufficient for the settled placement choice. No dependency or model/framework change is needed.

Global body: 6,935 → 4,465 bytes, reducing it by 2,470 bytes (35.62%). Applicable-task bodies total 7,583 bytes, 648 more than the original before tool overhead. These are body-byte counts, not tokenizer, total-context, fee or speed measurements. This chat already includes the full rules in a user message; a future file edit cannot remove that existing message.

## Validation

| Check | Result | Scope |
|---|---|---|
| Standard alignment | PASS | Proposed conditional reference fits current recommendations and the verified user choice. |
| Behavioral preservation | PASS | Static obligation preservation: all 20 original rules exactly once; moved block unchanged. Runtime equivalence unverified. |
| Conflict check | PASS | Approval gates, applicability, routine-execution exceptions and no-edit restriction preserved; router grants no approval. |
| Regression check | PASS | Static boundary analysis, negative integrity assertions, patch applicability and unchanged-target check. No agent-run suite. |

Static normal/boundary/negative analysis:

- Research, feasibility experiments, dependency/framework selection, architecture design/review/change, implementation/code review and contract/workflow reuse explicitly trigger reading before affected work.
- Previously approved small fixes still use Section 6 applicability and Section 5 approval reuse.
- Pure translation/formatting without those tasks does not trigger the detailed reference.
- Unavailable or incomplete reference requires disclosure and pausing dependent work while independent authorized work continues. Detection of completeness in a future drifted reference remains unverified.
- Executed integrity negatives reject a missing clause, duplicated clause and removed architecture approval. They validate the comparison checks, not the agent's real response to these conditions.

Actual commands/results:

1. `codex-skill-validate skills/agents-md-editor`: exit 0, `Skill is valid!`; inspected wrapper uses its dedicated Python environment. Structure only.
2. Python static assertions: initial verifier exited 1 because the parser omitted unchanged blank-line diff context. Corrected parser exited 0; no target file was written in either attempt.
3. `git apply --check` on the complete existing patch against a temporary baseline copy: exit 0. No patch applied; temporary baseline unchanged and no temporary reference created.
4. Global target SHA-256 before/after: `a1acc7690963c37f21c908421975c8b42b5a668acf5fa8a45777c4a2dfee1e42`. Proposed global reference still absent.

[Machine-readable recheck evidence](/Users/xuebai/Downloads/agent-learning-harness-v0.1-visible/feedback/records/agents-md-editor-2026-10-06-recheck-validation.json).

## Evidence

Current official pages linked above; global file and safe selected configuration fields; current user/host instructions; editor SKILL.md/output contract; installed grilling; README/INSTALL/router snippet/starter evals; actual prior user clarification/confirmation messages; complete existing patch; commands and recheck JSON.

Rescan: the placement gap is addressed by the proposal only. No further global-file repair has sufficient evidence from this review. Runtime loading, missed triggers, cross-project behavior, reading/testing/approval frequency, tokens/cost/latency and maintained-reference drift remain unverified. Skill installation and reference linkage are separate surfaced package gaps. No consequential choice remains pending for this bounded proposal; the next boundary is user review and, if later authorized, adoption and representative runtime verification.

Only this recheck record and its JSON evidence were written. AGENTS.md, the proposed reference, existing patch, skills, installation documentation, configuration and memory were not modified.

## Follow-up: authorized skill closure update

After the user challenged premature audit closure, the user approved updating the skill with “ok, make this change.” This follow-up changes `skills/agents-md-editor/SKILL.md` Steps 4/7 and Completion, and its output contract. It requires per-dimension behavior/counterexample/evidence review, substantiated barriers before accepting evidence limitations, continued independent authorized work, an AUDIT-only review ledger and completion status, and validation scoped to the named object. The entrypoint now links the output contract; PATCH remains scoped to the known issue and directly introduced regressions. No AGENTS.md adoption is authorized by this update.

Validation: `codex-skill-validate skills/agents-md-editor` exited 0 (`Skill is valid!`). Source diffs were reviewed; diff exits 1 indicate expected differences. Readback confirmed the referenced contract exists and global AGENTS.md retains the SHA-256 recorded above. Static boundary review checked that one repair plus remaining feasible checks cannot close an audit; unavailable evidence needs an attempted investigation and specific barrier; a pending user decision does not halt independent work; and PATCH does not require a whole-system audit ledger. These are instruction/contract checks, not independent model-execution tests or proof of improved adherence. The original audit's unverified dimensions remain unverified; this skill edit does not retroactively complete them.
