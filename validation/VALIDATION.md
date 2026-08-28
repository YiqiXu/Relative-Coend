# Unified-manuscript validation receipt

Date: 2026-08-26

Status: **adversarially reviewed working draft**.  This is a
publication-oriented manuscript, not a release candidate and not an
independently refereed mathematical result.

## Source freeze and literature boundary

The four supplied slide decks remain frozen by title, talk date, physical
page count, logical-slide map, and SHA-256 digest in `source-manifest.json`.
The two 2026 files with the same title are different versions:

- D26-LHC: 92 physical pages, 21 logical slides,
  SHA-256 `0b8347b88d47c63c1fa8e1332d90c99fbfa56b68d7a59ab383c31a6f310b4ddc`.
- D26-TACL: 140 physical pages, 22 logical slides,
  SHA-256 `ac6131fca882e3ef26c9e48a4238bf3dd0849c62353c8b4a28c2c67c9d5f20e9`.

The source roles are separated as follows:

- Caramello--Zanfa supports the fibrewise opposite, canonical stack,
  small-generated-site convention, and relative-topos vocabulary.
- Loregian, Definitions 1.1.4 and 1.1.6 (pp. 23--24), supports the ordinary
  cowedge/coend baseline; Theorem 1.3.1 (pp. 37--39) supports ordinary
  Fubini.
- Shulman, Definition 2.4 (p. 7), Definition 2.10 (p. 8), and Lemma 3.25
  (pp. 21--22), supports the established indexed-coproduct and indexed
  profunctor-composition comparison theory.
- Pitts (1985), Convention and Lemma 1.1 (pp. 46--47) and the proof of
  Theorem 2.3 (p. 51), establishes that coend constructions and Fubini were
  already used in an `S`-indexed setting.
- The published title and abstract of Betti--Walters (1989), DOI
  `10.1016/0022-4049(89)90057-1`, provide a prior-art boundary for an end
  calculus over a base topos; no theorem-level equivalence with the present
  fixed-site construction is claimed.
- Nickel--Arkor's “Coend Calculus in a Compact Closed Virtual Equipment” was
  announced in a Topos Institute seminar abstract on 29 June 2026.  The
  abstract targets Fubini and `Span(E)` examples; no public manuscript was
  located in the present search.
- Drieux's slides support motivation and the announced computation/co-Yoneda
  programme.  They are not used as proofs of the new fixed-base,
  stable-base-change, or Fubini theorems.

Web searches on 2026-08-26 for the two titles announced in the 2026 slides,
“On Indexed Limits and Colimits” and “Yoneda and co-Yoneda Lemma in Indexed
Category Theory”, located no public Drieux--Caramello preprint.  This is a
search result, not evidence that no manuscript exists.

## Mathematical claim status

| Item | Status | Exact hypothesis or boundary |
|---|---|---|
| Localized relative cowedge/coend | candidate definition | fixed small site and indexed coefficient system |
| Localized relative wedge/end | candidate definition | explicit dual dinaturality and base-coherence equations; no end-existence theorem claimed |
| Representing property and uniqueness | proved_in_document | Proposition 3.3 |
| Restriction and coherent canonical base-change maps | proved_in_document | Proposition 4.1 and Theorem 4.3 |
| Indexed-equivalence invariance; terminal-site reduction | proved_in_document | chosen coherent indexed equivalence; Propositions 5.1--5.2 |
| Fixed-base coequalizer formula | proved_in_document | relevant coproducts/coequalizer and every `v_! ⊣ v^*`; no pullback or Beck--Chevalley used |
| Exact stability criterion | proved_in_document | canonical `b_u` is invertible iff the restricted universal cowedge is initial |
| Pullback-deficient-site counterexample | proved_in_document | constant `Set` coefficients on `0 -> 2 <- 1`; all available BC maps are identities, but `b_p,b_q` are not isomorphisms |
| Stable base change | proved_in_document, conditional | chosen pullbacks, Beck--Chevalley, and preservation by reindexing of the displayed coproducts/coequalizers |
| Inner coends form an indexed bifunctor | proved_in_document, conditional | every inner relative coend exists and its canonical base-change maps are invertible |
| Relative Fubini | proved_in_document, conditional | stable-inner hypothesis plus existence of either corresponding outer/simultaneous representing object |
| Equality with Shulman's canceling product | evidence_missing | the two universal problems are not identified in this draft |
| Relative co-Yoneda | evidence_missing | announced in slides; no proof claimed |
| Relative profunctor bicategory | evidence_missing | depends on comparison, units, and associativity beyond Fubini |
| Site-presentation/Morita invariance | evidence_missing | fixed-presentation construction only |

The stable-base-change and Fubini proofs are original in-document arguments.
Three role-separated adversarial agents reviewed the same frozen manuscript
for base-change/mates, foundations/coherence, and Fubini/literature.  After
repairs, all mathematical review tracks returned `PASS`; the review trail is
recorded in `adversarial-review-2026-08-26.md`.  This is internal adversarial
review, not independent human peer review or formal verification.

## Build and artifact checks

- xStyle direct-root TeX/BibTeX preflight: no blocking issue.  The preflight
  does not expand `\input` files and therefore reports zero directly seen
  citations; successful BibTeX compilation and the clean final log supply
  the citation-resolution check.  The guarded receipt is
  `xstyle-unified-compile-report.md`.
- The xTopos chapter-preview depth validator was executed and returned
  `fail` because the inherited phase-0--1 inventory uses the v1 field schema,
  while the current validator requires its v2 source-artifact schema.  The
  exact receipt is `depth-gate-phase23.json`.  The four supplied PDFs were not
  copied into this public-facing repository merely to satisfy that schema;
  no depth-gate pass is claimed.
- Combined manuscript: TeX Live 2026 with `latexmk -pdf`, clean exit, 22 A4
  pages.
- Final PDF SHA-256:
  `fa69dd47875bdb15ba1720373f8f42b0695a0dc01f560d5b98beca0a9308e885`.
- Log scan: no unresolved citation/reference, duplicate destination,
  overfull box, underfull box, or LaTeX-package warning in the final logs.
- `qpdf --check`: no syntax or stream-encoding error on the unified PDF.
- Font check: every listed font is embedded; all are subsetted and
  Unicode-mapped.
- Text extraction: successful with `pdftotext -layout` on the unified PDF.
- Visual inspection: all 22 rendered pages inspected in contact sheets;
  title/contents, mate and Beck--Chevalley pages, generator calculations,
  Fubini coherence, and bibliography also inspected at full-page resolution.
  No clipping, collision, blank page, or ownership-label defect was found.

## Gates intentionally left open

Before submission, the manuscript still needs:

1. independent human specialist review or conventional peer review;
2. a novelty comparison against the full text of Betti--Walters (1989), not
   only its published title/abstract and later retrospective comparisons;
3. an editorial choice of journal, house style, author metadata, and final
   theorem-number/source-locator audit; and
4. a separate theorem before any claim of change-of-site/Morita invariance,
   relative co-Yoneda, or a relative-profunctor equipment.

No commit, push, release, or submission is part of this receipt.
