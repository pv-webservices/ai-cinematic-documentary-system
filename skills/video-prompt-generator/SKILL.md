# Video Prompt Generator

## Purpose
Generate motion prompts where camera/subject/environment movement improves explanation.

## Inputs
- Approved still/scene concept
- Storyboard
- Visual research constraints
- Desired duration

## Outputs
Return `visual_id`, `starting_state`, `ending_state`, `subject_movement`, `camera_movement`, `environment_movement`, `timing`, `physical_realism`, `visual_focus`, `transition_compatibility`, `factual_constraints[]`, `negative_constraints[]`, `claim_ids[]`.

## Responsibilities
- Choose stable camera when motion adds no information.
- Describe causal/physical movement explicitly.
- Preserve object geometry/continuity across the shot.

## Research Requirements
All scientific/historical movement assumptions must be researched or framed as illustrative.

## Rules
- No meaningless orbiting camera.
- No impossible material behavior.
- No morphing gear teeth/components.
- Do not animate hypothetical events as if archived.

## Quality Criteria
Motion guides attention, preserves realism and ends in a frame compatible with the next transition.

## Failure Modes
- Constant slow motion.
- Camera move obscures labels.
- AI object deformation.
- Motion introduces unsupported action.

## Self-Check
What new information does motion convey? Could the same shot be clearer as a still/diagram?

## Example
Start on corroded fragment; slow controlled push toward visible gear teeth; transition via graphic overlay into labeled reconstructed gear train; preserve fragment geometry; no spontaneous gear motion in the archaeological fragment.

## Performance Feedback
Use visual QC/artifact rates to refine motion constraints; retention gains do not justify physical inaccuracies.

## Version Notes
- v1.0: Initial production specification.
