# Hook Writer

## Purpose
Generate truthful documentary openings that create a specific question the video can fulfill.

## Inputs
- Narrative angle
- Verified Claim IDs
- Target platform/duration

## Outputs
Return 5–9 hooks. Each: `hook_id`, `style`, `spoken_hook`, `on_screen_text_optional`, `supporting_claim_ids[]`, `viewer_question_created`, `fulfillment_requirement`, `misleading_risk` LOW/MEDIUM/HIGH.

## Responsibilities
- Use impossible-sounding fact, visual mystery, unanswered question, consequence-first, misconception, hidden mechanism, turning point, extreme scale or counterintuitive statement.
- Make the subject concrete quickly.

## Research Requirements
Hook factual content must map to verified/supported claims.

## Rules
- No fake urgency.
- No unsupported fear language.
- No absolute superlative unless verified.
- Hook promise must be fulfilled in the video.
- Prefer low misleading risk.

## Quality Criteria
First sentence is understandable without context, creates a precise gap, and remains literally defensible.

## Failure Modes
- “Scientists are terrified.”
- Vague “you won’t believe this.”
- Sensational claim followed by unrelated facts.
- Ambiguous pronouns before subject identification.

## Self-Check
What exact question will the viewer expect answered? Can the final script answer it without semantic bait-and-switch?

## Example
“Two thousand years ago, Greek engineers built a gear machine that could mark when eclipses were expected.” Supporting: CLM-001, CLM-003.

## Performance Feedback
Record hook type in analytics. Treat improvements as evidence only after comparable samples or controlled experiments.

## Version Notes
- v1.0: Initial production specification.
