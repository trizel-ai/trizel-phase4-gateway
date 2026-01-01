# TCRL EXECUTION DIRECTIVE — TRIZEL (PRE-PHASE-4)

## Purpose
TCRL (Theory Comprehension & Reduction Layer) exists to transform a closed theory into a set of explicitly stated, testable-or-constrainable claims WITHOUT distorting the theory.

## Non-Negotiable Rule
TCRL is permitted to perform deep holistic analysis of a theory as a closed unit.
TCRL is NOT permitted to:
- test claims,
- classify truth,
- rank theories,
- publish scientific conclusions.

TCRL produces only a "theory package" and "reduced claims" that Phase-4 can later evaluate.

## Inputs
- theory source materials stored under: theories/<THEORY_ID>/source/
- no external network retrieval is required in CI

## Outputs (Only)
- theories/<THEORY_ID>/tcrl/theory_package.json  (schema-governed)
- claims/<OBJECT_ID>/<CLAIM_ID>.json             (schema-governed)

## Required Properties of Reduction
Every reduced claim MUST:
- name the observable or constraint surface explicitly,
- state assumptions explicitly,
- specify pass/fail or constraint logic deterministically,
- include a "loss statement" describing what could not be preserved without distortion.

## Forbidden Content
- no "superiority" or endorsement language,
- no implicit claims,
- no hidden premises,
- no theory comparison.

END.
