---
name: agents-md-editor
description: >
  Audit or minimally repair AGENTS.md. Use when reviewing agent instructions
  or fixing a known instruction gap.
---

# AGENTS.md Editor

Align AGENTS.md with current authoritative OpenAI/Codex guidance and repository
intent. Prefer the smallest change that materially improves behavior. Historical
assumptions are not current best practice.

## Scope and dependencies

Resolve target, scope, mode, and authorization. Reuse settled approvals;
findings do not authorize applying changes. Respect refusals and excluded material.

Investigate facts before asking. For consequential unresolved choices, load,
announce, and follow installed `grilling`. If unavailable, disclose it and pause
the dependent decision; continue independent authorized work. Generic questions
are not invocation. Clarify other genuine user choices as needed.

## Modes and reading

- **PATCH:** a specific learning, bad case, gap, or change; check its target and
  directly introduced regressions.
- **AUDIT:** whole-system review; investigate every materially relevant dimension.

Read Shared Output, [Decision](references/output-contract.md#decision),
Investigation, and Validation before reviewing. For AUDIT, also read Review Ledger,
Audit Completion, and Final Audit Summary before opening the ledger. Follow
[the contract](references/output-contract.md) throughout; PATCH needs no whole-system ledger.

## Process

1. Establish current authoritative standards; distinguish requirements,
   recommendations, and inference. Search broadly enough that further discovery
   is unlikely to materially change the review.
2. Inspect applicable AGENTS.md files, hierarchy, and repository context.
   Preserve supplied Candidate Learning's behavioral intent.
3. Investigate each dimension's behavior, mechanism, counterexample, and evidence
   using the contract. Written coverage is not behavioral proof.
4. Resolve uncertainty and recommend the minimum repair: MODIFY, MERGE, ADD,
   DELETE, MOVE, or NO_CHANGE. Avoid duplication, bloat, conflicts, and regressions;
   prefer Skills/references for task-specific procedures. Apply only authorized changes.
5. After each finding or repair, rescan conflicts, regressions, gaps, and remaining
   or newly relevant dimensions. Update the AUDIT ledger and continue independent
   authorized checks while other dimensions await decisions or evidence.

## Completion

One repair cannot complete an AUDIT with feasible investigation outstanding.
Unread available evidence is remaining work, not a limitation. Do not finalize
until each relevant dimension meets the contract's closure requirements.

Lead with the repair answer; return findings, supported versus unverified results,
minimum changes, unresolved choices/limitations, and rescan. AUDIT also requires
the ledger, final tables, and Audit Completion. PASS applies only to named checks.
