# PHASE-4 EXECUTION DIRECTIVE — TRIZEL (EVALUATION GATEWAY)

## 0. Hard Context Lock (Non-Negotiable)
- Phase-2 and Phase-3 artifacts are frozen in their original repository and must not be modified by this Phase-4 repository.
- This repository implements Phase-4 only: evaluation of pre-reduced, testable claims.
- Phase-4 is not permitted to perform holistic theory comprehension.

## 1. Decisive Rule (Scope Guardrail)
Phase-4 MUST NOT "understand" closed theories.
Phase-4 MAY ONLY:
- validate reduced claim objects,
- map reduced claims to observational constraints,
- produce deterministic evaluation results.

All theory comprehension and reduction MUST occur exclusively in TCRL (Pre-Phase-4).

## 2. Absolute Exclusions
Phase-4 MUST NOT introduce:
- theory endorsement language ("superior", "validated theory", "ToE", "STOE"),
- physical explanation narratives,
- simulation or fitting unless explicitly encoded as a reduced, testable claim method with declared observables,
- any attempt to infer claims from theory text.

## 3. Permitted Outputs (Only)
Phase-4 outputs are restricted to:
- evaluation_result objects under evaluations/
- deterministic logs printed by validators
No other artifact types are permitted.

## 4. Canonical Interfaces
Phase-4 consumes ONLY:
- theory packages produced by TCRL (theories/<THEORY_ID>/tcrl/theory_package.json)
- reduced claims (claims/<OBJECT_ID>/*.json)

Phase-4 produces ONLY:
- evaluation results (evaluations/<OBJECT_ID>/<RUN_ID>/*.json)

## 5. Determinism Requirements
- No network access in CI.
- No timestamps in outputs.
- Lexicographic ordering required for registry-style lists.
- JSON must be stable: UTF-8, sorted keys, fixed indentation.

## 6. Stop Rule
Stop after:
- directives + schemas exist,
- validators + tests pass,
- templates exist.
No expansion into domain-specific physics is allowed during initialization.

END.
