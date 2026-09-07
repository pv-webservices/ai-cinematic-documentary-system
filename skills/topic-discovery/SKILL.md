# Topic Discovery

## Purpose
Generate documentary topics with a central question and enough evidence/visual potential to support a narrative.

## Inputs
- Active content pillars
- Audience profile
- Optional trend/reference inputs
- Excluded/sensitive topics

## Outputs
Return 10–20 records with: `topic_id_candidate`, `working_title`, `central_question`, `topic_category`, `why_interesting`, `curiosity_driver`, `possible_hook`, `visual_opportunities[]`, `research_challenges[]`, `controversy_or_uncertainty`, `source_availability_estimate`, `short_form_suitability`, `long_form_expansion_potential`.

## Responsibilities
- Prefer mechanism, discovery, cause/effect, survival, turning-point or unresolved-question narratives.
- Reject random trivia and topics whose only value is shock.
- Flag topics requiring current-event/real-person stricter review.

## Research Requirements
Use quick discovery research only to estimate whether credible sources exist. Do not treat discovery snippets or Tier 3 pages as final evidence.

## Rules
- Do not write a script.
- Do not fabricate “facts” to make an idea stronger.
- Phrase uncertain premises as questions until researched.
- Prefer Phase 1 Science + History + Mysteries.

## Quality Criteria
At least 80% of returned topics should have a clear central question, plausible Tier 1/Tier 2 source path, and at least three distinct visual opportunities.

## Failure Modes
- Trivia lists.
- Topic premise already assumes a disputed conclusion.
- No credible source path.
- Visually repetitive subjects with no diagram/map alternative.
- Breaking-news dependence in Phase 1.

## Self-Check
For each topic: Is the question answerable? Is there narrative movement? Can I name the likely authoritative source class? Could a truthful hook be written without exaggeration?

## Example
Working title: “The 2,000-Year-Old Machine That Predicted Eclipses”
Central question: How did the Antikythera Mechanism encode astronomical cycles using gears?
Uncertainty: exact full front display remains reconstructed/debated.
Source availability: HIGH (peer-reviewed studies + museum).

## Performance Feedback
Compare approved vs rejected topic patterns and later performance only after enough comparable videos exist. Update topic heuristics from documented analytics/experiments, never one outlier.

## Version Notes
- v1.0: Initial production specification.
