# AGENTS.md Editor — AUDIT 评估记录

## Separate hypothetical-line PATCH test — 2026-10-06

This test evaluates the user-supplied assumed line `you can do what ever it takes to get things done`. It is not present in the actual global AGENTS.md and does not supersede the actual-file AUDIT result below. The user explicitly prohibited AGENTS.md modification and requested the editor output contract, with a patch only for CHANGE.

Current decision: NEEDS_DECISION. Current Standard discovery covered instruction loading/hierarchy, explicit constraints and completion criteria, practical instruction wording, autonomy and follow-through, skill priority, and enforced sandbox/approval boundaries. Follow-up official searches and reads refined these dimensions without adding another material standard for this specific line. Coverage is limited to this PATCH test, not an exhaustive system audit.

Material sources fetched this run:
- https://learn.chatgpt.com/docs/agent-configuration/agents-md — REQUIRED loading and layering mechanism.
- https://learn.chatgpt.com/docs/agent-approvals-security — REQUIRED execution boundaries; prose cannot change configured enforcement.
- https://learn.chatgpt.com/guides/best-practices — RECOMMENDED practical, accurate instructions, constraints, completion and verification.
- https://developers.openai.com/api/docs/guides/latest-model — RECOMMENDED persistent completion of authorized work, appropriate clarification and review of conflicting instructions; model advice is a starting point requiring workload evaluation.
- https://developers.openai.com/api/docs/guides/text — REQUIRED developer/user instruction priority mechanism.

Gap: the assumed broad permission does not specify whether it means persistence under existing gates or a deliberate change to the user's scope/architecture approval policy. The applicable global rules already require scope/architecture approval and exempt routine execution from repeated approval. Host instructions already require persistence. Thus missing permission enforcement is not established, and adding another blanket approval rule is not warranted. Grammar alone is not a meaningful gap. The intended additional behavioral difference remains unconfirmed.

Candidate Learning: NONE; supplied material is an instruction to assess, not a separately confirmed feedback learning. Apparent persistence intent is provisional.

Grilling Round 1 frontier: Q1 asks whether the line should mean persistent completion within existing approval gates or change those gates. Recommend preserving the gates: it preserves follow-through without silently changing approved governance. Detailed permission choices depend on this answer and belong to a later round. Shared understanding must be confirmed before adaptation. No patch is proposed or applied.

Validation of the assumed instruction: Standard alignment FAIL (meaning remains ambiguous); Behavioral preservation FAIL (intended policy cannot yet be validated); Conflict check FAIL (broad permission versus specific approval gates remains ambiguous); Regression check PASS for file preservation only, with runtime behavior unverified. Adaptation and final semantic validation are pending, and the Gap Frontier remains open.

Actual checks: `codex-skill-validate skills/agents-md-editor` returned exit 0, `Skill is valid!` (structure only). Read-only SHA-256 assertion returned exit 0, confirming actual global AGENTS.md unchanged at `a1acc7690963c37f21c908421975c8b42b5a668acf5fa8a45777c4a2dfee1e42`; cwd AGENTS.md remains absent. Normal/boundary/negative static review distinguished authorized persistence, approval-governed scope changes, and the explicit no-edit prohibition. No agent behavior experiment or adoption occurred.

## Current result — 2026-10-06, Asia/Shanghai

**Decision: NO_CHANGE.** This assessment supersedes the earlier CHANGE recommendation below. AGENTS.md was not modified. Historical candidate patches are retained as historical evidence, not as the current proposal or adopted policy.

### Scope and acceptance

The user explicitly authorized an AUDIT using Current Standard → Gap → resolve consequential uncertainty with grilling when necessary → Adapt → Validate, prohibited modifying AGENTS.md, and requested the editor output contract. Success means a source-backed decision, preservation of confirmed user requirements, both frontiers reviewed to saturation, static validation, and a patch only for CHANGE. This is a single assessment of the instruction system applicable to this directory, not a guarantee about all repositories, automatic skill discovery, future compliance, or model behavior.

Actual target: `/Users/xuebai/.codex/AGENTS.md`. CODEX_HOME is unset; no project_doc configuration fields were found by the focused configuration check. No applicable AGENTS.override.md or project AGENTS.md was found. `git rev-parse --show-toplevel` returned exit 128: no Git repository. The global file matches the rules supplied in the current conversation. Host instructions and the explicit no-edit request remain applicable. The router snippet is a proposed snippet, not a loaded AGENTS.md file.

### Current Standard

REQUIRED identifies documented discovery, structure, or execution mechanisms; it does not mean every mechanism must be copied into AGENTS.md. RECOMMENDED identifies official guidance. INFERRED identifies this audit's interpretation. Model-specific advice is a conditional starting point, not evidence of measured behavior on this task.

