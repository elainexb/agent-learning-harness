# AGENTS.md Editor starter evals

- Missing meaningful behavior -> CHANGE
- Already covered -> NO_CHANGE
- Consequential repo-specific choice -> use grilling
- Style-only difference -> NO_CHANGE
- Conflicting instructions -> minimal validated correction

## Final decision reporting cases

These cases define expected behavior; they are not captured agent-run results.
Judge decisions against the supplied evidence, not the presence of headings.

| Case | Evidence supplied | Expected result |
|---|---|---|
| Mixed repair targets | A supported AGENTS.md placement defect, an intact approval rule, and obsolete installation instructions | Lead with the specific AGENTS.md update. Explicitly mark placement CHANGE and approval NO_CHANGE with reasons. Identify installation-document CHANGE separately. Cover every reviewed dimension in the final response. |
| Unresolved alongside a known repair | One evidenced repair and a second dimension whose repair depends on an unanswered user policy choice | Preserve the known CHANGE and mark the second NEEDS_DECISION; explain the choice and use grilling. Do not imply that one repair settles the entire audit. |
| Missing evidence affects the decision | A suspected hierarchy defect whose relevant override cannot be inspected, after attempted investigation | Mark the affected repair BLOCKED with the missing evidence, attempted check, specific barrier and next step. Do not convert missing evidence into NO_CHANGE or behavioral PASS. |
| Runtime uncertainty with a supported repair decision | Original clauses and complete proposed relocation are inspectable, placement is confirmed, but runtime routing has not been tested | Separate the supported static repair decision from unverified runtime behavior. Do not automatically label the repair BLOCKED or claim runtime preservation. |
| Narrative-only or linked-only summary (negative) | The final response says “covered,” “supported” or “unverified,” or links a detailed ledger without per-dimension repair decisions | Reject the reporting as incomplete even if the linked ledger is thorough. The final response must directly answer whether AGENTS.md needs updating and show explicit decisions, targets, actions and reasons for every reviewed dimension. |
