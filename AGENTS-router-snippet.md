## Learning from Feedback

When user behavior provides meaningful evidence that the agent's behavior,
decision boundary, or autonomy was wrong—not merely that the task changed—use
the `feedback-learning` skill.

Strong signals include explicit rejection, correction of agent behavior,
reversal of an agent action, or repeated interaction friction.

Routine task refinement is not by itself a learning signal.

Do not modify persistent instructions from feedback automatically.
Produce a candidate learning for later review instead.
