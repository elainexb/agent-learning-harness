---
name: agents-md-editor
description: >
  Audit or minimally improve AGENTS.md against current authoritative OpenAI
  and Codex guidance. Use PATCH for a known issue and AUDIT for whole-system review.
---

# AGENTS.md Editor

Keep AGENTS.md aligned with current authoritative guidance and repository intent.

Prefer the smallest change that materially improves agent behavior.

Do not rely on this skill's historical assumptions as current best practice.

## Dependency

Use `grilling` only for consequential user or repository decisions that cannot
be resolved from available evidence.

Investigate discoverable facts directly before asking the user.

## Modes

### PATCH

Use for a specific learning, bad case, known gap, or requested change.

Resolve the target and check for directly introduced regressions.

### AUDIT

Use for whole-system review.

Identify the materially relevant review dimensions before concluding.

Do not stop because the first actionable issue has been found or resolved.

## Process

1. **Establish the current standard**
   - Use current authoritative OpenAI and Codex guidance.
   - Distinguish requirements, recommendations, and inference.
   - Search broadly enough that further discovery is unlikely to materially change the review.

2. **Inspect the effective instruction system**
   - Inspect applicable AGENTS.md files, hierarchy, and relevant repository context.
   - Preserve the intent of any provided Candidate Learning.

3. **Evaluate behavior**
   - Compare each materially relevant dimension against the effective instructions.
   - Ask whether an agent could fully follow the instructions while still violating the intended behavior.
   - Do not treat similar wording as proof of behavioral coverage.

4. **Check evidence**
   - Distinguish between a rule being present and the behavior being proven effective.
   - If evidence would materially change the conclusion, investigate available files, history, tests, measurements, or experiments.
   - Do not treat missing evidence as a pass.
   - For every materially relevant review dimension, state the expected behavior and its applicable scope, and identify the instruction or mechanism intended to produce it.
   - Attempt a concrete counterexample: could the agent fully follow the effective instructions while violating that behavior?
   - Investigate available evidence that could materially change the conclusion. Written coverage alone is not a behavioral pass.

5. **Resolve uncertainty**
   - Discoverable fact → investigate directly.
   - Genuine user decision → use `grilling`.
   - Separate evidence needed to choose a repair from evidence needed only to verify behavior. Apply [the decision meanings](references/output-contract.md#decision) before assigning a status; do not invent a repair target for a verification-only question.
   - When missing evidence affects a repair or requested verification, surface its impact and the smallest next check during the work. If that check needs a user choice about scope, access, resources, or execution, present the bounded options and your recommendation; use `grilling` for consequential choices.
   - Reuse existing authorization. Respect explicit refusals and scope limits; do not access excluded material or repeatedly request a settled expansion.
   - Every evidence limitation needs an actionable route: name the missing evidence, the attempted checks or explicit scope barrier, the next check, and the access or user action needed. If no route is currently available, explain why and what would have to change.
   - Do not wait for the user to ask what is still unknown.

6. **Recommend the minimum repair**
   - Prefer MODIFY, MERGE, ADD, DELETE, MOVE, or NO_CHANGE as appropriate.
   - Avoid unnecessary duplication, instruction bloat, conflicts, and regressions.
   - Prefer a Skill or reference document over permanent AGENTS.md instructions when the behavior is task-specific.

7. **Rescan and close every review dimension**
   - After each finding or repair, check for conflicts, regressions, new gaps, and remaining review dimensions.
   - In AUDIT mode, maintain a review ledger covering every materially relevant dimension identified during the audit.
   - Revisit the other dimensions and discover any newly relevant dimensions.
   - For each dimension, record its counterexample analysis, evidence investigated, reason, action or next step, and remaining uncertainty. For repair dimensions, name the target and explicit repair decision (CHANGE | NO_CHANGE | NEEDS_DECISION | BLOCKED). For verification-only dimensions without an identified repair target, record the verification status and limitation separately.
   - An evidence limitation is a valid stopping condition only after identifying the evidence needed and establishing why it cannot be obtained within the authorized scope. Record attempted investigation and the specific barrier.
   - Uninspected available evidence and unperformed feasible checks are remaining work, not evidence limitations.
   - Continue independent authorized checks while user decisions or unavailable evidence block other dimensions.

## Completion

Do not claim that remaining dimensions are compliant unless available evidence supports that conclusion.

In AUDIT mode, resolving one issue is not completion of the audit.

Do not finalize an AUDIT while any materially relevant dimension has an
unperformed feasible investigation within the authorized scope.

Before returning an AUDIT, check the review ledger:
- Every dimension has a supported conclusion, a genuine unresolved user
  decision, or a substantiated evidence limitation.
- Every suspected gap has a repair decision or an explicit reason why
  that decision remains unresolved.
- The final response directly answers whether the reviewed AGENTS.md should
  be updated and includes a summary table with an explicit repair decision
  for every reviewed repair dimension. Show verification-only dimensions in
  a separate validation or limitations table; every reviewed dimension must
  remain visible. A linked ledger or narrative conclusion cannot substitute
  for these tables. Identify repairs to other files separately.
- Every unresolved user choice needed to decide a repair or complete requested
  verification has been raised during the work. Every evidence limitation has
  a concrete route forward or an explanation of why none is currently available.
  A status label alone is not an actionable handoff.
- No dimension is marked compliant merely because similar wording exists,
  no failure was observed, or another repair passed.

Return Audit Completion: COMPLETE | INCOMPLETE for AUDIT mode. COMPLETE
means the relevant feasible investigation is exhausted; it does not mean
every behavior is verified. If INCOMPLETE, identify the remaining work and
why it cannot currently proceed.

Validation PASS results apply only to the explicitly named checks and
objects. They must not imply whole-system compliance.

Read and follow [the output contract](references/output-contract.md) when
preparing the result. Lead with the direct repair answer. Include the final
decision summary, review ledger and Audit Completion in AUDIT mode; keep
PATCH mode scoped to the known issue and directly introduced regressions.

Return:
- material findings,
- what is supported versus still unverified,
- minimum recommended changes,
- unresolved decisions or evidence limitations,
- and the rescan result.
