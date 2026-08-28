# TopPrism Repository README Contract

This contract defines the shared information structure for TopPrism public
repositories. It does not force every project to use the same voice, language,
or architecture diagram.

## Required information

Every original repository README must make these questions answerable near the
top or in a clearly labeled status section:

| Field | Question |
|---|---|
| Purpose | What question or user problem does this repository address? |
| Maturity | Is it production, applied, validated, research, framework, internal, learning or reference material? |
| Evidence | What data, study, benchmark or evaluation supports the claim? |
| Boundary | What does the evidence not prove, and what does the repository not do? |
| Relations | Which repositories are related, and is the relation dependency, consumer, sibling, parent case or reference only? |

Every original code or research repository should also include a minimal
`CITATION.cff` containing only verified title, author and repository URL. Add
version, DOI, paper or deployment claims only when they are explicitly
available and maintained.

## Role-specific sections

- **Customer Decision / Insight**: user question, inputs/outputs, decision boundary, human review.
- **World Model**: semantic objects, data/provenance assumptions, validation and downstream consumers.
- **Decision Engine**: decision variables, constraints, objective, certification level and execution boundary.
- **Decision Science**: research question, experiment design, reproducibility, withdrawn claims and transfer limits.
- **Native AI**: experience/evidence lifecycle, promotion gate, governance and evaluation boundary.
- **Learning Project**: capability learned, failure history, parent project and explicit “not a customer product” statement.
- **Upstream Fork**: preserve upstream README and attribution; put TopPrism purpose, modifications and sync state in `TOPPRISM_NOTES.md`.

## Claim discipline

- Write “the repository reports” unless the result has been independently reproduced in the README's stated environment.
- Separate technical evidence from commercial maturity.
- Separate recommendation from approved decision, and decision from execution.
- Never turn internal evaluation into an external benchmark.
- Never imply that a related repository is a runtime dependency without a versioned interface or an explicit adapter contract.

## Maintenance signals

Each original repository should keep its status and evidence current when a
release, benchmark, deployment boundary or major dependency changes. The
organization profile should link to repositories; it should not duplicate every
repository's detailed claim.
