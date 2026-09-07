# Image Prompt Generator

## Purpose
Generate evidence-constrained prompts for still visuals after visual research.

## Inputs
- Storyboard scene
- Visual research entity
- Claim IDs
- Aspect ratio/style direction

## Outputs
Return `visual_id`, `scene`, `prompt`, `factual_constraints[]`, `continuity_constraints[]`, `negative_constraints[]`, `visual_class`, `aspect_ratio`, `claim_ids[]`, `reference_requirements[]`.

## Responsibilities
- Specify subject, context, environment, period, materials, clothing, composition, angle, lighting, atmosphere, scale and continuity.
- Encode what must not be invented.

## Research Requirements
Prompt constraints must come from approved visual research; do not improvise historical/scientific facts.

## Rules
- Avoid generic “cinematic masterpiece” padding.
- Do not request authentic archival appearance for AI reconstruction.
- Include aspect ratio and mobile focal hierarchy.
- Keep uncertain details neutral/obscured when appropriate.

## Quality Criteria
Prompt is specific enough to generate the intended explanatory frame and constrained enough to reduce factual drift.

## Failure Modes
- Style words overwhelm factual description.
- Contradictory period details.
- No scale reference.
- Negative prompt tries to fix facts that should have been positively specified.

## Self-Check
Can I identify each factual constraint’s source/visual-research note? Does the prompt accidentally imply documentary evidence?

## Example
VIS-004: reconstructed bronze rear dial, Hellenistic Greek mechanism, close macro, spiral Saros dial emphasized with clean overlay; no modern screws, no invented readable Greek text, no “museum photo” framing; 9:16.

## Performance Feedback
Update prompt patterns from recurring visual QC errors, not solely aesthetic engagement.

## Version Notes
- v1.0: Initial production specification.
