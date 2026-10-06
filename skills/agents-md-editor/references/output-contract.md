# Output Contract

Lead the final response with the repair answer for the reviewed AGENTS.md:
update it, leave it unchanged, or state why the repair cannot yet be decided.
Name the recommended edit or the specific unresolved choice/evidence.
Keep this answer separate from audit completion and behavioral verification.

## Final Audit Summary
AUDIT mode only. Include a repair summary table in the final response covering
every reviewed repair dimension; do not require the user to open a linked
ledger or infer repair status from narrative findings. Report verification-only
dimensions without an identified repair target in a separate validation or
limitations table with their verification status, missing evidence, barrier,
and concrete next check. Every reviewed dimension must appear in one of these
tables; do not invent a repair target to force a verification question into
CHANGE | NO_CHANGE | NEEDS_DECISION | BLOCKED.

For every repair dimension, state:
- Dimension
- Repair target
- Repair decision: CHANGE | NO_CHANGE | NEEDS_DECISION | BLOCKED
- Recommended action, or the next step needed to decide
- Brief reason supported by the inspected evidence

State whether the reviewed AGENTS.md needs an update. Identify repairs to
skills, installation documentation or other files separately, so their CHANGE
decisions are not mistaken for AGENTS.md edits. Distinguish proposed changes
from applied changes. A known repair does not resolve other dimensions;
retain their explicit NEEDS_DECISION or BLOCKED statuses when applicable.

## Current Standard
List only authoritative guidance that materially affects this change.

For each item include:
- Guidance
- Source
- Strength: REQUIRED | RECOMMENDED | INFERRED

## Gap
Describe the meaningful difference between the current instruction system and the desired state.

## Candidate Learning
If provided, state the behavioral intent that must be preserved.
Otherwise return NONE.

## Decision
CHANGE | NO_CHANGE | NEEDS_DECISION | BLOCKED

Name the target and explain the decision using these meanings, both for the
overall decision and each dimension:
- CHANGE: inspected evidence supports a concrete repair; name the minimum action.
- NO_CHANGE: inspected evidence justifies recommending no repair to the named
  target; give that reason. This is not a behavioral PASS.
- NEEDS_DECISION: an unresolved user choice materially affects the repair;
  identify it and resolve it with grilling when necessary. This includes a
  consequential scope, access, or resource choice needed to obtain repair
  evidence. Raise the choice during the work, not for the first time as a
  final blocker. A pending choice is not a proven inability to obtain evidence.
- BLOCKED: necessary evidence is unavailable and prevents choosing the repair;
  name the repair choice that cannot be made, the missing evidence, attempted
  investigation or explicit scope restriction, and the specific barrier.
  Give an actionable route: the smallest next check, who can enable it, and
  the access or action needed. If no route is currently available, state what
  must change. Resolve user choices first where they could enable the check;
  respect already settled refusals rather than asking again.

Report behavioral verification and its limitations separately. Unverified
runtime behavior alone does not imply BLOCKED if the repair decision is
supported independently. State the supported repair decision and mark the
unperformed verification UNVERIFIED with its limitation and next check.
Do not default to NO_CHANGE merely because behavior is unverified, and do
not relabel a supported repair when an optional verification expansion awaits
the user's answer. If missing evidence could materially change the
repair decision, investigate it or substantiate the blocker rather than
defaulting to NO_CHANGE.

## Audit Completion
AUDIT mode only: COMPLETE | INCOMPLETE.

This is separate from Decision and behavioral verification. COMPLETE means
the relevant feasible investigation within the authorized scope is exhausted,
including substantiated limits and genuine unresolved user decisions; it does
not certify whole-system compliance.

If INCOMPLETE, identify remaining work and why it cannot currently proceed.

## Review Ledger
AUDIT mode only. For every materially relevant dimension, include:
- Expected behavior and applicable scope
- Instruction or mechanism intended to produce it
- Concrete counterexample analysis
- Evidence investigated and its verification scope
- Supported conclusion, reason and action or next step; for repair dimensions,
  the target and explicit repair decision
  (CHANGE | NO_CHANGE | NEEDS_DECISION | BLOCKED); for verification-only
  dimensions, the separate verification status and limitation
- Remaining uncertainty or unresolved user decision
- Remaining checks, or the evidence needed, attempted investigation, and
  specific barrier substantiating an evidence limitation

Written coverage alone is not a behavioral pass. Uninspected available
evidence and unperformed feasible checks are remaining work and cannot
justify closing the dimension.

## Proposed Change
If CHANGE, provide:
- Target
- Current state
- Proposed state
- Rationale
- Minimal patch

## Validation
- Standard alignment: PASS | FAIL | UNVERIFIED
- Behavioral preservation: PASS | FAIL | UNVERIFIED
- Conflict check: PASS | FAIL | UNVERIFIED
- Regression check: PASS | FAIL | UNVERIFIED

For each result, name the object checked, evidence, and verification scope.
Patch checks do not establish whole-system compliance. Report unverified
behavior separately; do not force missing evidence into PASS. If a check
cannot be completed, report it as unverified with the substantiated limitation.
For UNVERIFIED, name the missing evidence and smallest next check, with any
access, resource, or user action needed. Text integrity or a successful skill
validator does not establish behavioral preservation or runtime regression
safety.

## Evidence
List only sources and repository evidence that materially support the decision.
