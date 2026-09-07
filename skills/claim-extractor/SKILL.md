# Claim Extractor

## Purpose
Convert source-backed research notes into a Claim Ledger so factual statements can be verified before writing.

## Inputs
- Research brief
- Source pack with evaluated SRC IDs
- Optional research notes

## Outputs
Claim records: `claim_id`, `exact_claim`, `claim_type`, `importance`, `source_ids[]`, `supporting_evidence_summary`, `confidence`, `uncertainty`, `contradictions`, `proposed_script_usage`, `visual_implication`, `verification_status`.

## Responsibilities
- Split compound claims when components require different evidence.
- Mark causal/superlative claims explicitly.
- Preserve contradictions instead of averaging them away.
- Create claims precise enough to be falsifiable.

## Research Requirements
Every major claim needs at least one directly relevant source; seek stronger/multiple evidence for causal, disputed, numerical and extraordinary claims.

## Rules
- Never invent a source ID.
- `UNCERTAIN` is acceptable in research; it is not permission to state the claim as fact.
- Claim wording must not be stronger than evidence.

## Quality Criteria
Major script-worthy statements each have stable IDs and explicit status; a reviewer can trace them to sources.

## Failure Modes
- Claims too vague (“Romans were advanced”).
- Combining fact + interpretation into one record.
- Omitting negative/contradictory evidence.
- Assigning VERIFIED merely because multiple articles repeat the same upstream source.

## Self-Check
Is this claim atomic? What evidence would contradict it? Does the source directly support this exact wording? Is uncertainty visible?

## Example
CLM-003: “The lower back dial encoded a 223-lunar-month Saros cycle used to predict eclipse possibilities.” Type: scientific/historical. Sources: SRC-002. Status: VERIFIED.

## Performance Feedback
Track claim categories involved in corrections. Improve extraction rules if the same hidden compound/causal problem recurs.

## Version Notes
- v1.0: Initial production specification.
