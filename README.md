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
mkdir -p .cache/build
(cd source && latexmk -pdf -interaction=nonstopmode -halt-on-error \
  -outdir=../.cache/build relative-coend.tex)
qpdf --check .cache/build/relative-coend.pdf
```

The build leaves its candidate PDF in `.cache/build/`; replacing the reviewed
root PDF is a separate release action.

## Reader and source map

| Reader PDF | Maintained source entrypoint |
|---|---|
| `relative-coend.pdf` | `source/relative-coend.tex` |
| `paper/chapter-previews/phases-0-1/preview.pdf` | `source/chapters/phases-0-1/preview.tex` |
| `paper/chapter-previews/phases-2-3/preview.pdf` | `source/chapters/phases-2-3/preview.tex` |

The canonical chapter bodies remain
`source/chapters/phases-0-1/body.tex` and
`source/chapters/phases-2-3/body.tex`. The root PDF is the primary reader
manuscript; the two `paper/` PDFs are secondary previews. Validation receipts
are archived in `archive/validation/`.
