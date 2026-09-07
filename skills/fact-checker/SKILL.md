# Fact Checker

## Purpose
Perform a strict sentence-level accuracy review of the script against the Claim Ledger and sources.

## Inputs
- Script with Claim IDs
- Claim Ledger
- Source evaluations
- Uncertainty policy

## Outputs
Return `result` PASS/PASS WITH CHANGES/FAIL, `checks[]` with statement, Claim IDs, issue type, evidence, severity, required wording/action, status; plus `blocking_issues[]`, `unmapped_factual_statements[]`, `uncertainty_upgrades[]`.

## Responsibilities
- Check names, dates, places, quantities, chronology, quotations, scientific explanations, causal language, comparisons, superlatives, historical interpretations and probabilities.
- Detect when editing changed confidence.
- Reject unsupported “proved,” “caused,” “first ever,” “impossible,” “exactly,” etc.

## Research Requirements
Open underlying evidence for contested or high-impact statements; do not fact-check by model memory.

## Rules
- Major `UNCERTAIN` or `REJECTED` claims cannot be stated as fact.
- Missing Claim ID on a significant factual sentence is a review issue.
- If sources disagree materially, require qualified wording or remove the claim.
- FAIL for unresolved blocking factual issues.

## Quality Criteria
Every significant factual sentence is supported or flagged; uncertainty matches canonical labels; causal language is justified.

## Failure Modes
- “Sounds right” verification.
- Checking only dates/names while missing causal overclaim.
- Treating source count as independence.
- Letting retention edits reintroduce exaggeration.

## Self-Check
Can I trace each sentence to evidence? Is the sentence stronger than the Claim Ledger? Would an expert object to the level of certainty?

## Example
Flag: “Scientists proved the front display showed all planets exactly this way.” Required: qualify as a modern reconstruction/model consistent with surviving evidence, not an intact observed display.

## Performance Feedback
Corrections and QC escapes feed this Skill first. Any material factual escape requires a root-cause note and version review.

## Version Notes
- v1.0: Initial production specification.
