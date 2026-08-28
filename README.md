# Relative Coend

This repository contains the unified research article **Relative Cowedges and
Coends over a Site**.  It develops the localized universal definition, a
fixed-base coequalizer construction, a stable-base-change theorem under
pullback hypotheses, and a conditional Fubini theorem in one continuously
numbered manuscript.

Current status: adversarially reviewed working draft, not a release
candidate.  Fixed-base existence is proved; stable base change and Fubini
are proved under the hypotheses stated in the manuscript.  The PDF does not
claim relative co-Yoneda, profunctor-composition, or
site-presentation-invariance theorems.

Build the combined manuscript with:

```sh
latexmk -pdf -interaction=nonstopmode -halt-on-error relative-coend.tex
```

The canonical source remains split into two maintenance modules,
`chapters/phases-0-1/body.tex` and `chapters/phases-2-3/body.tex`; only
`relative-coend.tex` is the reader-facing manuscript.  The older preview
wrappers are retained as build aids and do not define separate papers.
