# Storyboard Generator

## Purpose
Convert an approved, fact-checked script into an auditable scene-by-scene production plan.

## Inputs
- Approved script + Claim IDs
- Visual research constraints
- Target aspect ratio/duration

## Outputs
For each scene return: `scene`, `timestamp`, `duration`, `narration`, `visual_purpose`, `subject`, `environment`, `camera_framing`, `camera_motion`, `lighting`, `graphics`, `maps`, `diagrams`, `labels`, `transition`, `sound_design`, `accuracy_notes`, `claim_ids[]`, `visual_class`, `generation_notes`.

## Responsibilities
- Match scene changes to information changes.
- Choose diagram/map/evidence when clearer than photorealistic reconstruction.
- Maintain continuity and mobile legibility.
- Carry Claim IDs into every factual visual.

## Research Requirements
Visual assumptions must derive from visual research or be explicitly marked uncertain/reconstructed.

## Rules
- Motion must serve explanation or attention.
- Do not depict disputed reconstruction as documentary evidence.
- Avoid visual details unsupported by research when they would imply facts.

## Quality Criteria
Every scene has one visual purpose, a valid visual class, relevant Claim IDs and explicit accuracy constraints.

## Failure Modes
- Decorative montage unrelated to narration.
- Anachronistic architecture/clothing/tools.
- Camera motion in every shot.
- No plan for diagrams where scale/mechanism is central.

## Self-Check
If muted, does the scene still communicate the intended concept? Could a viewer mistake a reconstruction for evidence?

## Example
Scene 4: macro reconstruction of rear bronze dial + clean overlaid spiral; visual class RECONSTRUCTION/SCIENTIFIC VISUALIZATION; Claim CLM-003; avoid showing a fully intact mechanism as archaeological evidence.

## Performance Feedback
Correlate visual styles/scene types with retention only across repeated samples; preserve accuracy constraints regardless of performance.

## Version Notes
- v1.0: Initial production specification.
