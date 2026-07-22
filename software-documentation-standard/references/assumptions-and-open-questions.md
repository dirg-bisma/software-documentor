# Assumptions and Open Questions

In software documentation, silence or guessing leads to catastrophic failures. The AI must explicitly declare missing information rather than inventing it.

## [ASSUMPTION]
Use `[ASSUMPTION]` when you have reasonable grounds to infer something, but it has not been explicitly confirmed by the user/stakeholder.
- **Rule:** Never silently convert assumptions into facts.
- **Example:** "[ASSUMPTION] The client will provide the existing customer master data via CSV before migration."

## [OPEN QUESTION]
Use `[OPEN QUESTION]` when a critical piece of information is entirely missing and you need the stakeholder to answer it.
- **Rule:** Always highlight open questions at the end of the generated document.
- **Example:** "[OPEN QUESTION] What is the expected maximum number of concurrent users during peak hours?"

## [TBD] (To Be Determined)
Use `[TBD]` within the text of a requirement when a specific value is pending confirmation.
- **Rule:** A document with [TBD]s is not final.
- **Example:** "The system shall support [TBD] concurrent users."

## [DECISION]
Use `[DECISION]` to log a previously debated topic that has now been finalized.

## [RECOMMENDATION]
Use `[RECOMMENDATION]` when providing a professional suggestion that the business has not yet requested but would benefit from.
