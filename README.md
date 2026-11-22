# Unpacking Alpöge's Proof of the Riemann Hypothesis

**A Guided Reconstruction of the Lean Argument**  
Brian Kramer, working with ChatGPT · **v1.1-review** · 21 November 2026

An accessible, detailed mathematical exposition of Levent Alpöge's announced proof of the Riemann Hypothesis and its formalization in Lean. The manuscript traces the analytic reduction, auxiliary arithmetic constructions, and interfaces between them. It is intended for mathematical review, **not** as an independent certification of the proof.

## Publication record

[Zenodo manuscript record](https://zenodo.org/records/24433694) · v1.1-review

## Read and download

- **[Read the manuscript (PDF)](paper/Unpacking_Alpoges_Proof_Of_the_Riemann_Hypothesis_v1.1-review.pdf)** — 137 pages.
- **[LaTeX manuscript (.tex)](source/Unpacking_Alpoges_Proof_Of_the_Riemann_Hypothesis_v1.1-review.tex)** — editable source.
- **[LaTeX bibliography](source/SCHOLARLY_BIBLIOGRAPHY.bib)** and **[editable figures](source/figures/)** — individual source files.

## Repository contents

```text
paper/       Compiled manuscript PDF
source/      LaTeX manuscript, bibliography, and editable TikZ figures
```

## Build from LaTeX

Requires a LaTeX distribution with `latexmk`, `pdflatex`, `biber`, and the packages loaded by the manuscript (including KOMA-Script, `biblatex`, TikZ, and `newtx`). From `source/`:

```bash
latexmk -pdf -interaction=nonstopmode -halt-on-error \
  Unpacking_Alpoges_Proof_Of_the_Riemann_Hypothesis_v1.1-review.tex
```

The manuscript PDF was built from this editable source. All diagrams are editable TikZ.

## Sources and mathematical status

- Alpöge's [announcement and remarks](https://alpo.ge/remark.pdf).
- [Lean source archive](https://github.com/CocoSgt/riemann-hypothesis-lean), with the manuscript referencing revision `7cbf7a0c32fca1badf05931879a37c3f8a2b03b4`.

This is a research exposition for review. Claims regarding verification of the original formal development are attributed within the manuscript; nothing in this repository represents independent mathematical certification.

**Feedback and corrections:** [zetacontinuation@gmail.com](mailto:zetacontinuation@gmail.com).

[**SIGMA Research**](https://sigma-research.duckdns.org/) · v1.1-review
