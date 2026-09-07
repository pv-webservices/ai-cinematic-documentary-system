# Quality Control

## Purpose
Run the final multi-stage gate across research, script, visuals, audio and platform requirements.

## Inputs
- Research package
- Approved script
- Storyboard/visual outputs
- Audio/narration plan or assembled video
- Platform checklist

## Outputs
Return `overall_result` PASS/PASS WITH CHANGES/FAIL; sections `research_qc`, `script_qc`, `visual_qc`, `audio_qc`, `platform_qc`; `blocking_issues[]`; `required_changes[]`; `human_review_required[]`; `skill_versions_checked[]`.

## Responsibilities
- Research QC: source adequacy, claim verification, contradictions, recency.
- Script QC: support, uncertainty, hook fulfillment, causality.
- Visual QC: plausibility, artifacts, scale, geography, reconstruction labeling.
- Audio QC: pronunciation, pacing, clarity, balance.
- Platform QC: framing, subtitle safe zones, reuse/copyright/disclosure risk.

## Research Requirements
Re-open evidence for any unresolved blocking claim. Check current platform rules at publication time rather than assuming this repository is always current.

## Rules
- `FAIL` blocks publishing.
- `PASS WITH CHANGES` requires changes and re-check.
- Human final approval remains mandatory in Phase 1.
- No silent override by engagement or schedule pressure.

## Quality Criteria
Blocking issues are explicit and actionable; every stage has a result; no category can be skipped without reason.

## Failure Modes
- Cosmetic pass despite factual blocker.
- “Probably fine” reconstruction.
- Audio/music hides narration.
- Missing asset license.
- Passing because production cost is already sunk.

## Self-Check
Would I defend every major claim and visual representation with the recorded evidence? Is anything likely to mislead a reasonable viewer?

## Example
PASS WITH CHANGES: replace “predict the exact eclipse” with “mark eclipse possibilities”; label intact-device shots as reconstruction; re-check pronunciation of Antikythera; then rerun QC.

## Performance Feedback
Every published correction becomes a QC escape. Log category/severity and update the responsible Skill/workflow when a pattern or serious failure appears.

## Version Notes
- v1.0: Initial production specification.
