# Future Automation Architecture

```mermaid
flowchart TD
A[Topic Discovery]-->B[Topic Scoring]
B-->C[Automated Research]
C-->D[Source Evaluation]
D-->E[Claim Ledger]
E-->F[Fact Verification]
F-->G[Narrative Selection]
G-->H[Script]
H-->I[Accuracy Review]
I-->J[Storyboard]
J-->K[Visual Generation]
K-->L[Narration]
L-->M[Audio]
M-->N[Video Composition]
N-->O[Automated QC]
O-->P{Human Final Review}
P-->Q[Publishing]
Q-->R[Analytics]
R-->S[Performance Feedback]
```

Potential technology categories: LLM APIs, web/search APIs, scholarly APIs, image/video generation, speech synthesis, FFmpeg, YouTube/Meta APIs, object storage/database, GitHub Actions and workflow orchestration.

## Boundaries
- provider-independent interfaces;
- evidence artifacts persist before generation artifacts;
- human approval for factual/sensitive/reconstruction/final publishing gates;
- automation may propose, never silently downgrade an accuracy gate;
- no Phase 1 implementation of credentialed publishing.
