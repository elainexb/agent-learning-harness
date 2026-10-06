# Output Contract

## Shared Output

Both modes: lead with whether the reviewed AGENTS.md needs updating and name
the edit or unresolved choice/evidence. Separate repair, completion, and
verification; identify other-file repairs and proposed versus applied changes.
PATCH covers only the issue and direct regressions.

Include:

- **Current Standard:** material authoritative guidance, sources, and strength:
  REQUIRED | RECOMMENDED | INFERRED.
- **Gap:** difference between effective instructions and desired behavior.
- **Candidate Learning:** supplied behavioral intent, or NONE.
- **Decision:** target, status below, and evidence-backed reason.
- **Proposed Change:** for CHANGE, target, current/proposed states, rationale, minimal patch.
- **Validation:** checks below, evidence, and limits.
- **Evidence/rescan:** material source/repository evidence and conflicts,
  regressions, gaps, choices, and next steps.

## Investigation

For each dimension, identify expected behavior, scope, and instruction/mechanism.
Attempt a counterexample: can an agent obey instructions yet violate that behavior?
Investigate files, history, tests, measurements, or experiments that could change
the conclusion.
Similar wording, missing evidence, no observed failure, or another repair's
success is not behavioral compliance.

Separate repair and verification evidence; never invent verification-only repair
targets. Proactively surface missing evidence, impact, and smallest next check
during work. Use grilling with bounded options/recommendation for consequential
scope, access, resource, or execution choices; do not re-request settled expansions.

## Decision

Use for overall and per-dimension repair decisions:

- **CHANGE:** inspected evidence supports a concrete repair; name target and minimum action.
- **NO_CHANGE:** inspected evidence supports no repair to the target; explain why.
  This is not behavioral PASS.
- **NEEDS_DECISION:** unresolved user choice materially affects repair or its evidence.
  Raise it during work; use grilling when consequential. A pending choice does not
  prove evidence is unobtainable.
- **BLOCKED:** necessary evidence unavailable, preventing repair choice. Name choice,
  missing evidence, attempted checks or explicit scope restriction, specific barrier,
  and smallest next check with who enables it and needed access/action. Resolve
  enabling choices first; respect settled refusals. If no route exists, explain why
  and what must change.

Supported repair decisions may coexist with UNVERIFIED runtime behavior. Neither
absent verification nor pending optional verification expansion makes repair
BLOCKED or changes its status. Missing evidence does not justify NO_CHANGE:
investigate evidence that could change repair or substantiate its barrier.

## Validation

Report Standard alignment, Behavioral preservation, Conflict check, and Regression
check as PASS | FAIL | UNVERIFIED. Name object, evidence, and static/runtime scope.
Text integrity, valid packages, static patches, or another repair's success do not
prove runtime preservation, regression safety, or whole-system compliance. Missing
evidence is not PASS. UNVERIFIED requires missing evidence, attempted checks or
scope barrier, and next check with needed access/resources/action.

## Review Ledger

AUDIT only. For every materially relevant dimension record:

- Expected behavior/scope and intended instruction/mechanism.
- Concrete counterexample; investigated evidence, results, and verification scope.
- Supported conclusion and reason. Repairs: target, decision, action/next step.
  Verification-only: status/limitation without inventing a repair target.
- Remaining uncertainty, user choices, feasible checks, and needed evidence;
  limitations: attempted investigation, specific barrier, and route forward.

## Audit Completion

AUDIT only: COMPLETE | INCOMPLETE, separate from repair and verification.
COMPLETE exhausts materially relevant feasible investigation within authorized
scope. Each dimension has a supported conclusion, genuine user choice raised
during work, or substantiated limitation. Every suspected gap needs a repair
decision or unresolved reason. Accept limitations only after identifying needed
evidence and substantiating why it cannot be obtained. Unread evidence/unperformed
feasible checks remain work. COMPLETE does not certify behavior or settle every
repair. INCOMPLETE names remaining work and why it cannot proceed.

## Final Audit Summary

AUDIT only. Include ledger, Audit Completion, and applicable tables in final
response; linked ledgers/narrative cannot replace tables. Show every reviewed
dimension:

1. **Repairs:** dimension, target, explicit repair decision, action/next step,
   evidence-backed reason.
2. **Verification-only:** dimension, status, missing evidence, barrier, next check.

Known repairs do not settle other dimensions; retain unresolved statuses.
Other-file edits do not imply AGENTS.md edits. Raise choices needed for repair or
requested verification during work. Every limitation needs an actionable route
or why none exists; a status label alone is insufficient.
