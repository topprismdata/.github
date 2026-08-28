# TopPrism Repository README Contract

This contract defines the shared information structure for TopPrism public
repositories. Projects can keep domain-specific terminology and architecture,
but their language entry points must be predictable.

## Language policy

- Public code, research and learning repositories use **English as the primary
  README language**, with a concise Chinese overview near the top.
- China-facing products and knowledge repositories may use **Chinese as the
  primary README language**, with a concise English overview near the top.
- If a repository has `README_CN.md`, `README_EN.md` or `README.zh-CN.md`, the
  language links must be reciprocal and visible near the top of each entry.
- Every top-level README declares `Language / 语言` within its first 15 lines.
- Technical terms, code, API names and data fields remain in their verified
  source language. Full translations require maintainer review.

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
