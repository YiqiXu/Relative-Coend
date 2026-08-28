# Adversarial review receipt

Date: 2026-08-26

Artifact: the unified manuscript Relative Cowedges and Coends over a Site.

Final PDF SHA-256:

    fa69dd47875bdb15ba1720373f8f42b0695a0dc01f560d5b98beca0a9308e885

The review was role-separated.  No reviewer edited the manuscript.

| Track | Adversarial remit |
|---|---|
| Base-change adversary | mates, Beck--Chevalley pasting, relations, and both inverse calculations |
| Foundations adversary | size, relative end, restriction coherence, indexed equivalence, and relative-topos claim strength |
| Fubini/reader adversary | simultaneous dinaturality, stable inner coends, currying, Fubini, novelty, and reader depth |

## Frozen review rounds

1. The first unified candidate had 18 pages and SHA-256
   4d70f70df8b33e702adb3ef9277c967584ad8cf4d8e0ad53e7a693913b502064.
   All three reviewers found no fatal counterexample, but identified major
   proof omissions.
2. The repaired 22-page candidate had SHA-256
   7fa54980c317d1cf8991c5d587a26088fec1b3d29bacb4074ad0f5ac1e460b79.
   Base-change and foundations returned PASS WITH MINOR.  The Fubini track
   returned FAIL because the composition equation for the base maps of the
   inner coend omitted the parameter pseudofunctor compositor.
3. The coherence-repaired candidate had SHA-256
   67906fc8941a723bbf04565fdae084e6c327dfb2ac069b52da3ad5741c2dbbaa.
   Base-change returned PASS, foundations returned PASS, and the
   Fubini/reader track returned PASS WITH MINOR.  Its only remaining findings
   were two duplicated words in cross-reference prose.
4. Those two typography findings were mechanically corrected.  The final
   PDF hash is the one recorded above; no mathematical formula changed after
   the third review round.

## Findings and disposition

| Finding | Initial severity | Disposition |
|---|---:|---|
| S3 omitted preservation of the binary coproduct of the two relation objects | major | Binary coproduct displayed and included in S3 |
| Beck--Chevalley data were not explicitly canonical or pasted coherently | major | Canonical mate, pasting formula, beta compatibility, and chosen-square transport proved |
| Stable base-change inverse proof was compressed into prose | major | Generator equations for a and b, section mate, and both inverse calculations written explicitly |
| Relative end was only described as dual | major | Wedge equations, wedge morphisms, category, and terminal universal object written explicitly |
| Restriction and stable assembly omitted compositor equations | major | Restriction compositor and exact b/phi composition laws added |
| Indexed-equivalence invariance omitted the inverse transport | major | Chosen pseudoinverse, unit/counit, both component formulas, and triangle-identity check added |
| Simultaneous dinaturality was not displayed | major | Separate A- and B-dinaturality equations and common domains added |
| Inner universal cowedge/base-change compatibility was implicit | major | Exact kappa base-change identity added |
| K base-change composition omitted parameter compositor transport | major | Theta transport, typed b composition/unit, and explicit chi-K coherence added |
| Reverse currying omitted the identity-base restriction calculation | minor | Two component equations added before invoking universality |
| Higher-variable Fubini was underdefined | major | Claim removed; the manuscript now states what additional definitions would be required |
| Indexed Fubini was presented without Pitts's earlier use | major novelty boundary | Pitts 1985 pp. 46--47 and 51 added with exact locators |
| Current compact-closed virtual-equipment work was absent | minor novelty boundary | Nickel--Arkor 2026 seminar abstract added and explicitly labelled programme-level |
| Fixed-site results risked sounding intrinsic to relative topoi | major framing | Canonical-stack statement changed to a cartesian section on a fixed site; intrinsic and Morita claims remain open |
| Terminal category was said to have a unique topology | minor | Replaced by the trivial/coarsest topology and unit-constraint formulation |

## Final validation

- TeX Live 2026 latexmk build: clean exit, 22 A4 pages.
- Log scan: no unresolved citation/reference, duplicate destination,
  overfull box, underfull box, or package warning.
- qpdf structural check: passed.
- Fonts: every listed font is embedded, subsetted, and Unicode-mapped.
- Text extraction: passed with layout preservation.
- Visual review: all 22 rendered pages inspected in contact sheets; title,
  mate/pasting pages, generator proof, coherence/Fubini pages, and
  bibliography also inspected at full page resolution.  No clipping,
  collision, blank-page, or ownership-label defect was found.

## Interpretation

PASS means that the assigned adversarial track found no remaining
fatal, major, or minor defect after the stated repairs.  It does not mean
formal verification, independent human refereeing, journal acceptance, or
proof of the open relative co-Yoneda, profunctor-equipment, and
site-presentation-invariance problems.
