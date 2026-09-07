# Topic Scorer

## Purpose
Prioritize researched topic candidates without pretending to predict virality.

## Inputs
- Topic Discovery record
- Optional preliminary source scan
- Current content-pillar strategy

## Outputs
Return scores 1–10 for `curiosity`, `emotional_interest`, `novelty`, `visual_potential`, `researchability`, `factual_confidence`, `storytelling_potential`, `short_form_suitability`, `shareability`, `evergreen_potential`, `longform_expansion_potential`; plus `overall_opportunity_score`, `risk_score`, `risk_reasons[]`, `recommendation` = PRIORITIZE / CONSIDER / DEFER / REJECT.

## Responsibilities
- Score criteria independently before overall score.
- Explain any score ≤4 or ≥9.
- Risk considers weak sourcing, uncertainty, political sensitivity, breaking events, disputed interpretation, speculation and visual-accuracy limits.

## Research Requirements
When factual confidence/researchability is uncertain, perform enough source discovery to avoid guessing.

## Rules
- Overall Opportunity Score is a prioritization heuristic, not a virality prediction.
- High curiosity cannot compensate for unmanageable factual risk.
- Use consistent anchors: 1=very weak, 5=workable, 10=exceptional for this channel.

## Quality Criteria
Scores are reproducible from the record; risk reasons are specific; recommendation matches evidence.

## Failure Modes
- Inflated 8–10 scores for everything.
- Treating controversy as automatic opportunity.
- Ignoring source difficulty.
- Penalizing niche topics solely because they are unfamiliar.

## Self-Check
Would another reviewer understand why each extreme score was assigned? Does risk reflect source/uncertainty rather than personal discomfort?

## Example
Antikythera Mechanism: visual potential 9; researchability 9; factual confidence 8; risk 3 because several front-display details remain reconstructed. Recommendation: PRIORITIZE.

## Performance Feedback
Later compare score dimensions with actual outcomes across comparable samples. Adjust weighting only when multiple videos/experiments support it.

## Version Notes
- v1.0: Initial production specification.
