# Visual Research

## Purpose
Determine what people, places, objects, processes and scales should plausibly look like before asset generation.

## Inputs
- Approved storyboard
- Claim Ledger
- Source pack

## Outputs
Return `visual_entities[]` with era/location/materials/clothing/tools/architecture/geography/scale/technology/anatomy/process constraints, `reference_sources[]`, `unknowns[]`, `safe_simplifications[]`, `prohibited_inferences[]`, `recommended_visual_class`.

## Responsibilities
- Research historical period details and scientific scale/mechanism.
- Identify where evidence is too weak for photorealistic specificity.
- Separate actual surviving artifact features from reconstructed missing parts.

## Research Requirements
Use authoritative museum/archive/scientific sources where possible. Reference images require provenance/licensing review before reuse.

## Rules
- Cinematic appeal never overrides known constraints.
- Unknown appearance must be marked unknown, not “filled in” by AI.
- Use abstraction/diagram when reconstruction risk is high.

## Quality Criteria
Each factual visual has enough constraints to prevent obvious anachronism or scientific distortion.

## Failure Modes
- Generic “ancient city” aesthetics.
- Invented inscriptions.
- Wrong scale.
- Mixing centuries/regions because visuals look good.

## Self-Check
What in this frame would a domain expert challenge? Which details are directly known vs reconstructed?

## Example
Antikythera: surviving fragments are corroded bronze; full casing/front gearing is incomplete. Reconstruction prompts must distinguish preserved fragments from modeled complete-device views.

## Performance Feedback
Visual QC incidents feed prohibited-inference lists and prompt constraints. Do not encode one-off aesthetic preference as accuracy policy.

## Version Notes
- v1.0: Initial production specification.
