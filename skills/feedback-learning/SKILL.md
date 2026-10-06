---
name: feedback-learning
description: >
  Analyze meaningful user correction, rejection, dissatisfaction, or interaction
  friction to determine whether it contains a reusable learning for future agent
  behavior. Use when evidence suggests the agent's behavior or decision boundary
  may have been wrong, not merely when the task changed.
---

# Feedback Learning

Turn interaction evidence into a reusable candidate learning.

Do not convert feedback directly into instructions or persistent memory.

## Dependency

Use the `grilling` skill as the shared mechanism for resolving consequential uncertainty.

Do not reproduce grilling logic inside this skill.
Do not ask the user directly when the unresolved question should be handled by `grilling`.
Do not invoke `grilling` when the answer is discoverable from available evidence.

## Process

### 1. Reconstruct

Determine from available evidence:
- what behavior occurred,
- what outcome was intended,
- what behavior would have produced a better outcome.

Distinguish evidence from inference.

### 2. Find the Behavioral Delta

Identify the smallest meaningful difference between observed behavior and preferred future behavior.

Describe behavior, not the wording of the original feedback.

### 3. Resolve the Decision Boundary

Determine whether consequential uncertainty remains.

If unresolved questions could materially change:
- the preferred behavior,
- when it should apply,
- its scope,
- or its legitimate exceptions,

use the `grilling` skill to resolve them.

Use the resolved decisions to define the behavioral boundary.

### 4. Test Generalization

Ask whether the resolved learning:
- would improve the original case,
- transfers to materially similar cases,
- avoids overfitting to incidental details,
- preserves legitimate exceptions and useful autonomy.

Reject or hold the learning when these conditions are not supported.

### 5. Return

Return one:
- ADMIT
- HOLD
- REJECT

For ADMIT, produce the fields defined in `references/output-contract.md`.

This is a candidate learning only.
Do not decide how or where it should be persisted.
