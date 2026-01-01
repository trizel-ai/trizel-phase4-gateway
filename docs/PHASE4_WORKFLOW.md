# PHASE-4 WORKFLOW — TESTABILITY HANDLING RULES

Phase-4 evaluates only reduced claims (TCRL output). It never interprets theory text.

## Input
- Reduced claim objects: claims/<OBJECT_ID>/<CLAIM_ID>.json

## Decision Policy (Deterministic)

Given a reduced claim with testability_class:

1) measurable_prediction
- Phase-4 MUST attempt evaluation under declared observable_surface.
- Output decision MUST be one of:
  - TESTED_PASS
  - TESTED_FAIL
  - UNRESOLVED (only if required observations are missing)

2) constrainable
- Phase-4 MUST attempt constraint evaluation under declared constraints.
- Output decision MUST be one of:
  - CONSTRAINED
  - UNRESOLVED (if constraints cannot be applied due to missing data)

3) non_testable_presently
- Phase-4 MUST NOT attempt evaluation.
- Output decision MUST be:
  - NON_TESTABLE_PRESENTLY

## No Privilege / No Dismissal Rule
All theories are handled identically if they provide reduced claims.
No alternative or non-traditional theory receives privilege.
No alternative or non-traditional theory is dismissed a priori.

END.
