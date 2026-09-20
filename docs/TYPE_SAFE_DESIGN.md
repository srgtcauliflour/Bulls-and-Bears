# TypeSafe / Jev design contract

Bulls&Bears follows TypeSafe System One guidance:

- deterministic code owns arithmetic, exact lookups, freshness and workflow;
- Jev owns narrow semantic judgments;
- observed facts stay separate from calculated features and model judgments;
- independent questions over one state are submitted together;
- Noul output is probability of yes and has no separate confidence;
- Choice/Score confidence is distribution concentration, not overall workflow correctness;
- typed output is not truth; thresholds and market interpretation require target-domain validation.

Current questions: direction_bias (Choice), rise_supported (Noul), fall_supported (Noul), setup_risk (Score), evidence_quality (Score), signals_conflicting (Noul).

Rise and fall Nouls are independent and are not normalized to 100%.

## v0.3 validation
Historical replay will persist exact state, question-pack version, model, outputs and forward outcome. Calibration and accuracy metrics remain deterministic code.