| ID | Guidance | Source | Strength | Applicability and relationship |
|---|---|---|---|---|
| C1 | Codex home guidance, overrides, project discovery, root-to-directory merge order, and the default 32 KiB limit determine which files apply. | [AGENTS.md](https://learn.chatgpt.com/docs/agent-configuration/agents-md) | REQUIRED | Establishes the target before content assessment. No Git root means the project check is cwd only. The target is 6,935 bytes. |
| C2 | Verify discovered instructions in a fresh run after applying changes. | [AGENTS.md](https://learn.chatgpt.com/docs/agent-configuration/agents-md) | RECOMMENDED | Complements C1; no adoption or fresh-run claim is made in this no-edit audit. |
| C3 | Put personal defaults globally and project conventions near the relevant code; use skills for rich reusable procedures. | [Customization](https://learn.chatgpt.com/docs/customization/overview) | RECOMMENDED | Distinguishes global policy from project commands and skill installation. |
| C4 | Keep guidance practical and accurate; add rules for demonstrated recurring friction and use supporting resources when the main file becomes too large. | [Best practices](https://learn.chatgpt.com/guides/best-practices) | RECOMMENDED | Supports avoiding duplicate rules; byte-limit compliance alone does not prove instruction quality. |
| C5 | Reassess instruction necessity, read context according to the task, and review overly prescriptive boundaries and premature stopping points. | [Rethinking skills and prompts, 2026-09-11](https://developers.openai.com/blog/rethinking-skills-and-prompts-for-gpt-6-astra) | RECOMMENDED | Conditional model advice; complements C4 without cancelling confirmed user gates. |
| C6 | Define the outcome, relevant context, output, boundaries, and verification; plan when approach or complexity warrants it. | [Prompting](https://learn.chatgpt.com/docs/prompting), [Best practices](https://learn.chatgpt.com/guides/best-practices) | RECOMMENDED | Existing goal, scope, architecture, and acceptance clauses provide these requirements. |
| C7 | Continue authorized work, avoid unnecessary approval requests, make explicit user instructions take precedence over skill guidelines, and identify the exact skill instruction responsible for a pause. | [Using GPT-6: prompting](https://developers.openai.com/api/docs/guides/latest-model) | RECOMMENDED | User-requested approval boundaries remain intentional; host guidance already covers skill priority and pause disclosure. |
| C8 | Use relevant, meaningful checks; broaden or repeat them when changes, failures, or unresolved concerns justify it. Evaluate model-related advice on the chosen workload. | [Using GPT-6: prompting](https://developers.openai.com/api/docs/guides/latest-model) | RECOMMENDED | Relates C5 to the existing risk-scaling and agreed-criteria rules. No model benchmark was performed. |
| C9 | Skills require name/description metadata, load fuller instructions when selected, and currently use `.agents/skills` for repository discovery. | [Build skills](https://learn.chatgpt.com/docs/build-skills) | REQUIRED | Installation/discovery mechanisms are distinct from this explicit reading of visible source. |
| C10 | Use focused triggers, explicit inputs/outputs/decision boundaries, referenced supporting files, and representative positive and negative requests. | [Build skills — Plugins](https://developers.openai.com/plugins/build/skills) | RECOMMENDED | Applied to the editor process and output contract; does not authorize rewriting either skill. |
| C11 | Evaluate actual agent traces and artifacts, including negative activation controls; package validation is insufficient to prove behavior. | [Testing skills with evals, 2026-01-22](https://developers.openai.com/blog/eval-skills) | RECOMMENDED | Complements C8/C10 and preserves the distinction between static and runtime evidence. |
| C12 | Sandboxing and approval policies govern real tool execution. | [Agent approvals & security](https://learn.chatgpt.com/docs/agent-approvals-security) | REQUIRED | Written workflow approval does not replace execution controls. |
| C13 | Delegate through explicit user/project/skill triggers; bound assignments and account for extra tokens and coordination. | [Subagents](https://learn.chatgpt.com/docs/agent-configuration/subagents) | RECOMMENDED | No unresolved grilling question required delegated fact-finding here; no agents were spawned. |
| C14 | A best-practice suggestion is not automatically a missing global rule if its intent is already satisfied by effective instructions. | C3–C8 and the editor's minimal-change requirement | INFERRED | Governs the disposition of the earlier scope candidate. |

### Standard Frontier and rescans

Discovery covered AGENTS loading and hierarchy, global/project placement, prompting and scope, context routing, current model instruction sensitivity/autonomy/testing, skill discovery and workflow boundaries, execution controls, eval evidence, and subagent triggers. Follow-up searches covered instruction conflicts, minimal changes/correctness, maintenance, and current discovery guidance. The subagent page added the last applicable adjacent dimension, C13. Later checks of negative eval controls and testing guidance refined existing dimensions without changing the evaluation.

Official HTML bodies were actually opened and their relevant sections read; unsuccessful Markdown endpoints were replaced by HTML, not treated as evidence. The current Build skills reference governs discovery recommendations; the January eval tutorial's older `.codex/skills` example is not used to supersede it. API/SDK implementation, model migration, GitHub review setup, Goals, automation installation, and archived ExecPlan recipes do not establish requirements for this global-file no-edit audit.

Final Standard rescan: preserving the existing rules creates no new component, dependency, contract, permission policy, or applicable source dimension. Instruction rescan: reviewed all 20 rules and the no-edit/Apply interaction; no new material gap was found. Coverage saturation is limited to the current authoritative sources and available evidence, not absolute completeness.

### Gap

| Item | Finding and disposition |
|---|---|
| Earlier scope candidate | **NO_CHANGE.** Source line 12 requires recording scope, line 10 defines exclusions and expansion gaps, and line 31 requires evidence, minimal changes, and approval before scope changes. The earlier proposed default-scope/necessary-expansion rule does not demonstrate a materially missing behavior. No current candidate learning or failure evidence supplies an additional decision boundary. |
| Global instruction length and procedure | **NO_CHANGE.** The file contains durable personal governance requirements. Line 38 scales research/documentation and allows reuse for small fixes; line 10 limits inspection to relevant context. Shortening or moving these confirmed requirements merely to match an optional model recommendation could alter their loading contract. No such migration is needed for the current assessment. |
| Approvals, autonomy, and grilling | **NO_CHANGE.** Line 11 limits grilling to consequential unresolved decisions; line 32 exempts authorized routine execution and retesting; line 38 preserves settled decisions. The current request directly authorizes this audit. No new permission policy or interview decision is inferred. |
| Skill priority and Apply conflict | **RESOLVED.** The explicit no-edit request overrides the editor Apply step. Host instructions already express user priority and precise pause attribution. No AGENTS clause is needed to duplicate them. |
| Verification and completion | **NO_CHANGE.** Lines 18, 19, and 33 already require defined criteria, normal/boundary/negative cases, actual evidence, and separation from user acceptance. Starter eval text does not prove runtime performance; the current verdict stays static. |
| Installation guidance | **NO_CHANGE for AGENTS.md.** README/INSTALL suggest `.codex/skills`; current local-skill documentation uses `.agents/skills`. This is a separate installation-document issue. Manual source loading worked; automatic discovery and older-path compatibility were not tested. It supplies no reason to patch global AGENTS.md. |
| Project commands, routing, review, ongoing maintenance | **NO_CHANGE.** This is a visible skill source package without application or Git/PR workflow. No project-specific command, router adoption, scheduled check, or universal ongoing guarantee is required by the authorized global audit. |

### Candidate Learning

NONE. The current request supplies no feedback-learning candidate. Historical audit suggestions were examined as unadopted proposals, not promoted to new user requirements.

### Grilling and Adapt

The installed grilling SKILL.md was read and its availability announced. Its interview rounds were not entered: current sources, actual instruction text, and explicit user constraints resolve the present evaluation. There is no consequential repository-specific policy choice left to decide. This is not a claim that a grilling interview occurred.

Adaptation means applying each standard at its actual scope: preserve confirmed governance, respect effective host instructions, and avoid adding already-covered behavior. The design-tree frontier contains no unresolved decision; no new confirmation gate is introduced.

### Decision

**NO_CHANGE.** No unresolved material item remains in this audit's Gap Frontier. The existing file does not need the earlier additional scope rule. The prior recommendation is superseded on the evidence above; no existing approval or adopted rule was changed.

### Proposed Change

NONE. No patch is emitted or applied for this decision.

### Validation

| Check | Result | Evidence and limit |
|---|---|---|
| Standard alignment | PASS | C1–C14 reviewed at the relevant scope; conditional recommendations are not misrepresented as mandatory text. |
| Behavioral preservation | PASS | All 20 rules remain byte-for-byte unchanged. |
| Conflict check | PASS | No directory override found; explicit no-edit request resolves Apply; no unapproved workflow or skill priority change. |
| Regression check | PASS | Static review and identity check only; no behavioral improvement or runtime generality is claimed. |

Static normal/boundary/negative reviews: an authorized audit proceeds under the current request; routine verification does not reopen settled approvals; scope expansion still requires evidence and approval; unnecessary adjacent refactoring remains outside confirmed scope; unavailable evidence blocks only dependent work; a candidate is not adoption; Apply cannot override no-edit; starter evals and successful validation cannot establish behavioral compliance. These are semantic reviews of the actual clauses, not executed synthetic agent scenarios.

Actual commands this run:

- `git rev-parse --show-toplevel`: exit 128; no project Git root.
- `command -v codex-skill-validate`: exit 0; `/Users/xuebai/.local/bin/codex-skill-validate`.
- Read the validator wrapper: it selects the dedicated virtual environment's Python and official quick_validate.py.
- `codex-skill-validate skills/agents-md-editor`: exit 0; `Skill is valid!`. Structure only.
- Read-only Python identity check: exit 0; SHA-256 matches the first read, 6,935 bytes, 20 rules retained, zero AGENTS writes.

Protected SHA-256: `a1acc7690963c37f21c908421975c8b42b5a668acf5fa8a45777c4a2dfee1e42`.

No fresh Codex reload, automatic skill discovery test, runtime scenario suite, cross-project test, or future compliance guarantee is included. User acceptance remains a separate state.

### Evidence

The linked official sources above; current `/Users/xuebai/.codex/AGENTS.md` lines 10–12, 18–19, 31–33, 37–39; the editor SKILL.md and output contract; installed grilling SKILL.md; README, INSTALL, router snippet, feedback-learning boundaries, and starter eval definitions. The existing audit record was treated as history. A lightweight memory lookup supplied governance context only; current target, requirements, and official guidance were verified live.

Only this existing project audit record was updated. AGENTS.md, skills, installation guidance, configuration, and persistent memory were not changed.

## Historical assessments — superseded by the current result above

日期：2026-10-06（Asia/Shanghai）。状态：CHANGE 候选；未应用；用户验收待定。

本次复核的当前结果见文末“本次重新取证与验证”。前文保留既有审核记录；前文“未执行验证器”等描述是此前状态，本次已实际执行结构验证。AGENTS.md 仍未修改。

本轮从现有文件和当前官方来源重新取证，不读取持久记忆，不使用上一轮结论或答案作为依据。没有删除持久记忆或重置聊天历史。

## Scope

目标是当前工作目录适用的指令系统，主要文件为 [/Users/xuebai/.codex/AGENTS.md](/Users/xuebai/.codex/AGENTS.md)。当前仓库、父目录与全局目录的 AGENTS/override 已检查，只有该全局文件存在；无 Git 根。环境 CODEX_HOME 未设置，配置查询未发现 project_doc 字段，model 为 gpt-6.1-sol。本文不声称已审核其他项目的 AGENTS.md。

仓库为两项技能的可见源码包，没有应用代码或运行入口。已读 README、INSTALL、TREE、router snippet、两项 SKILL.md、两个 output-contract 和两项 starter eval 文本。router snippet 尚不是生效 AGENTS。

用户明确要求这次只评估，禁止修改 AGENTS.md；因此技能 Apply 不执行。除本文审核记录，不修改指令、配置、技能或安装文档。

## Current Standard

### 来源与强度

REQUIRED 表示已记录的加载/结构/权限机制，不表示 AGENTS.md 必须逐字包含每项。RECOMMENDED 是官方建议，按适用性与明确用户要求判断；INFERRED 是本次从官方说明推导的边界，单独标注。

源码包和技能是任务上下文，不作为官方标准。旧 cookbook 示例、Astra 表现、示例技术栈、API 参数与安装旧路径不自动升级为全局要求。

<a id="source-a"></a>
- **A** — [Custom instructions with AGENTS.md](https://learn.chatgpt.com/docs/agent-configuration/agents-md)。加载、覆盖、大小、验证。

<a id="source-b"></a>
- **B** — [Build skills](https://learn.chatgpt.com/docs/build-skills)。技能结构、发现、调用、元数据。

<a id="source-c"></a>
- **C** — [Prompting](https://learn.chatgpt.com/docs/prompting)。目标、上下文、边界、验证与任务例子。

<a id="source-d"></a>
- **D** — [Rethinking skills and prompts for GPT-6 Astra](https://developers.openai.com/blog/rethinking-skills-and-prompts-for-gpt-6-astra)。2026-09-11；模型相关的上下文、流程、维护建议。

<a id="source-e"></a>
- **E** — [Using GPT-6 — Prompting best practices](https://developers.openai.com/api/docs/guides/latest-model)。通用起点；须在选定模型与工作负载上评估。

<a id="source-f"></a>
- **F** — [Build skills — Plugins](https://developers.openai.com/plugins/build/skills)。工作流边界、用户优先级、资源与验证。

<a id="source-g"></a>
- **G** — [Best practices](https://learn.chatgpt.com/guides/best-practices)。持久指令内容、规划、验证、配置与维护。

<a id="source-h"></a>
- **H** — [Customization](https://learn.chatgpt.com/docs/customization/overview)。全局/项目分工、技能与工具、反馈维护。

<a id="source-i"></a>
- **I** — [Agent approvals & security](https://learn.chatgpt.com/docs/agent-approvals-security)。权限与沙箱机制，区别于文字审批规则。

<a id="source-j"></a>
- **J** — [Testing Agent Skills Systematically with Evals](https://developers.openai.com/blog/eval-skills)。2026-01-22；实际轨迹、负例、语义评估；旧安装路径不作为当前标准。

### Standard Frontier 的扩展与停止依据

1. 从 AGENTS、Codex prompting、skills 三个维度搜官方资料；阅读 A–F 的有关正文。
2. 技能及模型页面暴露相邻维度：技能优先级、流程、模型适用性、验证。补查并阅读 G–J。
3. A、B、C、D、F、G、H 的有关正文及 J 的评估方法已检查；E 仅把 Prompting best practices 作为本任务标准，API 迁移/价格参数不适用；I 核对权限机制，不进行环境配置审计。
4. 后续搜索覆盖 instruction conflicts、scope、testing、maintenance；返回已检查的 AGENTS、模型、Customization、Best practices，以及 GitLab/SDK 专门场景。后者与本轮无 Git/无 SDK 的环境无关。
5. 已记录新增维度、适用层级及模型条件；相邻发现没有再加入能改变当前 AGENTS 内容评估的新适用项。由此达到本轮覆盖饱和，不是找到所有可能文档的绝对保证。

检索主题：
- Codex AGENTS.md best practices
- Codex prompting guide instructions scope autonomy
- Codex skills instruction best practices
- AGENTS.md concise testing / priority skills user / skill evals process outcome negative cases
- AGENTS.md instruction conflicts scope testing / current guidance instruction following maintenance

部分官方 markdown URL 被 web 工具拒绝为 unsupported content-type；已改用同源 HTML 正文，没有以失败链接或搜索摘要代替读取。

### 逐项标准清单

下表包含适用、条件适用及排除项，完整列出本轮 48 个审查单位。它不是 48 条需要新增的规则；数量也不构成完备性证明。

| ID | Principle | Source | Strength | Applicability | Relationship | Disposition | 逐项依据 |
|---|---|---|---|---|---|---|---|
| S01 | 全局文件发现及 override 优先 | [A](#source-a) | REQUIRED | 当前目标 | 加载机制；独立于内容建议 | NO_CHANGE | 默认 home；无全局 override；目标为 ~/.codex/AGENTS.md。 |
| S02 | 项目路径发现；无项目根时仅查 cwd | [A](#source-a) | REQUIRED | 当前工作目录 | 与 01 组成有效指令链 | NO_CHANGE | 此目录无 .git、无 AGENTS/override；不把 router snippet 当作生效指令。 |
| S03 | 靠近工作目录的指令覆盖较远规则 | [A](#source-a) | REQUIRED | 存在嵌套规则时 | 补充 01–02 | NO_CHANGE | 本轮不存在项目/嵌套覆盖；未发现层级冲突。 |
| S04 | 非空文件及累计字节上限 | [A](#source-a) | REQUIRED | 当前加载 | 不同于是否简洁的 12 | NO_CHANGE | 目标 6935 bytes；无 project_doc_max_bytes 配置匹配；低于文档默认 32768。 |
| S05 | 更改后在新运行中核对有效指令 | [A](#source-a) | RECOMMENDED | 实际应用补丁后 | 加载验证不等于语义验证 | NO_CHANGE | 本轮禁止应用；未启动新 Codex 会话，也不声称重载已验证。 |
| S06 | 个人默认与项目规则分层 | [H](#source-h) | RECOMMENDED | 全局文件 | 界定 07–10 的适用层级 | NO_CHANGE | 当前文件主要是个人治理偏好；项目命令不应硬编码进全局。 |
| S07 | 项目布局与重要目录 | [G](#source-g) | RECOMMENDED | 项目级指令 | 06 的项目内容分支 | NO_CHANGE | README/TREE 已给目录；当前目标是全局规则，无需重复写入。 |
| S08 | 项目运行方式 | [G](#source-g) | RECOMMENDED | 有可运行项目时 | 与 07、09 相关 | NO_CHANGE | 仓库是技能源码包，没有应用运行入口；不编造启动命令。 |
| S09 | 构建、测试、lint 命令 | [G](#source-g) | RECOMMENDED | 项目级且有实际工具时 | 区别于 27 的测试策略 | NO_CHANGE | 包仅有 starter eval 文本；全局指定技能验证器，不新增虚构命令。 |
| S10 | 工程约定和 PR/review 预期 | [G](#source-g) | RECOMMENDED | 项目与审查工作流 | 补充 06、45 | NO_CHANGE | 本轮不是 PR；未发现要求覆盖全局治理的项目约定。 |
| S11 | 约束、完成条件和验证标准 | [G](#source-g) | RECOMMENDED | 当前文件 | 由 18、20、29 细化 | NO_CHANGE | §1、§2、§5 已定义目标、验收和实际证据。 |
| S12 | 规则具体、简洁，表达行为与例外 | [A](#source-a), [G](#source-g) | RECOMMENDED | 当前文件 | 不是 04 的大小合格即质量合格 | RESOLVED | 候选范围边界未明确；最小新增一条含正确性例外的规则。 |
| S13 | 用真实反复错误/反馈驱动新增规则 | [G](#source-g), [H](#source-h) | RECOMMENDED | 长期维护 | 与 15 区分维护触发 | NO_CHANGE | 本轮未取得额外反复错误证据；不据假设删除或增加其他治理要求。 |
| S14 | 将长的重复工作流放进按需资源 | [D](#source-d), [H](#source-h) | RECOMMENDED | 确有冗长/加载问题时 | 依赖 06、16；不是强制迁移 | NO_CHANGE | 20 条治理规则不证明上下文故障；整体迁移需新文件与调用契约，不是此次正确性依赖。 |
| S15 | 重新审视指令必要性与时效 | [D](#source-d), [H](#source-h) | RECOMMENDED | 当前审核；后续维护 | 不同于 41 的自动调度 | NO_CHANGE | 本轮即执行复审；文字不能保证未来永远最新，不擅自设定周期。 |
| S16 | 只读取与任务相关的上下文 | [C](#source-c), [D](#source-d) | RECOMMENDED | 当前文件 | 制约 14 与 17 的成本 | NO_CHANGE | §2 写 relevant；§6 按风险缩放，没有每次全仓阅读的规定。 |
| S17 | 复杂/模糊任务先规划 | [G](#source-g) | RECOMMENDED | 复杂任务 | 用户可指定更严格阶段 | NO_CHANGE | §1、§4 已要求设计先行；§6 允许小修复复用既有研究/设计。 |
| S18 | 明确目标、上下文、边界、输出和验收 | [C](#source-c), [G](#source-g) | RECOMMENDED | 当前文件 | 完成条件 11 的展开 | NO_CHANGE | §2、§4、§5 覆盖；不要求所有任务都新建完整规格文档。 |
| S19 | 按实际授权推进，避免不必要澄清 | [E](#source-e) | RECOMMENDED | 授权明确时 | 不取代用户明确审批门 | NO_CHANGE | §5 复用有效审批；§6 不重问已决事项。直接请求可构成该请求的明确授权。 |
| S20 | 持续完成授权工作，不停在首个候选 | [D](#source-d), [E](#source-e) | RECOMMENDED | 任务尚有必要工作时 | 受 11、19、21 限定 | NO_CHANGE | §5 要实际验证和验收；不把框架确认、架构批准或脚本成功混作完成。 |
| S21 | 安全、授权的常规执行不反复审批 | [D](#source-d), [E](#source-e) | RECOMMENDED | 有效授权内 | 区别于真实 scope 变更 | NO_CHANGE | §5 第二条已明确执行/重测无需重复审批或 grilling。 |
| S22 | 不因假设风险添加额外审批流程 | [E](#source-e) | RECOMMENDED | 新增建议时 | 与 19 相同授权前提 | NO_CHANGE | 不删除用户主动制定的既有审批；本轮也不新增权限流程。 |
| S23 | 明确用户任务指令优先于技能指导 | [E](#source-e), [F](#source-f) | RECOMMENDED | 技能参与任务时 | 与 03 的目录覆盖是不同优先级 | NO_CHANGE | 当前宿主已明确此优先级；本轮 no-edit 指令覆盖技能 Apply 步骤，不再复制一条。 |
| S24 | 技能引发停顿时指出文件与原指令 | [E](#source-e) | RECOMMENDED | 实际发生停顿时 | 提供 23 的可解释性 | NO_CHANGE | 当前宿主已要求；本轮无技能引发的新暂停，不虚构引用或审批。 |
| S25 | 按任务需要设定清楚的表达风格 | [E](#source-e) | RECOMMENDED | 输出质量 | 不同于行为约束 | NO_CHANGE | 当前宿主已给写作规则；此次输出契约优先，不进行全局风格改写。 |
| S26 | 按工作流指定代理分工边界 | [E](#source-e) | RECOMMENDED | 使用多代理时 | 不是每次都必须委派 | NO_CHANGE | 没有未决且须委派发现的事实；本轮不启动代理，不改变全局分工策略。 |
| S27 | 运行与改动相称、有意义的检查 | [E](#source-e), [G](#source-g) | RECOMMENDED | 验证工作 | 与 09 的具体命令不同 | NO_CHANGE | §5 agreed criteria、§6 风险缩放；不因 Astra 建议取消现有负例/证据要求。 |
| S28 | 已通过的检查只因新变更/失败/疑虑扩大重做 | [E](#source-e) | RECOMMENDED | 重复验证可能发生时 | 27 的停止条件 | NO_CHANGE | 没有条款要求无依据反复运行全部测试；routine retesting 无需重复审批。 |
| S29 | 评估前定义结果、过程和效率标准 | [J](#source-j) | RECOMMENDED | 本轮评估及技能演化 | 细化 11、18 | NO_CHANGE | 技能规定两类 Frontier、来源、验收；全局要求实验前定义准则。 |
| S30 | 用实际运行轨迹与产物支撑效果判断 | [J](#source-j) | RECOMMENDED | 声称运行有效性时 | 不同于 05、32 | NO_CHANGE | §3、§5 已区分文档/静态/实际运行；本轮只声称静态评估。 |
| S31 | 正例、负例、边界与错误触发 | [F](#source-f), [J](#source-j) | RECOMMENDED | 技能/行为验证 | 为 29–30 提供案例边界 | NO_CHANGE | §3、§5 已要求 normal/boundary/negative；starter eval 包含 NO_CHANGE 等负控制，但不是执行证据。 |
| S32 | 语义/定性正确性不能只靠计数和文件存在 | [J](#source-j) | RECOMMENDED | 评价结果时 | 补充 30 | NO_CHANGE | §5 明确次数、退出码或单例不能证明正确性与泛化。 |
| S33 | 技能聚焦目标，描述触发与不适用范围 | [B](#source-b), [F](#source-f) | RECOMMENDED | 被调用技能 | 与 26 的代理分工不同 | NO_CHANGE | editor 的 PATCH/AUDIT 及反馈技能的 admit/hold/reject 分工已明确。 |
| S34 | 选中技能后读全文，资源按需加载 | [B](#source-b), [H](#source-h) | REQUIRED | 本轮技能调用 | 加载机制；支持 16 | NO_CHANGE | 已重读 editor、输出契约及相关仓库文本，不凭技能名代替执行。 |
| S35 | 技能 front matter 有 name/description | [B](#source-b), [F](#source-f) | REQUIRED | 技能结构 | 不是语义或效果验证 | NO_CHANGE | 两个技能均有字段；未修改技能，未将结构正确声称为行为通过。 |
| S36 | 当前技能发现位置和同名技能不合并 | [B](#source-b) | REQUIRED | 自动发现/安装时 | 不同于 01 的 AGENTS 加载 | NO_CHANGE | 当前官方写 .agents/skills；本包安装文档写 .codex/skills。路径差异已记录，但手动读取本轮技能不依赖安装。 |
| S37 | 实际依赖存在并处理缺失/模糊结果 | [F](#source-f) | RECOMMENDED | 依赖被调用时 | 区别于技能元数据 35 | NO_CHANGE | grilling 在当前技能目录可用；editor 仅在实质未决决策时调用，不需要 MCP 元数据。 |
| S38 | 指令优先；确定性处理再用脚本 | [B](#source-b), [F](#source-f) | RECOMMENDED | 技能实现选择 | 服务于 33、16 | NO_CHANGE | 仓库两项技能为指令及 references；本轮不新建评测框架。 |
| S39 | 沙箱和权限策略控制实际可执行行为 | [I](#source-i) | REQUIRED | 工具执行 | 不能由 19 的文本授权绕过 | NO_CHANGE | 本轮不申请改写全局文件的权限；AGENTS 的审批门不是沙箱配置。 |
| S40 | 文本规则与基础设施执行分开 | [H](#source-h), [I](#source-i) | INFERRED | 宣称治理能力时 | 区分 39 与内容合规 | NO_CHANGE | §5 已禁止以脚本成功代替效果/用户验收；未声称此 AGENTS 强制运行时安全。 |
| S41 | 稳定后才安排自动维护/漂移检查 | [G](#source-g), [H](#source-h) | RECOMMENDED | 显式要求周期运行时 | 15 的可选实施方式 | NO_CHANGE | 此次仅 first test、评估当前文件；不创建自动化，也不声称持续合规。 |
| S42 | 同仓并行改动用隔离工作树 | [G](#source-g) | RECOMMENDED | 真实并发代码改动时 | 26 的环境保障 | NO_CHANGE | 当前无 Git/并行改动；本次不适用。 |
| S43 | 外部信息需要时再接工具/MCP | [G](#source-g), [H](#source-h) | RECOMMENDED | 现有工具不足时 | 区别于写入静态指令 | NO_CHANGE | 可用 web 已能取得官方资料；不安装新连接器或扩展权限。 |
| S44 | 模型建议须在选定模型/工作负载上评估 | [D](#source-d), [E](#source-e) | RECOMMENDED | 跨模型采用指导 | 限定 19–28 的外推 | NO_CHANGE | 配置为 gpt-6.1-sol；不把 Astra 的表现推断为 Sol 已验证效果。 |
| S45 | 复核 diff、回归及最终行为 | [G](#source-g) | RECOMMENDED | 变更候选 | 27、30 的交付检查 | NO_CHANGE | 本轮检查最小文本差异和保留性；无实际应用，无 PR 运行效果声明。 |
| S46 | GitHub review 规则贴近代码，格式检查交给 CI | [A](#source-a) | RECOMMENDED | GitHub 自动 review 场景 | 专门审查建议，不扩为全局强制 | NO_CHANGE | 当前无 GitHub repo/CI 审查需求；不在全局新增 Code Review Rules。 |
| S47 | 跨团队/可安装分发优先插件 | [B](#source-b), [H](#source-h) | RECOMMENDED | 技能分发任务 | 区别于 36 的本地发现 | NO_CHANGE | 本轮不发布或安装本包；不把分发建议变成全局依赖。 |
| S48 | 保留适用过程，自由度与治理按任务需要配置 | [C](#source-c), [D](#source-d) | RECOMMENDED | 是否改写个人工作流 | 统合 14、17、19；允许过程本身重要 | NO_CHANGE | 原规则明确把批准和证据作为工作要求；官方建议没有强制废除这些要求。 |

### 当前全部 20 条规则的反向检查

| 源行 | 现有行为 | 关联标准 | 结论 |
|---|---|---|---|
| [5](/Users/xuebai/.codex/AGENTS.md:5) | 最小充分架构、成本及维护 | S11,S18,S43 | 保留。尺寸少不等于完整正确，未增加框架。 |
| [6](/Users/xuebai/.codex/AGENTS.md:6) | 目标到验收的顺序 | S17,S20,S48 | 保留。§6 允许复用已有设计，避免把指导解释为每次重做全部阶段。 |
| [10](/Users/xuebai/.codex/AGENTS.md:10) | 真实材料、范围与验收 | S11,S16,S18,S30 | 保留。relevant 和 §6 共同限定适用上下文。 |
| [11](/Users/xuebai/.codex/AGENTS.md:11) | 未决重要决策用 grilling | S19,S21,S24,S37 | 保留。规则只针对 consequential unresolved；不针对可查事实或已决事项。 |
| [12](/Users/xuebai/.codex/AGENTS.md:12) | 记录范围、研究/设计确认与独立推进 | S17,S18,S19,S22 | 保留。此明确审核请求授权此次官方资料研究，不要求重复确认。 |
| [16](/Users/xuebai/.codex/AGENTS.md:16) | 包、版本、维护来源调查 | S15,S16,S18 | 保留。用于选型研究；本轮无选型，不把所有包调查阶段套到规则检查。 |
| [17](/Users/xuebai/.codex/AGENTS.md:17) | 最小候选与完整权衡 | S17,S18,S48 | 保留。属于用户明确选择的研究流程。 |
| [18](/Users/xuebai/.codex/AGENTS.md:18) | 实验假设与正/边界/负例 | S27,S29,S31 | 保留。不构造应用实验；本轮静态审查单独标注。 |
| [19](/Users/xuebai/.codex/AGENTS.md:19) | 文档/源码/运行/结论/验收分开 | S30,S32,S40 | 保留。不把网页说明、哈希或退出码混作实际效果。 |
| [20](/Users/xuebai/.codex/AGENTS.md:20) | 确认关键可行性后定框架 | S17,S18,S48 | 保留。无框架变更请求。 |
| [24](/Users/xuebai/.codex/AGENTS.md:24) | 已确认可行性到架构批准 | S17,S18,S48 | 保留。本文不修改应用架构。 |
| [25](/Users/xuebai/.codex/AGENTS.md:25) | 直接复用、适配、自定义与维护责任 | S18,S48 | 保留。无上游源码复制或新增依赖。 |
| [26](/Users/xuebai/.codex/AGENTS.md:26) | 证据支持自定义代码 | S18,S38,S43 | 保留。不新建审查框架。 |
| [27](/Users/xuebai/.codex/AGENTS.md:27) | 配置复用、第二真实输入、避免推测框架 | S18,S30,S38 | 保留。不声称此单次审核证明跨项目泛化。 |
| [31](/Users/xuebai/.codex/AGENTS.md:31) | 架构/契约/技术/范围变更先审批 | S19,S21,S39,S48 | 保留。候选正确性例外不明确撤销此规则，新条目引用它。 |
| [32](/Users/xuebai/.codex/AGENTS.md:32) | 复用批准、常规执行/重测不重复问 | S19,S21,S28 | 保留。符合授权内推进。 |
| [33](/Users/xuebai/.codex/AGENTS.md:33) | 实际验证、限制、负例、用户验收 | S11,S27,S30,S31,S32,S45 | 保留。静态 PASS 限于文本候选，用户验收未取得。 |
| [37](/Users/xuebai/.codex/AGENTS.md:37) | 唯一权威事实记录、分离证据状态 | S13,S29,S30,S40 | 保留。本文件为此次审核的唯一项目记录。 |
| [38](/Users/xuebai/.codex/AGENTS.md:38) | 按风险缩放、适用阶段、复用已决内容 | S14,S16,S17,S19,S48 | 保留。不为 first test 删除证据门，也不强加不适用的应用步骤。 |
| [39](/Users/xuebai/.codex/AGENTS.md:39) | 专用环境验证 Codex Skills | S09,S29,S35 | 保留。验证器已查到；未修改技能，因此未执行技能验证/行为评测。 |

## Gap

| ID | Meaningful difference / 潜在冲突 | 标准与证据 | Classification / 处理 |
|---|---|---|---|
| G1 | 最小架构不等于任务变更范围最小；现有规则缺少“范围内能正确完成就保持范围”的直接行为要求。 | S12、S18；源行 5、10、31；用户 candidate。 | RESOLVED：新增一条范围规则，保留正确性依赖例外。 |
| G2 | “正确性要求扩展”可能被解释为取消现有 scope 审批。 | 源行 31 明确先审批；candidate 没有撤销审批。 | RESOLVED：同时满足两者，先提出必要的最小扩展，再按 §5 获批执行。 |
| G3 | 全阶段流程会不会把简单任务强制变成新项目研究？ | S16、S17、S48；源行 32、38。 | NO_CHANGE：复用已批准设计，按风险缩放；不能据官方可选建议撤销明确用户门。 |
| G4 | 用户优先级、技能阻塞解释、写作风格、自主推进是否缺失？ | S19–26；本次宿主已有明确相关指令。 | NO_CHANGE：在本轮有效系统中已覆盖，不把宿主默认规则全部复制进 AGENTS。跨宿主未验证。 |
| G5 | 如何确保所有 AGENTS 今后始终最新？ | S15、S41；当前只有单次审核授权。 | NO_CHANGE：单次结果不能保证未来；不添加周期、全机器扫描或自动改写。未来维护安排未在本次任务中设计。 |
| G6 | INSTALL/README 使用 .codex/skills，当前官方本地发现指导使用 .agents/skills。 | S36、B；J 的旧例子与新版指导不同。 | NO_CHANGE（AGENTS 目标）：记录文档差异；本轮手动读取技能无需安装。未测试旧路径兼容，不声称 .codex 已不可用。 |
| G7 | starter eval/结构验证能否证明技能实际行为？ | S29–32、J；仓库仅有案例描述，没有执行轨迹。 | NO_CHANGE（AGENTS 目标）：原规则已要求实际证据；本次不新建行为评测系统。运行效果保留为未验证。 |
| G8 | 是否需缩短全局文件、迁移完整研究流程或新增项目指令？ | S06、S14、S48；目标 6935 bytes，20 条个人治理规则。 | NO_CHANGE：没有本轮证据证明迁移是正确性依赖；体积合格不证明最佳，但也不能单凭风格进行跨文件重构。 |

### Grilling

本轮不调用 grilling。当前标准和重新读取的指令足以确定：
- 样式/可选建议不要求撤销用户治理；
- scope 扩展仍须满足源行 31 的批准门；
- 没有取消审批、安装、迁移、调度或额外权限授权。

这是按 editor 的依赖规则避免为已能取证的事项发问；不是复用上一轮答案，也不是用普通问答代替 grilling。若后续要求取消门、迁移流程或设置持续维护，则这些新决策应走 grilling。

## Candidate Learning

- Behavioral goal：适用 AGENTS.md 按当前相关权威指导评估，保留明确用户要求；不宣称永久满足所有可能建议。
- Decision boundary：任务在原范围内能正确完成时，保持变更范围。
- Important exception：正确性确实依赖额外变更时，提出最小必要扩展，解释依赖并遵守现有批准要求。
- 本次范围：当前有效指令链；不是全部项目文件或定时维护系统。

## Decision

CHANGE。

理由：G1 是未明确表达的行为差异；新增一条即可覆盖，同时通过引用 §5 消除 G2。其他审查项没有充分证据支持修改当前 AGENTS。

## Proposed Change

- Target：全局 AGENTS.md 第 1 节，在现有第一条之前新增。
- Current state：有最小充分架构、范围确认和范围变更审批，缺少默认不扩展任务变更范围的明确条款。
- Proposed state：默认范围边界 + 必要正确性扩展 + 依赖解释 + 现有审批。
- Rationale：最小补充，不重写原有 20 条，不把官方可选建议变成新增审批或框架。

仅供审阅，未应用：

```diff
--- a/AGENTS.md
+++ b/AGENTS.md
@@ -4,0 +5 @@
+- Keep changes within the requested scope when the task can be completed correctly there. If correctness requires additional changes, propose the minimum necessary scope expansion, explain the dependency, and obtain approval under Section 5 before executing it.
```

## Validation

### 结果与边界

| Check | Result | Evidence / Limit |
|---|---|---|
| Standard coverage | PASS | Standard Frontier 已按上述维度及相邻搜索饱和；不是绝对完备。 |
| Source traceability | PASS | 每项均有官方来源 ID、强度、适用条件及关联项。 |
| Standard alignment | PASS | 必须机制没有冲突；建议按情境处理，没有把建议误当用户要求的替代。 |
| Behavioral preservation | PASS | 内存候选删除新增行后与原文逐字相等，原有 20 条均保留。 |
| Candidate-learning coverage | PASS | 默认范围限制与正确性例外同时表达；原审批仍有效。 |
| Conflict check | PASS | 引用 §5，避免“必要”被误读为无需批准；不复制已生效的宿主规则。 |
| Regression check | PASS（静态） | 下列边界推理及最小文本差异检查通过。 |
| Frontier exhaustion | PASS | G1/G2 已解决，G3–G8 已给 NO_CHANGE 的目标范围理由；无 NEEDS_DECISION/BLOCKED。 |
| Runtime behavior | 未验证 | 没有应用补丁或启动新代理行为评测。 |
| User acceptance | 待定 | 不以代理判断代替用户验收。 |

### 正常、边界与负例检查

以下是文本语义推理，不是实际代理实验，也不替代真实材料或运行证据。

| 情境 | 候选规则允许/要求的行为 | 静态判断 |
|---|---|---|
| 在已请求文件中即可完整正确修复 | 完成范围内修复，不主动做其他改动。 | PASS |
| 不修复真实关联依赖就无法满足正确性 | 说明具体依赖，提出最小扩展，按 §5 获批后执行。 | PASS |
| 顺手格式化、升级框架或可选重构 | 未证明是正确性依赖，不因“顺手”扩展。 | PASS |
| 仅声称“更好”而没有依赖证据 | 不满足 required for correctness 的条件。 | PASS |
| 必要扩展改变架构、契约或技术 | 同时遵守原 §5 对这些变更的审批要求。 | PASS |
| 用户更新任务范围或明确批准扩展 | 按最新明确要求工作，原 §5/§6 复用授权规则继续有效。 | PASS |
| 本次 no-edit 指令与 editor Apply 步骤并存 | 只返回候选，不应用，保持当前 AGENTS 字节不变。 | PASS |

### 实际命令与结果

1. `test -f /Users/xuebai/.codex/skills/grilling/SKILL.md`：exit 0；只验证依赖文件可用。
2. `command -v codex-skill-validate`：exit 0；返回 `/Users/xuebai/.local/bin/codex-skill-validate`。未执行该验证器，因没有修改技能；其结构验证也不代替行为评测。
3. 内存 Python 检查：读取实际 AGENTS、断言初始 SHA-256、生成候选、检查删除新增行即恢复原文、原 20 条变为候选 21 条、再次读取源文件未改变。exit 0。
   - EXISTING_20_RULES_PRESERVED: PASS
   - ONE_RULE_ADDED_IN_MEMORY: PASS
   - AGENTS_UNCHANGED: PASS
   - Source bytes: 6935
   - Candidate bytes: 7197
   - SHA-256: `a1acc7690963c37f21c908421975c8b42b5a668acf5fa8a45777c4a2dfee1e42`

### 两层复扫

- Standard rescan：依赖、加载、审批、测试证据、模型适用性和维护均在标准清单中；候选未引入新依赖、配置或工作流。未发现需要再开 Standard Frontier 的新适用维度。
- Instruction rescan：新增行只界定本任务变化范围，并引用已有批准门；不改变原 20 条。未发现新内部冲突或回归。
- 因此可以完成本次静态审核。真实采用、重载、跨项目行为和未来时效仍不在已验证结论内。

## Evidence

- 上述 A–J 官方正文和本轮检索扩展。
- [/Users/xuebai/.codex/AGENTS.md](/Users/xuebai/.codex/AGENTS.md)：初始和验证时 SHA-256 相同。
- [editor skill](/Users/xuebai/Downloads/agent-learning-harness-v0.1-visible/skills/agents-md-editor/SKILL.md)：本轮版本要求 Standard Frontier 与 Gap Frontier 同时穷尽。
- [output contract](/Users/xuebai/Downloads/agent-learning-harness-v0.1-visible/skills/agents-md-editor/references/output-contract.md)。
- [README](/Users/xuebai/Downloads/agent-learning-harness-v0.1-visible/README.md)、[INSTALL](/Users/xuebai/Downloads/agent-learning-harness-v0.1-visible/INSTALL.md)、[router snippet](/Users/xuebai/Downloads/agent-learning-harness-v0.1-visible/AGENTS-router-snippet.md)、[starter evals](/Users/xuebai/Downloads/agent-learning-harness-v0.1-visible/evals/agents-md-editor/eval-cases.md)。

本文是审核记录，不是新 AGENTS、技能、持续记忆或自动化。

## 本次重新取证与验证

日期：2026-10-06（Asia/Shanghai）。本次明确请求授权执行 Current Standard → Gap → Adapt → Validate 的只评估流程；不执行 Apply。目标仍为当前目录适用的全局 AGENTS.md，不代表已审查机器上所有项目的 AGENTS.md。

### 当前材料与授权边界

实际重读 editor skill、output contract、grilling skill、全局 AGENTS.md、README、INSTALL、TREE、router snippet、feedback-learning skill/contract、两项 starter eval 及既有记录。全局 AGENTS.md 与用户本次提供的规则一致。全局及 cwd/父目录不存在 AGENTS.override.md，cwd 无 AGENTS.md；`git rev-parse --show-toplevel` exit 128，无 Git 根。`CODEX_HOME` 未设置，用户配置读取到 `model = "gpt-6.1-sol"`，未匹配 project_doc 配置字段；不把配置值当作本次实际模型的运行证明。

轻量持久记忆检索对 agents-md-editor、agent-learning-harness、Current Standard、Candidate Learning 无命中；本次结论没有依赖持久记忆。既有记录作为仓库材料检查，来源与目标均重新核验。

### Current Standard 与 Frontier 复核

本次重新搜索并实际打开 A–J 官方 HTML 来源的相关正文。采用的标准、强度、适用性及关系仍见前文 S01–S48；其中 REQUIRED 指产品机制/结构要求，不表示必须把每项复制进 AGENTS.md。

发现顺序：AGENTS 加载/层级 → prompting 的目标/边界 → best practices 的规划/验证/长期维护 → skills 的发现/资源/用户优先级 → 模型相关自主性/测试尺度 → security 的工具执行边界 → eval 的运行轨迹和负控制。新增线索由插件技能页实际链接到当前模型指导，重新确认该指导要求在所选模型与工作负载上评估。本文未做模型性能实验。

相邻复搜主题包括 scope、instruction conflicts、autonomy、validation、maintenance、correctness、minimal changes。结果没有加入会改变当前目标评估的新适用原则。新出现的 Goals、SDK/sandbox、自建修复循环属于专门实施场景，本次不采用；ExecPlans 搜索结果明确标注 archived，不升级为当前强制规则。Docs MCP 是文档接入选项；现有官方网页工具已满足本次来源核验，不需要安装。

本次最终 Standard rescan：范围规则没有新增工具、依赖或工作流；加载、授权、维护、验证和模型适用维度已纳入。覆盖饱和限于上述权威来源与可用仓库证据，不是绝对完备声明。

### Gap、Adapt 与决策

重新对全部 20 条源规则逐条检查，并复核 G1–G8：

- G1 RESOLVED：现有“最小充分架构”及范围审批不直接表达默认保持任务范围；仍建议新增前文的一条规则。
- G2 RESOLVED：正确性例外与源行 31 可以同时满足；新增规则引用 Section 5，保留先批准再执行的明确用户要求。
- G3/G4/G8 NO_CHANGE：适用阶段、风险缩放、已授权执行和宿主优先级已有覆盖；没有证据支持以可选官方建议撤销用户审批或迁移整个全局流程。
- G5 NO_CHANGE：单次 first test 不能保证所有文件未来始终最新；不把行为目标推断成全机器审查或自动化授权。
- G6 NO_CHANGE（当前 AGENTS 目标）：安装文档的 .codex/skills 与当前官方 .agents/skills 有差异；本次通过源码手动读取技能，不依赖修正安装路径。旧路径兼容性未测试。
- G7 NO_CHANGE（当前 AGENTS 目标）：文本 starter eval 不是实际代理行为实验；全局原文已要求区分静态与运行证据。

Grilling 的 SKILL.md 已加载并向用户宣布；没有进入访谈轮次，因为上述决策由明确用户要求、源行 31/32/38 与官方适用边界解决，没有需要替用户决定的新政策。并非以普通问答替代技能。后续若要求撤销批准门或设计跨项目持续维护，应重新进入该技能的决策流程。

Decision：CHANGE 候选。Target、Current state、Proposed state、Rationale 和 minimal patch 均仍采用前文 Proposed Change；本次没有第二份补丁或替代审批政策。

### 实际验证与限制

1. `codex-skill-validate skills/agents-md-editor`：exit 0，输出 `Skill is valid!`。已检查包装器：它调用专用虚拟环境的 Python 与官方 quick_validate.py。该检查验证技能结构，不能证明行为效果。
2. 内存 Python 候选检查：exit 0；读取源字节与初始 SHA-256，生成一条新增规则的候选，删除新增行后逐字恢复源文；原 20 条全部保留，候选 21 条。再次读取源文相等。
   - `ORIGINAL_RULES_PRESERVED: PASS`
   - `AGENTS_UNCHANGED: PASS`
   - 源文件 6935 bytes；候选 7197 bytes。
   - SHA-256 仍为 `a1acc7690963c37f21c908421975c8b42b5a668acf5fa8a45777c4a2dfee1e42`。
3. 复核前文正常/边界/负例的文本语义：范围内可正确完成、真实依赖要求扩展、可选重构、无证据声称“更好”、架构变化、已批准范围、本次 no-edit 指令，均与候选及原批准门一致。这是人工静态推理，不是执行过的代理行为测试。

输出契约结果：Standard alignment PASS；Behavioral preservation PASS；Conflict check PASS；Regression check PASS（静态）。来源可追溯、候选行为与正确性例外覆盖、双层复扫均完成；本轮 Gap Frontier 无 NEEDS_DECISION/BLOCKED 项。没有应用补丁、启动代理运行评测、验证新会话重载或证明跨项目泛化。用户验收仍待定。

本次仅更新这份唯一项目审核记录，未修改 AGENTS.md、技能、安装文档、配置或持久记忆。
