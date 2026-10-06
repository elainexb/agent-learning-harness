# AGENTS.md Editor audit with review ledger

Date: 2026-10-06, Asia/Shanghai. Mode: AUDIT. Decision: CHANGE, proposal only. Audit Completion: COMPLETE within the authorized inspection scope; behavioral effectiveness is not certified.

The user authorized this skill audit and expressly prohibited modifying AGENTS.md. Outcome: current source-backed standards, a per-dimension counterexample/evidence assessment, preserved requirements and prior decisions, a minimal proposed repair, scoped validation, and a rescan. No adoption, installation, application work, configuration change, or independent model delegation is included. Only this record and its validation JSON are new workspace outputs. Historical reports are evidence to inspect, not authority for a present pass.

## Current Standard

| ID | Guidance | Source | Strength |
|---|---|---|---|
| S1 | Global and project discovery, overrides, fallback names, precedence, startup loading and a default 32 KiB limit determine the file instruction chain. | [AGENTS.md documentation](https://learn.chatgpt.com/docs/agent-configuration/agents-md) | REQUIRED: documented mechanism, not a mandate to duplicate its documentation |
| S2 | Keep durable guidance practical; distinguish personal defaults from repository rules; reference detailed task-specific planning, review and architecture guidance when useful. Define goal, context, constraints and completion. | [Best practices](https://learn.chatgpt.com/guides/best-practices) | RECOMMENDED |
| S3 | Keep permanent guidance focused, place it near its applicable scope, and use skills for rich repeatable workflows. Enforcement infrastructure complements instruction text. | [Customization](https://learn.chatgpt.com/docs/customization/overview) | RECOMMENDED |
| S4 | Revisit instruction relevance; avoid indiscriminate reading, excessive tests, unnecessary permission stops and premature completion. The September 11 advice includes model-specific qualifications. | [Instruction maintenance](https://developers.openai.com/blog/rethinking-skills-and-prompts-for-gpt-6-astra) | RECOMMENDED; does not override explicit user governance |
| S5 | Skill discovery, metadata loading, full SKILL.md loading and references are distinct stages. Current authoring guidance documents .agents/skills for repository skills. Keep triggers focused. | [Build skills](https://learn.chatgpt.com/docs/build-skills) | REQUIRED for documented mechanisms; RECOMMENDED for authoring choices |
| S6 | Evaluate outcomes and process using captured runs, artifacts and explicit checks, including negative trigger cases. Structural validation alone does not establish behavior. | [Skill evaluations](https://developers.openai.com/blog/eval-skills) | RECOMMENDED |
| S7 | Moving the detailed Sections 3–4 verbatim into one mandatory conditional reference fits this user's confirmed placement preference. | S2–S4 and the verified user decision below | INFERRED adaptation, not an OpenAI requirement |

All cited pages were opened. Follow-up searches covered AGENTS discovery, current authoring guidance, maintenance, evaluation and recent release history. The [current changelog](https://learn.chatgpt.com/docs/changelog) was also opened: its historical December 2025 entry documents .codex/skills, while the current Build skills page documents .agents/skills. This establishes a documentation/version distinction, not proof that every legacy path has stopped working. Local CLI version is 0.159.2; current documentation is not asserted to have been executed by that version. No latest-model recommendation is necessary for this audit.

## Gap

The global target has 20 rules and 6,935 bytes. Its nine detailed research/architecture rules occupy 3,118 bytes and enter initial instruction context regardless of task. Section 6 already limits applicable stages; the meaningful gap is context placement, rather than an absent applicability exception. A translation-only task can obey the original rules and still carry all research/architecture detail. This is a structural counterexample, not measured excess billing or an observed translation failure.

An actual prior user decision settles the tradeoff: the explanation compared always-visible detail against mandatory conditional loading, including the additional file/read step and unverified runtime benefit. The user replied “可以，我同意你的建议” at 2026-10-06T03:30:15.320Z. The underlying user message and preceding explanation were read from the session log, rather than accepted from an earlier report. This confirms placement only, not patch adoption or effectiveness acceptance.

The installed grilling entrypoint was read and announced. The decision tree has settled target, requirement preservation, no-edit scope and placement branches. No material new evidence changes that choice. Its frontier is empty for this proposal, so repeating the interview would conflict with reuse of settled decisions. No new consequential decision is silently assumed.

Separate findings: README/INSTALL still direct users to .codex/skills; the editor is in visible skills/ and is absent from this session's installed-skill catalog. This explicit invocation was fulfilled by locating and reading its source. Automatic discovery is not thereby demonstrated. The previously reported missing output-contract link has already been repaired: the current SKILL.md explicitly links the contract. Neither finding calls for a new global instruction. No package files were changed.

## Candidate Learning

NONE. No supplied Candidate Learning. Historical corrections are inspected as process evidence, not automatically persisted as a learning.

## Decision

CHANGE — recommend MOVE, preserving all original rules. No active change is applied.

NO_CHANGE alternatives were considered: retaining one file avoids another loading step but retains irrelevant startup detail; deletion/paraphrase introduces avoidable semantic risk; a new skill introduces discovery and installation work. A mandatory plain reference is sufficient for the confirmed placement choice. No claim is made that fewer bytes alone prove a better complete workflow.

## Audit Completion

COMPLETE: relevant directly permitted source, file, configuration, historical trace and deterministic investigations have been exhausted, with limits recorded below. COMPLETE does not mean that all behaviors pass.

The active candidate cannot be observed loading because the reference is absent and AGENTS.md adoption is prohibited. This chat's actual supplied instruction chunk matches the current global rules but cannot reveal whether an automatic loader or supplied context produced it. Local CLI help/version and actual historical traces were inspected; a fresh independent agent execution would be a new autonomous-agent run, for which the active host instructions require explicit delegation authority. No unresolved grilling frontier supplies that trigger here. Those runs were not launched. No attempted model execution is falsely claimed to have failed, and no network or credential barrier is invented.

The required next evidence for efficacy is captured normal/boundary/negative runs in the intended host, after a separately authorized candidate-loading trial or adoption: translation without loading the reference; research/selection and code review with loading before affected work; an approved small fix without renewed approval; changed architecture stopping only dependent work; missing/incomplete reference handling; and completion/reporting under source failure. Other clients/projects, longitudinal maintenance and actual fees need their own observable runs. A textual simulation or this audit's integrity assertions would not certify those properties. This audit closes their investigation as substantiated evidence limitations, not behavioral passes.

## Final Audit Summary

**Yes: update AGENTS.md for Dimension 5 only.** Move Sections 3–4 verbatim to the mandatory conditional reference using the existing unapplied patch. Keep the other AGENTS.md rules unchanged.

The decisions below answer whether each dimension warrants an AGENTS.md repair on the current evidence. NO_CHANGE means no AGENTS.md edit is recommended; it does not certify runtime behavior. NEEDS_DECISION would mean an unresolved user choice affects the repair; BLOCKED would mean the evidence needed to choose a repair is unavailable. Behavioral uncertainties remain separately recorded in the detailed ledger.

| Reviewed dimension | AGENTS.md repair decision | Action |
|---|---|---|
| 1. Target and discovery | NO_CHANGE | Keep the current target and hierarchy. |
| 2. Size and truncation | NO_CHANGE | No size-limit repair. |
| 3. Personal/project scope | NO_CHANGE | Keep personal defaults global. |
| 4. Goals and real examples | NO_CHANGE | Keep current goal/example requirements. |
| 5. Context placement | CHANGE | MOVE Sections 3–4 verbatim; retain mandatory routing. |
| 6. Proportional reading/research | NO_CHANGE | Keep applicability and prior-work exceptions. |
| 7. Research and feasibility | NO_CHANGE | Keep research and feasibility obligations. |
| 8. Architecture and reuse | NO_CHANGE | Keep architecture approval and reuse rules. |
| 9. Consequential decisions | NO_CHANGE | Keep grilling triggers and settled-decision reuse. |
| 10. Approval boundaries | NO_CHANGE | Keep approval gates and routine-work exceptions. |
| 11. Persistence and closure | NO_CHANGE | No duplicate global rule; the current editor already contains closure requirements. |
| 12. Testing proportionality | NO_CHANGE | Keep risk scaling and evidence requirements. |
| 13. Evidence honesty | NO_CHANGE | Keep evidence-state distinctions. |
| 14. User/skill hierarchy | NO_CHANGE | No duplicate rule for the effective host hierarchy. |
| 15. Maintenance and enforcement | NO_CHANGE | Keep canonical records and distinct adoption/acceptance gates. |
| 16. Skill integration | NO_CHANGE | No global rule repair; package installation documentation is a separate target. |

**Separate package-documentation repair: CHANGE** to README.md and INSTALL.md guidance to align with current .agents/skills authoring documentation while identifying the legacy/version distinction. That issue does not require an AGENTS.md edit. Package files remain unchanged.

No dimension has an unresolved user repair choice. Runtime uncertainty is not treated as a behavioral PASS or silently converted into a repair blocker.

## Review Ledger

G = current global AGENTS.md; H = effective host instructions; E = current editor skill and contract. “No further G patch” means no additional repair is justified by the named evidence; it does not mean runtime compliance.

| Dimension: expected behavior and scope | AGENTS.md repair decision | Intended instruction/mechanism | Concrete counterexample analysis | Evidence investigated and supported conclusion/repair | Remaining uncertainty, needed evidence and barrier |
|---|---|---|---|---|---|
| 1. Target/discovery: review the effective rules in this cwd | NO_CHANGE | Global file, overrides, config and supplied instructions | A correct base file can be ignored by an override or different home. Inspection found no such override/home setting. Supplied content could still mask loader failure. | Global/working-dir AGENTS and overrides checked; selected config fields inspected; git root probe exit 128; current session chunk equals G. Target supported. No further G patch. | Fresh automatic discovery unverified. Need a newly launched host trace; supplied-context provenance cannot prove it, and no independent agent run is authorized. |
| 2. Size/truncation: important rules enter the present instruction context | NO_CHANGE | Loader cap and file size | Being below the cap can coexist with irrelevant detail. | Actual 6,935-byte body; no configured project_doc_max_bytes; original supplied chunk complete. No present truncation defect supported. Placement handled separately. | Different combined chains could truncate elsewhere. No other active project chain exists here; other projects require their own trace. |
| 3. Personal versus project scope: keep cross-project preferences global and project commands local | NO_CHANGE | G personal working rules; README/package ownership | Requiring npm tests globally would harm this instruction-only package. G does not prescribe a project stack. | Whole G, README, INSTALL, tree and no Git/application pipeline inspected. Retain personal gates; do not invent build/lint/CI commands. | Applicability in other repositories unverified; their actual files/workflows are needed. No particular second repository is selected for this test. |
| 4. Goals and real examples: establish outcome and measurable acceptance before dependent work | NO_CHANGE | G §§1–2, §6; current explicit request | An invented success sample presented as full-scale completion violates G. Merely listing an acceptance criterion does not demonstrate achieving it. | Actual request, G, canonical requirements and historical records inspected. This run records dry-run acceptance and uses real current files. No further G patch. | Reliable extraction in other task domains needs representative runs, absent from inspected editor histories. New delegated runs not authorized. |
| 5. Context placement: detailed procedures load only when relevant, with obligations preserved | CHANGE | G §§3–4 currently permanent; proposed router | Translation complies with G while carrying all detail. Proposed code-review/reuse task could miss a narrow research-only trigger; existing proposed router explicitly includes those categories. | Verbatim block comparison, byte counts, complete patch and static trigger review. Supported MOVE repair; all 20 rules retained once. | Reading before action and runtime trigger reliability unverified. Real reference absent; adoption barred. A simulated rule list cannot prove live loading. |
| 6. Proportional reading/research: small settled fixes reuse relevant prior work | NO_CHANGE | G §6, G §5 approval reuse, H relevance rules | Repeating an already valid full research program for a typo has no applicability justification under §6. Ambiguous relevance could still lead to poor agent judgment. | Actual wording, requirements U8/U11, task scope and current-source recommendations inspected. Preserve exemptions; no evidence justifies weakening research gates. No further G patch. | Frequency/quality of relevance judgments unmeasured. Need real small-fix traces; available histories concern this audit only. |
| 7. Research/feasibility: select after evidenced critical paths, report failures | NO_CHANGE | G §3 and sequencing in §§1/6 | Select a familiar framework, then justify it: explicit violation. A correct ordered report could still contain bad scientific judgment. | All five original research rules and canonical U2–U4 inspected; moved block exact; weakened-clause negative rejected. No further G patch. | Process adherence and experiment quality not proven by text. No application experiment or independent agent study is authorized in this instruction audit. |
| 8. Architecture/reuse: preserve approvals and demonstrated custom gaps | NO_CHANGE | G §§4–5 and canonical U5–U9 | Rename an unauthorized change as thin adaptation: expressly excluded by the original fork/copy/patch distinction and architecture gate. | All four architecture rules retained exactly; architecture-approval removal rejected; router includes architecture review/change, custom code and contract reuse. No further G patch. | Enforcement in real implementation requires actual change/approval traces; none of those application tasks is part of this test. |
| 9. Consequential decisions: ask only unresolved user choices and reuse answers | NO_CHANGE | G §2/§5; installed grilling | Ask the user for a file path that tools can discover: violates fact-finding procedure. Re-ask the settled placement choice: violates approval reuse. | Grilling read and structurally validated; actual prior explanation/user message inspected. Choice confirmed; no reopened interview or extra G rule. | Classification reliability across future decisions unverified. Available prior trace demonstrates this placement decision only; new agent interviews not authorized. |
| 10. Approval boundaries: explicit scope is respected, routine work continues | NO_CHANGE | G §§2/5/6; H authorization rules | Stop routine approved retesting for a second approval, or use placement approval to apply the patch: each violates explicit boundaries. | Canonical generation/adoption policy, live hash, prior approval object and current no-edit request checked. Gates retained; active file unchanged. No further G patch. | Future false stops/unauthorized actions need real scenario traces. This audit proves current file preservation, not general permission judgment. |
| 11. Persistence: complete agreed authorized workflow and isolate blocked work | NO_CHANGE | G real/full-scale acceptance and dependent-only pause; H completion; E ledger closure | An agent could resolve one gap and call an audit done under the older editor's loose stopping rule. The historical trace actually shows this failure; present E explicitly forbids it. | Actual 03:54 result and later user corrections/readback inspected; current E Steps 4/7/Completion reviewed. Historical failure supported; current task-specific repair already present. No duplicate G repair. | New E does not erase the historical failure or prove future adherence. This run exercises its ledger; independent recurrence tests need separate run authority. |
| 12. Testing proportionality: necessary checks with normal/boundary/negative coverage | NO_CHANGE | G §§5–6 and H no redundant tests | Run unrelated tests after relevant checks already passed without new concern: H excludes this. Global rules in isolation could be interpreted too broadly; §6 supplies risk scaling. | Starter evals, real prior validation artifacts, current validator wrapper, scoped new integrity negatives and patch check inspected/executed. No further G patch in this effective host. | No representative app suite or standalone-host portability claim. Starter bullet cases lack captured agent runs; they are coverage intentions, not runtime tests. |
| 13. Evidence honesty: distinguish source, static checks, execution, adoption and acceptance | NO_CHANGE | G §§2/3/5/6; E scoped validation | Report PASS for the patch then imply every dimension works. Historical result/discussion shows this interpretive problem. Current E explicitly restricts PASS scope. | Prior report, actual user challenge and current contract checked; present ledger separates evidence states. No new global duplication; maintain explicit unverified states. | Honest future reporting remains unverified. No grader/model run can replace user acceptance; independent repeated reporting trials are not authorized. |
| 14. User/skill hierarchy: user no-edit scope prevails over workflow defaults | NO_CHANGE | H explicit user precedence and disclosure; G wrapper/scope requirement | A skill asks for persistence contrary to DO NOT modify AGENTS.md. Following both effective H and user request excludes the edit. | Host instructions, editor/grilling entrypoints, current request and unchanged hash inspected. Supported in this host. No further G patch. | Standalone clients with different higher-level instructions need their own instruction-chain audit; none is in this session. |
| 15. Maintenance/enforcement: canonical facts, distinct adoption, no false guarantee from prose | NO_CHANGE | G §6; canonical generation/requirements/state; host filesystem controls | Approve placement and silently mark runtime effectiveness accepted; violates separate approval objects. A well-written prohibition can still lack hard enforcement infrastructure. | Canonical generation procedure and selected current-state facts inspected; active hash agrees; U12 enforcement capability remains undeployed/pending in records. No claim of hooks/monitor enforcement. No G wording repair supplies that mechanism. | Architecture/approval enforcement and future reference drift need approved infrastructure or longitudinal traces. Deploying either is outside this audit; do not install it to create a pass. |
| 16. Skill integration: invocation and contract use are distinguishable from installation | NO_CHANGE | E explicit contract link; source folder; host skill catalog; INSTALL | A user follows legacy .codex/skills instructions and expects current .agents discovery. The documentation differs; compatibility on 0.159.2 is not established. | Visible source found/read, installed catalog and standard dirs inspected, actual source validation exit 0, current docs and historical changelog compared. Contract link is repaired; install documentation remains a separate package gap. No G patch for package installation. | Legacy-path/new-session compatibility needs an installation/discovery trial. Installation is outside this no-adoption test; no automatic discovery claim. |

All dimensions received concrete counterexample analysis and available evidence investigation. Structural support is not relabeled as behavioral PASS. No dimension is closed merely because another repair passed.

## Proposed Change

- Target: `/Users/xuebai/.codex/AGENTS.md` plus proposed `/Users/xuebai/.codex/references/research-and-architecture.md`.
- Current state: all 20 rules permanently loaded globally.
- Proposed state: retain the 11 original core rules and one mandatory router globally; move the nine rules in Sections 3–4, with their headings, verbatim into one reference.
- Rationale: implement the confirmed placement preference without paraphrasing requirements or altering approval authority. The reference must be included; a router alone would introduce a missing dependency.
- Minimal complete patch: [two-file MOVE patch, unapplied](/Users/xuebai/Downloads/agent-learning-harness-v0.1-visible/feedback/records/agents-md-editor-2026-10-06-proposed-move.patch).

Global body: 6,935 → 4,465 bytes, 2,470 fewer bytes. Relevant tasks load 7,583 body bytes across both files, 648 more than before, excluding tool/output overhead. Neither value is a token, fee, latency or adherence measurement. This already-started chat still carries the full supplied rules.

## Validation

| Check | Result, checked object and evidence | Verification scope |
|---|---|---|
| Standard alignment | PASS: complete proposed two-file layout versus S2–S4 and verified placement choice | Source-backed static adaptation; not overall compliance |
| Behavioral preservation | PASS: all 20 original clauses appear exactly once; nine moved clauses and source block are byte-identical | Static obligation preservation only; conditional-reading equivalence unverified |
| Conflict check | PASS: proposed router grants no new approval, keeps §§5–6 exceptions, includes research/selection/review/reuse, and specifies missing-reference dependent pause | Static effective-system review; future hosts and reference drift unverified |
| Regression check | PASS: missing/duplicate/weakened clauses rejected, temporary-baseline `git apply --check` exit 0, target hash unchanged, active reference absent | Deterministic integrity, applicability and file-preservation checks; no independent agent scenario suite |

Executed `codex-skill-validate skills/agents-md-editor` and `codex-skill-validate /Users/xuebai/.codex/skills/grilling`: both exit 0, `Skill is valid!`. The wrapper was read and uses the dedicated validator Python environment. This verifies structure, not skill adherence. `codex --version` and `codex exec --help` exit 0 with a sandbox PATH-alias warning; they do not prove model execution. `git rev-parse --show-toplevel` exit 128 establishes that this directory has no Git root; it is not a patch failure.

The first in-memory verifier exited 1 because it incorrectly normalized the source block's trailing blank line. Correct exact-block comparison exited 0. Neither attempt modified the target. The successful script checked a temporary original baseline using git apply --check; it never applied the patch. The baseline remained identical and no temporary reference was created. Those missing/duplicate/weakened-clause negatives test the integrity verifier, not the agent's behavior.

Target SHA-256 before/after: `a1acc7690963c37f21c908421975c8b42b5a668acf5fa8a45777c4a2dfee1e42`.

[Machine-readable validation](/Users/xuebai/Downloads/agent-learning-harness-v0.1-visible/feedback/records/agents-md-editor-2026-10-06-ledger-validation.json).

## Evidence

The official sources in Current Standard; current G and safely selected configuration/discovery facts; current user/host instructions; local editor and its output contract; installed grilling and validator wrapper; README/INSTALL/router/starter evals; canonical governance AGENTS_REQUIREMENTS.md, AGENTS_GENERATION.md and review-state.json; existing complete MOVE patch; executed commands and validation JSON.

Historical trace evidence inspected directly:

- `/Users/xuebai/.codex/sessions/2026/10/06/rollout-2026-10-06T10-51-28-01a10f1f-8f1e-7de2-803e-b9e1c426c773.jsonl`: actual placement explanation and user decision.
- `/Users/xuebai/.codex/sessions/2026/10/06/rollout-2026-10-06T11-50-02-01a10f55-2a6a-72a0-a987-b5cf0665eecc.jsonl`: actual earlier audit result, user objections to incomplete exploration, and authorized editor closure update.
- Current session instruction chunk: exact textual match with global rules; provenance does not prove automatic file discovery.

Memory provided only the established standard/requirements separation and a pointer to canonical governance records; the relevant present state and placement decision were independently checked. No memory was written.

Rescan: the placement defect is addressed in the proposal; live files still retain it. The corrected output-contract linkage is current, rather than an outstanding gap. Installation documentation remains a separate surfaced issue. Historical premature closure is actual adverse evidence and cannot be reported as a behavioral pass. No additional global-file repair is justified by the inspected evidence. Runtime loading, reliability, cross-client portability, enforcement, drift and efficiency remain explicitly unverified for the substantiated reasons above. User adoption and acceptance remain separate.

## Authorized skill update: informative final repair decisions

The user rejected narrative-only repair conclusions, required CHANGE / NO_CHANGE / NEEDS_DECISION / BLOCKED for every reviewed dimension, and then explicitly requested updating the skill. This authorizes the focused skill/contract update; it does not authorize applying the AGENTS.md proposal.

Updated the editor's Step 7 and Completion requirements and its existing output contract. The final response must lead with whether AGENTS.md needs updating and include every reviewed dimension in a decision table with target, explicit status, action or next step, and evidence-backed reason. Linked ledgers cannot replace the final table. Other-file repairs, proposed versus applied changes, audit completion and behavioral verification remain distinct. Decision definitions prevent unsupported NO_CHANGE and distinguish a blocker affecting the repair from unverified runtime behavior that does not affect the repair choice.

Added five reporting evaluation cases to the existing starter eval document: mixed repair targets; known repair alongside an unresolved decision; unavailable evidence affecting the repair; runtime uncertainty with independently supported static repair; and a negative narrative-only/linked-only summary. These are specified evaluation cases, not executed model trials.

Validation: `codex-skill-validate skills/agents-md-editor` exited 0 (`Skill is valid!`). Readback/static review checked consistency between entrypoint, final summary, ledger, status definitions and PATCH/AUDIT scope. Structural validation and static review do not prove future model adherence. No independent model runs were launched for this narrow instruction edit. Global AGENTS.md still has SHA-256 `a1acc7690963c37f21c908421975c8b42b5a668acf5fa8a45777c4a2dfee1e42`.
