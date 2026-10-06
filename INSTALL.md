# INSTALL

This package intentionally uses a visible top-level `skills/` directory.

To install into a Codex repository, copy:

skills/feedback-learning
skills/agents-md-editor

into:

.codex/skills/

Your repository should then contain:

.codex/
  skills/
    feedback-learning/
      SKILL.md
      references/
        output-contract.md
    agents-md-editor/
      SKILL.md
      references/
        output-contract.md

Then merge `AGENTS-router-snippet.md` into the applicable `AGENTS.md`.

Prerequisite:
A skill named `grilling` must already be available to Codex.
