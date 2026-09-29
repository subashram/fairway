# Fairway v0.3.1 Release Readiness

Date: 2026-09-29
Fairway task: `FW-416`
Candidate version: `v0.3.1`

## Scope

This candidate groups one reviewed product increment:

- task-scoped, preview-first learned-context capture from cited Fairway facts;
- deterministic lexical retrieval with optional disposable local semantic and
  hybrid ranking;
- bounded knowledge export/import with checksum and authority validation;
- separately budgeted learned-context selection for cold-start packets; and
- a bounded AI Cloud consumer pilot covering relevance, fallback, packet cost,
  stale content, and incorrect-authority observations.

The exact candidate source SHA will be the release-preparation commit containing
this assessment after commit-bound review and push. Production rehearsal and
the annotated tag must bind that SHA.

## Underlying Increment Qualification

- `FW-415` completed independent architecture, governance, and security review
  at commit `412aeb838f37038220222318a91e3f41508a0330`;
- full Go unit, integration, focused race, vet, changed-diff lint, formatting,
  and diff-hygiene checks passed for the increment;
- privacy and custody regressions cover excluded free-form source bodies,
  symlink and traversal rejection, duplicate and oversized bundle entries,
  checksum and metadata validation, embedding bounds, and imported trust
  removal; and
- the AI Cloud pilot recorded calibrated lexical/hybrid results, explicit
  lexical fallback, cold-start byte accounting, stale-corpus limitations, and
  zero incorrect authority transitions in its bounded sample.

## Exact-Candidate Gates

1. Full Go, integration, formatting, lint, release-configuration, migration,
   and Docusaurus production checks pass on the clean candidate.
2. Architecture, governance, operations, and security approve the exact release
   metadata, upgrade guidance, supply-chain posture, and claim boundary.
3. `main` is pushed and CI plus Docs Portal pass for the exact SHA.
4. The production `v0.3.1` rehearsal passes tests, signing, notarization,
   candidate smoke, vulnerability/license/SBOM evidence, signed assurance, and
   immutable packet verification.
5. The annotated tag binds the successful rehearsal run id and promotion
   creates a draft from that verified packet without rebuilding.
6. Draft assets and checksums are inspected before publication; public asset
   URLs and Homebrew fetch are verified before closeout.

## Claim Boundary

`v0.3.1` may claim cited preview-first lesson capture, reviewed Markdown as the
knowledge source, deterministic lexical retrieval, optional disposable hybrid
ranking, fail-visible lexical fallback, bounded portable bundles, and
separately budgeted learned-context selection. It may cite the AI Cloud
assessment as a bounded consumer pilot.

It may not claim authoritative generated interpretation, automatic capture or
promotion, authenticated external provenance, model-independent semantic
accuracy, causal delivery improvement, autonomous execution or review,
sovereign deployment readiness, regulatory certification, independent security
assessment, or a complete AI Quality System.

## Migration And Rollback

This increment adds no database migration. Knowledge pages and source manifests
remain normal Git-managed project files. Semantic indexes and staged portable
bundles are derived local artifacts and may be removed without losing reviewed
knowledge.

Before upgrade, back up the Fairway database and Git-managed knowledge files.
Consumer rollback uses the `v0.3.0` binary and the matching pre-upgrade config.
Preserve any Markdown changes applied while using `v0.3.1` for ordinary Git
review or revert, and remove an incompatible semantic index before running an
older binary. No task, review, evidence, or authority record needs to be
synthesized or rewritten for rollback.

Do not move or recreate an immutable tag. If rehearsal or promotion fails,
leave the version untagged or the draft unpublished, fix the owning defect on
`main`, and rehearse the corrected exact SHA. If a published artifact is wrong,
yank it and cut a new version; never reuse `v0.3.1`.
